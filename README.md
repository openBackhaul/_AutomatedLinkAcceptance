# _AutomatedLinkAcceptance
UserDemand for automation of the link acceptance

The _AutomatedLinkAcceptance UserDemand shall be redesigned from batch execution once a day to device individual execution of a pre-acceptance by the GU on site.  

This redesign will increase the success rate of performing a link acceptance from 75% to 95%.  

The entire process of installing a new device needs to be fully automated to facilitate the GU waiting for the result of a pre-acceptance on site.  

The following figure shows the high-level design of the application interworking:  
![AutomatedLinkAcceptanceFlow](./diagrams/AutomatedLinkAcceptanceFlow.png)  

The following applications are required for implementing the _AutomatedLinkAcceptance UserDemand:  
- AccessPlanningTool  
- [MountingOrchestrator](https://github.com/openBackhaul/MountingOrchestrator)  
- [ConnectionPreparation](https://github.com/openBackhaul/ConnectionPreparation)  
- [MediatorManager](https://github.com/openBackhaul/MediatorManager)  
- [LinkIdIntoLtpWriter](https://github.com/openBackhaul/LinkIdIntoLtpWriter)  
- [MicroWaveDeviceGatekeeper](https://github.com/openBackhaul/MicroWaveDeviceGatekeeper)  
- PerformanceManagement  
- [AccessPlanningToolProxy](https://github.com/openBackhaul/AccessPlanningToolProxy)  
- [MicroWaveDeviceInventory](https://github.com/openBackhaul/MicroWaveDeviceInventory)

