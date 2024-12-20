Release Note

Version 1.0.8.9:
- Thêm completion cho hàm điều khiển thiết bị: func sendControlDeviceMessageWith(_ deviceUUID: String, value: RGBCmdValue, elements: [Int]) -> func sendControlDeviceMessageWith(_ deviceUUID: String,
                                      value: RGBCmdValue,
                                      elements: [Int],
                                      completion: RGBCompletionObject<Bool>?)

- Update api cho IR:
  + Tách hàm tính năng học mã raw và detect protocol điều hoà thành 2 hàm khác nhau
  + Detect protocol cho điều hoà dùng hàm  public func setIRDetectModeFor(deviceType: RGBProductCategoryType,
                                   hub: RGBDevice,
                                   observer: AnyObject?,
                                   isEnable: Bool,
                                   timeout: Int?,
                                   completion: RGBCompletionObject<RGBIrRemoteInfo?>?)

  + Học mã raw dùng hàm func setIRLearningModeFor(deviceType: RGBProductCategoryType,
                                     hub: RGBDevice,
                                     observer: AnyObject?,
                                     isEnable: Bool,
                                     timeout: Int?,
                                     completion: RGBCompletionObject<RGBIrRemoteRawInfo?>?)

  + Đổi tên model RGBIrFanRemoteInfoMessage -> RGBIrRemoteRawInfo (sẽ dùng chứa mã raw dùng cho cả quạt lẫn điều hoà)

