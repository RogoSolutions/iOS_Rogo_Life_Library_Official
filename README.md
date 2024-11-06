Release Note

Version 1.0.7.8
- Test hàm tạo mã đăng kí cho loa xử lý tình trạng không có callback trả về khi loa add thành công
    func generateDeviceActiveCode(locationId: String,
                                         verifyId: String?,
                                         observer: AnyObject?,
                                         didGetCodeCompletion: RGBCompletionObject<RGBActiveCode?>?,
                                         didAddDeviceCompletion: RGBCompletionObject<RGBDevice?>?)
                                         
  Truyền observer = self

