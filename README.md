# _AutomatedLinkAcceptance
UserDemand for automation of the link acceptance

The _AutomatedLinkAcceptance UserDemand shall be redesigned from batchwise execution once a day towards device individual execution of a pre-acceptance by the GU on-site.  

The successrate of executing a link acceptance shall be lifted from 75% to 95% by this redesign.  

The entire process for mounting a new device needs to be fully automated for facilitating the GU waiting for the result of a pre-acceptance on-site.  

The following picture shows the high level design of the interworking of applications:  


The following applications are required for implementing the _AutomatedLinkAcceptance UserDemand:  
- APT  
- [AccessPlanningToolProxy](https://github.com/openBackhaul/AccessPlanningToolProxy)
- [MountingOrchestrator](https://github.com/openBackhaul/MountingOrchestrator)
- [MediatorManager](https://github.com/openBackhaul/MediatorManager)
- 
