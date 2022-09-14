# STM32F3_DFU_Test
USB DFU bootloader firmware with winusb descriptors (for use WinUSB driver)

This firmaware is based on USB DFU bootloader example with next changes:
- Middlewares/STM32_USB_Device_Library/Core/Src/usbd_ctlreq.c: add USBD_GetWinUSBDescriptor() function and add WINUSB_REQ in USBD_StdDevReq() function, add MSFTStringDescriptor;
- USB_DEVICE/App/usbd_desc.c: add CompIDDescriptor, ExtPropsDescriptor and FS_MSFT100StrDesc descriptors
