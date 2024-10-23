Release Note

Version 1.0.7.7
- Sửa lỗi tạo mã đăng nhập dùng khi add smart speaker không có thông tin project (appKey/appSecret)
- Hỗ trợ đổi wifi cho thiết bị wile qua ble (điện thoại phải đặt gần để connect device qua ble):
    - Hàm yêu cầu device quét các wifi khả dụng quanh nó:
    func sendRequestScanWifiOnDeviceWith(deviceId: String,
                                         timeOut: Int?,
                                         completion: RGBCompletionObject<[RGBWifiInfo]?>?) 
                                        
    - Hàm set wifi cho device: 
    func sendRequestSetupWifiWith(deviceId: String,
                                  wifiSsid: String,
                                  wifiPassword: String?,
                                  timeOut: Int?,
                                  completion: RGBCompletionObject<Bool?>?)

