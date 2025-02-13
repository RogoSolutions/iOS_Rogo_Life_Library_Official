Release Note

Version 1.0.9.9:
- Add Rf methods:
        func sendRFSelfTestCommandToAllDevices(inGatewayUuid: String,
                                           completion: RGBCompletionObject<Bool>?)
                                           
        func sendRFSelfTestCommandToDevice(deviceUuid: String,
                                       completion: RGBCompletionObject<Bool>?)
                                       
        func sendRFSelfTestNetworkCommand(_ rootUuid: String,
                                             timeOut: Int?,
                                             completion: RGBCompletionObject<[String : Bool]?>?)
        
        func sendRFDeviceSilenceAlarmCommandToDevice(deviceUuid: String,
                                                 completion: RGBCompletionObject<Bool>?)                                      
- Update IR learning raw 
    

