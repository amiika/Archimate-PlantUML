

# Archimate template

All available element:

```plantuml
@startuml
!include ../Archimate.puml

title Archimate Example - Elements

Strategy_Resource(SR_01, "Resource")
Strategy_Capability(SC_01, "Capability")
Strategy_CourseOfAction("SA_01", "Course of Action")

Business_Actor(BA_01, "Business Actor")
Business_Role(BR_01, "Business Role")
Business_Collaboration(BC_01, "Business Collaboration")
Business_Interface(BI_01, "Business Interface")
Business_Process(BP_01, "Business Process")
Business_Function(BF_01, "Business Function")
Business_Interaction(BIt_01, "Business Interaction")
Business_Event(BE_01, "Business Event")
Business_Service(BS_01, "Business Service")
Business_Object(BO_01, "Business Object")
Business_Contract(BCt_01, "Contract")
Business_Representation(BRep_01, "Representation")
Business_Product(BPr_01, "Product")

Application_Component(AC_01, "Application Component")
Application_Collaboration(ACol_01, "Application Collaboration")
Application_Interface(AI_01, "Application Interface")
Application_Function(AF_01, "Applcation Function")
Application_Interaction(AInt_01, "Application Interaction")
Application_Process(AP_01, "Application Process")
Application_Event(AE_01, "Application Event")
Application_Service(AS_01, "Application Service")
Application_DataObject(AD_01, "Data Object")


Technology_Node(TN_01, "Node")
Technology_Device(TD_01, "Device")
Technology_SystemSoftware(TSS_01, "System Software")
Technology_Collaboration(TC_01, "Technology Collaboration")
Technology_Interface(TI_01, "Technology Interface")
Technology_Path(TP_01, "Path")
Technology_CommunicationNetwork(TCN_01, "Communication Network")
Technology_Function(TF_01, "Technology Function")
Technology_Process(TPr_01, "Technology Process")
Technology_Interaction(TInt_01, "Technology Interaction")
Technology_Event(TE_01, "Technology Event")
Technology_Service(TS_01, "Technology Service")
Technology_Artifact(TA_01, "Artifact")

'Physical Elements
Physical_Equipment(PE_01, "Equipment")
Physical_Facility(PF_01, "Facility")
Physical_DistributionNetwork(PDN_01, "Distribution Network")
Physical_Material(PM_01, "Material")

Motivation_Stakeholder(MS_01, "Stakeholder")
Motivation_Driver(MD_01, "Driver")
Motivation_Assessment(MA_01, "Assessment")
Motivation_Goal(MG_01, "Goal")
Motivation_Outcome(MO_01, "Outcome")
Motivation_Principle(MP_01, "Principle")
Motivation_Requirement(MR_01, "Requirement")
Motivation_Constraint(MC_01, "Constraint")
Motivation_Meaning(MM_01, "Meaning")
Motivation_Value(MV_01, "Value with some longer text\nand multiline\nand more")

'Implementation Elements
Implementation_WorkPackage(IWP_01, "Work Package")
Implementation_Deliverable(ID_01, "Deliverable")
Implementation_Event(IE_01, "Event")
Implementation_Plateau(IP_01, "Plateau")
Implementation_Gap(IG_01, "Gap")

'Other Elements
Grouping(G_01, "Grouping") {
    Junction_Or(JO_01, "or")
    Junction_And(JA_01, "and")
}
Group(G_02, "Group") {
    Other_Location(OL_01, "Location")
}

@enduml
```

#Does this work?

Yes.

```plantuml
@startuml Example-CompositionDown
!include ../Archimate.puml
Motivation_Stakeholder(StakeholderElement, "Stakeholder Description")
Business_Service(BService, "Business Service")

Rel_Composition_Down(StakeholderElement, BService, "Description for the relationship")
@enduml
```