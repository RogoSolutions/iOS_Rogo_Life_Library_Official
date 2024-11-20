Release Note

Version 1.0.8.2
- Fix bug missing state in message state v2
- Refactoring:
    func requestStateAndSettingOf(device: RGBDevice) 
    -> func requestStateAndSettingOfDeviceWith(deviceUuid: String)

    func subscribeStateChangeOf(devices: [RGBDevice], observer: AnyObject?, statusChangedHandler: RGBCompletionObject<RGBDeviceState?>?)
    -> func subscribeStateChangeOfDevicesWith(deviceUuids: [String], observer: AnyObject?, statusChangedHandler: RGBCompletionObject<[RGBDeviceState]?>?)

