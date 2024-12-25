Release Note

Version 1.0.9.1:
- Thêm callback response cho hàm:
    func requestStateOfDeviceWith(deviceUUID: String,
                                  timeOut: Int?,
                                  completion: RGBCompletionObject<RGBDeviceState?>?)

- Hàm subscribeStateChangeOfDeviceWith nếu không có state không trả về callback
