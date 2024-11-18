# _AutomatedLinkAcceptance
UserDemand for automation of the link acceptance

The _AutomatedLinkAcceptance UserDemand is already implemented as the AutomatedLinkAcceptanceProxy (ALAP) passing data from MicrowaveDeviceInventory (MWDI) to the AccessPlanningTool (APT) for comparing device data from live network with planning data.

The UserDemand is operational, but suffers from unsatisfying performance due to root causes mostly outside the APT and MW SDN domain.

A redesign of the UserDemand from batchwise execution once a day towards device individual execution by the GUI on-site is under implementation.
