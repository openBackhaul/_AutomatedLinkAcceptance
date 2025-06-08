# Linear Process

The former structuring of the AutomatedMounting ...

![formerStructure](./diagrams/FormerStructure.png)  

... implements a linear process.  

Example steps in this process:  
- prepare device  
- create mediator  
- create mount point at controller  
- ...  

It fulfils a single purpose: Make a REST interface available for a new device.  

During discussing the MediatorManager, we saw that further function would be reasonable:  
- Support of non-traffic-affecting mediator update  
![MovingMediators](./diagrams/MovingMediators.png)  

- Device configuration hygiene    
need for a separate application for cleaning up SDN configurations on the device has been documented into the roadmap  


# New Concept  

The former MediatorManager that was just for providing mediators will be expanded to a DeviceDomainManager, which will be responsible for providing and maintaining the transport of the management connection between NetconfClient at the MountPoint (inside the Controller) and device.  

This shall include  
- managing the mediatorProcesses,  
- implementing load sharing in general, but also in case of a crash of a mediatorVM and for supporting mediator updates  
- initiating the device configurations for the SNMP/Qx connections to the mediatorProcesses  
- managing the NetconfClient configurations at the MountPoints (via ControllerDomainManager)  
- cleaning up configuration artifacts on the devices and mediatorVms.  

