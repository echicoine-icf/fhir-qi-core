### [qicore-communicationdone](StructureDefinition-qicore-communicationdone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Communication.status: (QI) preparation | in-progress | on-hold | stopped | completed</li>
<li>Communication.payload.content[x]: Message part content</li>
</ul>

<b>Primary code path:</b> reasonCode
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-condition-encounter-diagnosis](StructureDefinition-qicore-condition-encounter-diagnosis.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Condition.category: (QI) category codes</li>
<li>Condition.category: encounter-diagnosis</li>
<li>Condition.code: Identification of the condition, problem or diagnosis</li>
<li>Condition.subject: (QI) Who has the condition?</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationdispensedone](StructureDefinition-qicore-medicationdispensedone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationDispense.status: (QI) preparation​ | in-progress​ | on-hold​ | completed​ | stopped​</li>
<li>MedicationDispense.medication[x]: (QI) What medication was supplied</li>
<li>MedicationDispense.subject: (QI) Who the dispense is for</li>
<li>MedicationDispense.performer.actor: Individual who was performing</li>
<li>MedicationDispense.substitution.wasSubstituted: Whether a substitution was or was not performed on the dispense</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-device](StructureDefinition-qicore-device.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Device.deviceName.name: The name of the device</li>
<li>Device.deviceName.type: udi-label-name | user-friendly-name | patient-reported-name | manufacturer-name | model-name | other</li>
<li>Device.specialization.systemType: The standard that is used to operate and communicate</li>
<li>Device.version.value: The version text</li>
<li>Device.property.type: Code that specifies the property DeviceDefinitionPropetyCode (Extensible)</li>
<li>Device.patient: (QI) Patient to whom Device is affixed</li>
</ul>

<b>Primary code path:</b> type
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-communicationrequest](StructureDefinition-qicore-communicationrequest.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>CommunicationRequest.status: (QI) draft | active | on-hold | revoked | completed | entered-in-error | unknown</li>
<li>CommunicationRequest.payload.content[x]: Message part content</li>
</ul>

<b>Primary code path:</b> category
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-practitioner](StructureDefinition-qicore-practitioner.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Practitioner.identifier: (QI) An identifier for the person as this agent</li>
<li>Practitioner.identifier.system: (QI) The namespace for the identifier value</li>
<li>Practitioner.identifier.value: (QI) The value that is unique</li>
<li>Practitioner.identifier.use: (QI) usual | official | temp | secondary | old (If known)</li>
<li>Practitioner.identifier.system: (QI) The namespace for the identifier value</li>
<li>Practitioner.identifier.value: (QI) The value that is unique</li>
<li>Practitioner.name: The name(s) associated with the practitioner</li>
<li>Practitioner.name.family: Family name (often called 'Surname')</li>
<li>Practitioner.qualification.code: Coded representation of the qualification</li>
</ul>

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-familymemberhistory](StructureDefinition-qicore-familymemberhistory.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>FamilyMemberHistory.status: partial | completed | entered-in-error | health-unknown</li>
<li>FamilyMemberHistory.patient: (QI) Patient history is about</li>
<li>FamilyMemberHistory.relationship: (QI) Relationship to the subject</li>
<li>FamilyMemberHistory.condition.code: (QI) Condition suffered by relation</li>
</ul>

<b>Primary code path:</b> type
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-immunizationrecommendation](StructureDefinition-qicore-immunizationrecommendation.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>ImmunizationRecommendation.patient: (QI) Who this profile is for</li>
<li>ImmunizationRecommendation.date: Date recommendation(s) created</li>
<li>ImmunizationRecommendation.recommendation: (QI) Vaccine administration recommendations</li>
<li>ImmunizationRecommendation.recommendation.forecastStatus: Vaccine recommendation status</li>
<li>ImmunizationRecommendation.recommendation.dateCriterion.code: Type of date</li>
<li>ImmunizationRecommendation.recommendation.dateCriterion.value: Recommended date</li>
</ul>

<b>Primary code path:</b> recommendation.vaccineCode
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-encounter](StructureDefinition-qicore-encounter.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Encounter.identifier.system: The namespace for the identifier value</li>
<li>Encounter.identifier.value: The value that is unique</li>
<li>Encounter.status: (QI) planned | arrived | triaged | in-progress | onleave | finished | cancelled +</li>
<li>Encounter.statusHistory.status: planned | arrived | triaged | in-progress | onleave | finished | cancelled +</li>
<li>Encounter.statusHistory.period: The time that the episode was in the specified status</li>
<li>Encounter.class: (QI) Classification of patient encounter</li>
<li>Encounter.classHistory.class: inpatient | outpatient | ambulatory | emergency +</li>
<li>Encounter.classHistory.period: The time that the episode was in the specified class</li>
<li>Encounter.type: (QI) Specific type of encounter</li>
<li>Encounter.subject: (QI) The patient or group present at the encounter</li>
<li>Encounter.diagnosis.condition: The diagnosis or procedure relevant to the encounter</li>
<li>Encounter.location.location: (QI) Location the encounter takes place</li>
</ul>

<b>Primary code path:</b> type
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-servicerequested](StructureDefinition-qicore-servicerequested.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>ServiceRequest.status: (QI) draft | active | on-hold | completed</li>
<li>ServiceRequest.intent: (QI) proposal | plan | directive | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>ServiceRequest.code: (QI) What is being requested/ordered</li>
<li>ServiceRequest.subject: (QI) Individual or Entity the service is ordered for</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationdispense](StructureDefinition-qicore-medicationdispense.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationDispense.status: (QI) preparation | in-progress | cancelled | on-hold | completed | entered-in-error | stopped | declined | unknown</li>
<li>MedicationDispense.medication[x]: (QI) What medication was supplied</li>
<li>MedicationDispense.subject: (QI) Who the dispense is for</li>
<li>MedicationDispense.performer.actor: Individual who was performing</li>
<li>MedicationDispense.substitution.wasSubstituted: Whether a substitution was or was not performed on the dispense</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-procedurenotdone](StructureDefinition-qicore-procedurenotdone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Procedure.extension: Extension</li>
<li>Procedure.extension: (QI) When the procedure was first captured in the subject's record</li>
<li>Procedure.status: (QI) not-done</li>
<li>Procedure.statusReason: (QI) Reason for the current status</li>
<li>Procedure.code: (QI) What procedure</li>
<li>Procedure.subject: (QI) Who the procedure was performed on</li>
<li>Procedure.performer.actor: The reference to the practitioner</li>
<li>Procedure.focalDevice.manipulated: Device that was changed</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-substance](StructureDefinition-qicore-substance.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Substance.code: (QI) If this describes a specific package/container of the substance</li>
<li>Substance.ingredient.substance[x]: (QI) A component of the substance</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-diagnosticreport-note](StructureDefinition-qicore-diagnosticreport-note.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>DiagnosticReport.status: (QI)registered | partial | preliminary | final +</li>
<li>DiagnosticReport.category: (QI) Service Category</li>
<li>DiagnosticReport.code: (QI) QI-Core Report Code</li>
<li>DiagnosticReport.subject: (QI) The subject of the report - usually, but not always, the patient</li>
<li>DiagnosticReport.media.link: Reference to the image source</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-nutritionorder](StructureDefinition-qicore-nutritionorder.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>NutritionOrder.status: draft | active | on-hold | revoked | completed | entered-in-error | unknown</li>
<li>NutritionOrder.intent: proposal | plan | directive | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>NutritionOrder.patient: (QI) The person who requires the diet, formula or nutritional supplement</li>
<li>NutritionOrder.dateTime: Date and time the nutrition order was requested</li>
</ul>

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-location](StructureDefinition-qicore-location.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Location.name: Name by which a facility or location is known.</li>
<li>Location.position.longitude: Longitude with WGS84 datum</li>
<li>Location.position.latitude: Latitude with WGS84 datum</li>
</ul>

<b>Primary code path:</b> type
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-allergyintolerance](StructureDefinition-qicore-allergyintolerance.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>AllergyIntolerance.code: (QI) Code that identifies the allergy or intolerance</li>
<li>AllergyIntolerance.patient: (QI) Who the sensitivity is for</li>
<li>AllergyIntolerance.reaction.manifestation: Clinical symptoms/signs associated with the Event</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-observation-lab](StructureDefinition-qicore-observation-lab.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Observation.status: (QI) registered | prliminary | final | amended | corrected | cancelled | entered-in-error | unknown</li>
<li>Observation.category: (QI) Classification of  type of observation</li>
<li>Observation.category: (QI) Classification of  type of observation</li>
<li>Observation.code: (QI) Laboratory Test Name</li>
<li>Observation.subject: (QI) Who and/or what the observation is about</li>
<li>Observation.component.code: Type of component observation (code / type)</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-taskdone](StructureDefinition-qicore-taskdone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Task.status: (QI) draft​ | requested​ | received​ | accepted​ | ready | in-progress​ | on-hold​ | completed</li>
<li>Task.intent: (QI) unknown | proposal | plan | order | original-order | reflex-order | filler-order | instance</li>
<li>Task.priority: (QI) routine | urgent | asap | stat</li>
<li>Task.code: (QI) Task Type</li>
<li>Task.executionPeriod: (QI) Start and end time of execution</li>
<li>Task.input.type: Label for the input</li>
<li>Task.input.value[x]: Content to use in performing the task</li>
<li>Task.output.type: Label for output</li>
<li>Task.output.value[x]: Result of output</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-deviceusestatement](StructureDefinition-qicore-deviceusestatement.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>DeviceUseStatement.status: (QI) active | completed | entered-in-error +</li>
<li>DeviceUseStatement.subject: (QI) Patient using device</li>
<li>DeviceUseStatement.device: (QI) Reference to device used</li>
</ul>

<b>Primary code path:</b> device.type
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationadministration](StructureDefinition-qicore-medicationadministration.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationAdministration.status: (QI) in-progress | not-done | on-hold | completed | entered-in-error | stopped | unknown</li>
<li>MedicationAdministration.medication[x]: (QI) What was administered</li>
<li>MedicationAdministration.subject: (QI) Who received medication</li>
<li>MedicationAdministration.effective[x]: (QI) Start and end time of administration</li>
<li>MedicationAdministration.performer.actor: Who performed the medication administration</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-imagingstudy](StructureDefinition-qicore-imagingstudy.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>ImagingStudy.status: registered | available | cancelled | entered-in-error | unknown</li>
<li>ImagingStudy.subject: (QI) Who or what is the subject of the study</li>
<li>ImagingStudy.series.uid: DICOM Series Instance UID for the series</li>
<li>ImagingStudy.series.modality: The modality of the instances in the series</li>
<li>ImagingStudy.series.performer.actor: Who performed the series</li>
<li>ImagingStudy.series.instance.uid: DICOM SOP Instance UID</li>
<li>ImagingStudy.series.instance.sopClass: DICOM class type</li>
</ul>

<b>Primary code path:</b> procedureCode
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-devicerequest](StructureDefinition-qicore-devicerequest.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>DeviceRequest.intent: (QI) proposal | plan | directive | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>DeviceRequest.code[x]: (QI) Device requested</li>
<li>DeviceRequest.subject: (QI) Focus of request</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-adverseevent](StructureDefinition-qicore-adverseevent.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>AdverseEvent.actuality: (QI) actual | potential</li>
<li>AdverseEvent.event: (QI) Type of the event itself in relation to the subject</li>
<li>AdverseEvent.subject: (QI) Subject impacted by event</li>
<li>AdverseEvent.suspectEntity.instance: (QI) Refers to the specific entity that caused the adverse event</li>
</ul>

<b>Primary code path:</b> event
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationadministrationnotdone](StructureDefinition-qicore-medicationadministrationnotdone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationAdministration.extension: Extension</li>
<li>MedicationAdministration.extension: (QI) Recorded</li>
<li>MedicationAdministration.status: (QI) not-done</li>
<li>MedicationAdministration.statusReason: (QI) Reason administration not performed</li>
<li>MedicationAdministration.medication[x]: (QI) What was administered</li>
<li>MedicationAdministration.subject: (QI) Who received medication</li>
<li>MedicationAdministration.effective[x]: (QI) Start and end time of administration</li>
<li>MedicationAdministration.performer.actor: Who performed the medication administration</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationdispensedeclined](StructureDefinition-qicore-medicationdispensedeclined.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationDispense.extension: Extension</li>
<li>MedicationDispense.extension: (QI) Extension</li>
<li>MedicationDispense.status: (QI) declined</li>
<li>MedicationDispense.statusReason[x]: (QI) Why a dispense was not performed</li>
<li>MedicationDispense.medication[x]: (QI) What medication was supplied</li>
<li>MedicationDispense.subject: (QI) Who the dispense is for</li>
<li>MedicationDispense.performer.actor: Individual who was performing</li>
<li>MedicationDispense.substitution.wasSubstituted: Whether a substitution was or was not performed on the dispense</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-immunization](StructureDefinition-qicore-immunization.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Immunization.status: (QI) completed | not-done | entered-in-error</li>
<li>Immunization.vaccineCode: (QI) Vaccine Product Type (bind to CVX)</li>
<li>Immunization.patient: (QI) Who was immunized</li>
<li>Immunization.occurrence[x]: (QI) Vaccine administration date</li>
<li>Immunization.performer.actor: Individual or organization who was performing</li>
<li>Immunization.protocolApplied.doseNumber[x]: Dose number within series</li>
</ul>

<b>Primary code path:</b> vaccineCode
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-immunizationnotdone](StructureDefinition-qicore-immunizationnotdone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Immunization.status: (QI) not-done</li>
<li>Immunization.statusReason: (QI) Reason not done</li>
<li>Immunization.vaccineCode: (QI) Vaccine Product Type (bind to CVX)</li>
<li>Immunization.patient: (QI) Who was immunized</li>
<li>Immunization.occurrence[x]: (QI) Vaccine administration date</li>
<li>Immunization.recorded: (QI) Documented date Immunization did not occur.</li>
<li>Immunization.performer.actor: Individual or organization who was performing</li>
<li>Immunization.protocolApplied.doseNumber[x]: Dose number within series</li>
</ul>

<b>Primary code path:</b> vaccineCode
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medication](StructureDefinition-qicore-medication.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Medication.code: Codes that identify this medication</li>
<li>Medication.ingredient.item[x]: The actual ingredient or content</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-careteam](StructureDefinition-qicore-careteam.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>CareTeam.subject: (QI) Who the care team is for.</li>
<li>CareTeam.participant: Members of the team</li>
<li>CareTeam.participant.role: Type of involvement</li>
<li>CareTeam.participant.member: (QI) Who is involved</li>
</ul>

<b>Primary code path:</b> category
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-deviceprohibited](StructureDefinition-qicore-deviceprohibited.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>DeviceRequest.modifierExtension: Extension</li>
<li>DeviceRequest.modifierExtension: (QI) Extension</li>
<li>DeviceRequest.modifierExtension.url: identifies the meaning of the extension</li>
<li>DeviceRequest.modifierExtension.value[x]: (QI) Value of extension</li>
<li>DeviceRequest.intent: (QI) proposal | plan | directive | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>DeviceRequest.code[x]: (QI) Device requested</li>
<li>DeviceRequest.subject: (QI) Focus of request</li>
<li>DeviceRequest.authoredOn: (QI) When recorded</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-immunizationdone](StructureDefinition-qicore-immunizationdone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Immunization.status: (QI) completed</li>
<li>Immunization.vaccineCode: (QI) Vaccine Product Type (bind to CVX)</li>
<li>Immunization.patient: (QI) Who was immunized</li>
<li>Immunization.occurrence[x]: (QI) Vaccine administration date</li>
<li>Immunization.performer.actor: Individual or organization who was performing</li>
<li>Immunization.protocolApplied.doseNumber[x]: Dose number within series</li>
</ul>

<b>Primary code path:</b> vaccineCode
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-observation-screening-assessment](StructureDefinition-qicore-observation-screening-assessment.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Observation.status: (QI) registered | prliminary | final | amended | corrected | cancelled | entered-in-error | unknown</li>
<li>Observation.category: (QI) Classification of  type of observation</li>
<li>Observation.category: (QI) Classification of  type of observation</li>
<li>Observation.code: (QI) Type of observation (code / type)</li>
<li>Observation.subject: (QI) Who and/or what the observation is about</li>
<li>Observation.component.code: Type of component observation (code / type)</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-claimresponse](StructureDefinition-qicore-claimresponse.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>ClaimResponse.status: (QI) active | cancelled | draft | entered-in-error</li>
<li>ClaimResponse.type: (QI) More granular claim type</li>
<li>ClaimResponse.use: (QI) claim | preauthorization | predetermination</li>
<li>ClaimResponse.patient: (QI) The recipient of the products and services</li>
<li>ClaimResponse.created: (QI) Response creation date</li>
<li>ClaimResponse.insurer: (QI) Party responsible for reimbursement</li>
<li>ClaimResponse.outcome: queued | complete | error | partial</li>
<li>ClaimResponse.item.itemSequence: Claim item instance identifier</li>
<li>ClaimResponse.item.adjudication: (QI) Adjudication details</li>
<li>ClaimResponse.item.adjudication.category: (QI) This code is fixed to 'submitted' to indicate that the adjudication result is on what was submitted.</li>
<li>ClaimResponse.item.detail.detailSequence: (QI) Claim detail instance identifier</li>
<li>ClaimResponse.item.detail.adjudication: Detail level adjudication details</li>
<li>ClaimResponse.item.detail.subDetail.subDetailSequence: Claim sub-detail instance identifier</li>
<li>ClaimResponse.addItem.productOrService: Billing, service, product, or drug code</li>
<li>ClaimResponse.addItem.adjudication: Added items adjudication</li>
<li>ClaimResponse.addItem.detail.productOrService: Billing, service, product, or drug code</li>
<li>ClaimResponse.addItem.detail.adjudication: Added items detail adjudication</li>
<li>ClaimResponse.addItem.detail.subDetail.productOrService: Billing, service, product, or drug code</li>
<li>ClaimResponse.addItem.detail.subDetail.adjudication: Added items detail adjudication</li>
<li>ClaimResponse.total.category: Type of adjudication information</li>
<li>ClaimResponse.total.amount: Financial total for the category</li>
<li>ClaimResponse.payment.type: Partial or complete payment</li>
<li>ClaimResponse.payment.amount: Payable amount after adjustment</li>
<li>ClaimResponse.processNote.text: Note explanatory text</li>
<li>ClaimResponse.insurance.sequence: Insurance instance identifier</li>
<li>ClaimResponse.insurance.focal: Coverage to be used for adjudication</li>
<li>ClaimResponse.insurance.coverage: Insurance information</li>
<li>ClaimResponse.error.code: Error code detailing processing issues</li>
</ul>

<b>Primary code path:</b> type
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-bodystructure](StructureDefinition-qicore-bodystructure.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>BodyStructure.active: (QI) Whether this record is in active use</li>
<li>BodyStructure.location: (QI) Body site</li>
<li>BodyStructure.patient: (QI) Who this is about</li>
</ul>

<b>Primary code path:</b> location
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-practitionerrole](StructureDefinition-qicore-practitionerrole.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>PractitionerRole.identifier: (QI) Business Identifiers that are specific to a role/location</li>
<li>PractitionerRole.identifier.use: (QI) usual | official | temp | secondary | old (If known)</li>
<li>PractitionerRole.identifier.system: (QI) The namespace for the identifier value</li>
<li>PractitionerRole.identifier.value: (QI) The value that is unique</li>
<li>PractitionerRole.active: (QI) Whether this practitioner role record is in active use</li>
<li>PractitionerRole.period: (QI) The period during which the practitioner is authorized to perform in these role(s)</li>
<li>PractitionerRole.telecom.system: (QI) phone | fax | email | pager | url | sms | other</li>
<li>PractitionerRole.telecom.value: (QI) The actual contact point details</li>
<li>PractitionerRole.notAvailable.description: Reason presented to the user explaining why time not available</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationrequested](StructureDefinition-qicore-medicationrequested.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationRequest.status: (QI) active | on-hold | cancelled | completed | stopped | draft</li>
<li>MedicationRequest.intent: (QI) proposal | plan | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>MedicationRequest.medication[x]: (QI) Medication to be taken</li>
<li>MedicationRequest.subject: (QI) Who or group medication request is for</li>
<li>MedicationRequest.substitution.allowed[x]: Whether substitution is allowed or not</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationprohibited](StructureDefinition-qicore-medicationprohibited.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationRequest.status: (QI) active | on-hold | cancelled | completed | stopped | draft</li>
<li>MedicationRequest.intent: (QI) proposal | plan | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>MedicationRequest.doNotPerform: (QI) True if medication was not requested</li>
<li>MedicationRequest.medication[x]: (QI) Medication to be taken</li>
<li>MedicationRequest.subject: (QI) Who or group medication request is for</li>
<li>MedicationRequest.authoredOn: (QI) When request was initially authored</li>
<li>MedicationRequest.reasonCode: (QI) Reason or indication for not ordering the medication</li>
<li>MedicationRequest.substitution.allowed[x]: Whether substitution is allowed or not</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationrequest](StructureDefinition-qicore-medicationrequest.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationRequest.status: (QI) active | on-hold | cancelled | completed | entered-in-error | stopped | draft | unknown</li>
<li>MedicationRequest.intent: (QI) proposal | plan | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>MedicationRequest.medication[x]: (QI) Medication to be taken</li>
<li>MedicationRequest.subject: (QI) Who or group medication request is for</li>
<li>MedicationRequest.substitution.allowed[x]: Whether substitution is allowed or not</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-procedure](StructureDefinition-qicore-procedure.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Procedure.status: (QI) preparation | in-progress | not-done | on-hold | stopped | completed | entered-in-error | unknown</li>
<li>Procedure.code: (QI) What procedure</li>
<li>Procedure.subject: (QI) Who the procedure was performed on</li>
<li>Procedure.performer.actor: The reference to the practitioner</li>
<li>Procedure.focalDevice.manipulated: Device that was changed</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-nonpatient-observation](StructureDefinition-qicore-nonpatient-observation.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Observation.status: (QI) registered | prliminary | final | amended | corrected | cancelled | entered-in-error | unknown</li>
<li>Observation.category: (QI) Classification of type of observation</li>
<li>Observation.code: (QI) Type of observation (code / type)</li>
<li>Observation.subject: (QI) The device/location/implantable device the observation is about</li>
<li>Observation.component.code: Type of component observation (code / type)</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-diagnosticreport-lab](StructureDefinition-qicore-diagnosticreport-lab.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>DiagnosticReport.status: (QI)registered | partial | preliminary | final +</li>
<li>DiagnosticReport.category: (QI) Service category</li>
<li>DiagnosticReport.category: (QI) Service category</li>
<li>DiagnosticReport.code: (QI) US Core Laboratory Report Order Code</li>
<li>DiagnosticReport.subject: (QI) The subject of the report - usually, but not always, the patient</li>
<li>DiagnosticReport.media.link: Reference to the image source</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-devicerequested](StructureDefinition-qicore-devicerequested.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>DeviceRequest.modifierExtension.url: identifies the meaning of the extension</li>
<li>DeviceRequest.modifierExtension.value[x]: (QI) Value of extension</li>
<li>DeviceRequest.intent: (QI) proposal | plan | directive | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>DeviceRequest.code[x]: (QI) Device requested</li>
<li>DeviceRequest.subject: (QI) Focus of request</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-coverage](StructureDefinition-qicore-coverage.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Coverage.identifier.type: Member Number identifier type</li>
<li>Coverage.status: active | cancelled | draft | entered-in-error</li>
<li>Coverage.beneficiary: (QI) Plan beneficiary</li>
<li>Coverage.relationship: Beneficiary relationship to the subscriber</li>
<li>Coverage.payor: (QI) Issuer of the policy</li>
<li>Coverage.class.type: Type of class such as 'group' or 'plan'</li>
<li>Coverage.class.value: Value associated with the type</li>
<li>Coverage.class.type: Type of class such as 'group' or 'plan'</li>
<li>Coverage.class.value: Group Number</li>
<li>Coverage.class.type: Type of class such as 'group' or 'plan'</li>
<li>Coverage.class.value: Plan Number</li>
<li>Coverage.costToBeneficiary.value[x]: The amount or percentage due from the beneficiary</li>
<li>Coverage.costToBeneficiary.exception.type: Exception category</li>
</ul>

<b>Primary code path:</b> type
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-condition-problems-health-concerns](StructureDefinition-qicore-condition-problems-health-concerns.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Condition.category: (QI) category codes</li>
<li>Condition.category: problem-list-item | health-concern</li>
<li>Condition.code: (QI) Identification of the condition, problem or diagnosis</li>
<li>Condition.subject: (QI) Who has the condition?</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-questionnaireresponse](StructureDefinition-qicore-questionnaireresponse.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>QuestionnaireResponse.questionnaire: Form being answered</li>
<li>QuestionnaireResponse.status: in-progress | completed | amended | entered-in-error | stopped</li>
<li>QuestionnaireResponse.subject: (QI) The subject of the questions</li>
<li>QuestionnaireResponse.authored: Date the answers were gathered</li>
<li>QuestionnaireResponse.item.linkId: (QI) Pointer to specific item from Questionnaire</li>
</ul>

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-goal](StructureDefinition-qicore-goal.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Goal.lifecycleStatus: proposed | planned | accepted | active | on-hold | completed | cancelled | entered-in-error | rejected</li>
<li>Goal.description: Code or text describing goal</li>
<li>Goal.subject: (QI) Who this goal is intended for</li>
</ul>

<b>Primary code path:</b> category
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-task](StructureDefinition-qicore-task.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Task.status: (QI) draft​ | requested​ | received​ | accepted​ | rejected | ready​ | cancelled​ | in-progress​ | on-hold​ | failed​ | completed | entered-in-error</li>
<li>Task.intent: (QI) unknown | proposal | plan | order | original-order | reflex-order | filler-order | instance</li>
<li>Task.priority: (QI) routine | urgent | asap | stat</li>
<li>Task.code: (QI) Task Type</li>
<li>Task.executionPeriod: (QI) Start and end time of execution</li>
<li>Task.input.type: Label for the input</li>
<li>Task.input.value[x]: Content to use in performing the task</li>
<li>Task.output.type: Label for output</li>
<li>Task.output.value[x]: Result of output</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationstatement](StructureDefinition-qicore-medicationstatement.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationStatement.status: (QI) active | completed | entered-in-error | intended | stopped | on-hold | unknown | not-taken</li>
<li>MedicationStatement.medication[x]: (QI) What medication was taken</li>
<li>MedicationStatement.subject: (QI) Who is/was taking the medication</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-serviceprohibited](StructureDefinition-qicore-serviceprohibited.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>ServiceRequest.status: (QI) draft | active | on-hold | completed</li>
<li>ServiceRequest.intent: (QI) proposal | plan | directive | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>ServiceRequest.doNotPerform: (QI) True if service/procedure should not be performed</li>
<li>ServiceRequest.code: (QI) What is being requested/ordered</li>
<li>ServiceRequest.subject: (QI) Individual or Entity the service is ordered for</li>
<li>ServiceRequest.authoredOn: (QI) Date request signed</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-relatedperson](StructureDefinition-qicore-relatedperson.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>RelatedPerson.active: (QI) Whether this related person's record is in active use</li>
<li>RelatedPerson.patient: (QI) The patient this person is related to</li>
<li>RelatedPerson.communication.language: The language which can be used to communicate with the patient about his or her health</li>
</ul>

<b>Primary code path:</b> relationship
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-proceduredone](StructureDefinition-qicore-proceduredone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Procedure.status: (QI) preparation | in-progress | ​on-hold​ | stopped​ | completed</li>
<li>Procedure.code: (QI) What procedure</li>
<li>Procedure.subject: (QI) Who the procedure was performed on</li>
<li>Procedure.performer.actor: The reference to the practitioner</li>
<li>Procedure.focalDevice.manipulated: Device that was changed</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationadministrationdone](StructureDefinition-qicore-medicationadministrationdone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationAdministration.status: (QI) in-progress | on-hold | completed | stopped</li>
<li>MedicationAdministration.medication[x]: (QI) What was administered</li>
<li>MedicationAdministration.subject: (QI) Who received medication</li>
<li>MedicationAdministration.effective[x]: (QI) Start and end time of administration</li>
<li>MedicationAdministration.performer.actor: Who performed the medication administration</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-medicationnotrequested](StructureDefinition-qicore-medicationnotrequested.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>MedicationRequest.status: active | on-hold | cancelled | completed | entered-in-error | stopped | draft | unknown</li>
<li>MedicationRequest.intent: proposal | plan | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>MedicationRequest.medication[x]: Medication to be taken</li>
<li>MedicationRequest.subject: Who or group medication request is for</li>
<li>MedicationRequest.substitution.allowed[x]: Whether substitution is allowed or not</li>
</ul>

<b>Primary code path:</b> medication
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-careplan](StructureDefinition-qicore-careplan.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>CarePlan.text.status: generated | additional</li>
<li>CarePlan.text.div: Limited xhtml content</li>
<li>CarePlan.status: draft | active | on-hold | revoked | completed | entered-in-error | unknown</li>
<li>CarePlan.intent: proposal | plan | order | option</li>
<li>CarePlan.category: (QI) Type of plan</li>
<li>CarePlan.category: (QI) Type of plan</li>
<li>CarePlan.subject: (QI) Who the care plan is for.</li>
<li>CarePlan.activity.detail.status: not-started | scheduled | in-progress | on-hold | completed | cancelled | stopped | unknown | entered-in-error</li>
</ul>

<b>Primary code path:</b> category
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-keyelement](StructureDefinition-qicore-keyelement.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Extension.url: identifies the meaning of the extension</li>
<li>Extension.value[x]: Value of extension</li>
</ul>

<!--End Generated Intro (DO NOT REMOVE)-->

### [codeOptions](StructureDefinition-codeOptions.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Extension.url: identifies the meaning of the extension</li>
<li>Extension.value[x]: Value of extension</li>
</ul>

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-taskrejected](StructureDefinition-qicore-taskrejected.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Task.status: (QI) The potential performer who claimed ownership of the task has decided not to execute it prior to performing any action</li>
<li>Task.statusReason: Reason for current status</li>
<li>Task.intent: unknown | proposal | plan | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>Task.executionPeriod: (QI) The timing the task was rejected.</li>
<li>Task.input.type: Label for the input</li>
<li>Task.input.value[x]: Content to use in performing the task</li>
<li>Task.output.type: Label for output</li>
<li>Task.output.value[x]: Result of output</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-communication](StructureDefinition-qicore-communication.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Communication.status: (QI) preparation | in-progress | not-done | on-hold | stopped | completed | entered-in-error | unknown</li>
<li>Communication.payload.content[x]: Message part content</li>
</ul>

<b>Primary code path:</b> reasonCode
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-communicationnotdone](StructureDefinition-qicore-communicationnotdone.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Communication.extension: Extension</li>
<li>Communication.extension: (QI) Captures the recorded date of the communication</li>
<li>Communication.status: (QI) not-done</li>
<li>Communication.statusReason: (QI) Reason for current status</li>
<li>Communication.payload.content[x]: Message part content</li>
</ul>

<b>Primary code path:</b> reasonCode
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-patient](StructureDefinition-qicore-patient.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Patient.identifier: An identifier for this patient</li>
<li>Patient.identifier.system: The namespace for the identifier value</li>
<li>Patient.identifier.value: The value that is unique within the system.</li>
<li>Patient.name: A name associated with the patient</li>
<li>Patient.telecom.system: phone | fax | email | pager | url | sms | other</li>
<li>Patient.telecom.value: The actual contact point details</li>
<li>Patient.gender: male | female | other | unknown</li>
<li>Patient.communication.language: The language which can be used to communicate with the patient about his or her health</li>
<li>Patient.link.other: The other patient or related person resource that the link refers to</li>
<li>Patient.link.type: replaced-by | replaces | refer | seealso</li>
</ul>

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-servicerequest](StructureDefinition-qicore-servicerequest.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>ServiceRequest.status: (QI) draft | active | on-hold | revoked | completed | entered-in-error | unknown</li>
<li>ServiceRequest.intent: (QI) proposal | plan | directive | order | original-order | reflex-order | filler-order | instance-order | option</li>
<li>ServiceRequest.code: (QI) What is being requested/ordered</li>
<li>ServiceRequest.subject: (QI) Individual or Entity the service is ordered for</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-claim](StructureDefinition-qicore-claim.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Claim.status: active | cancelled | draft | entered-in-error</li>
<li>Claim.type: Category or discipline</li>
<li>Claim.use: claim | preauthorization | predetermination</li>
<li>Claim.patient: (QI) The recipient of the products and services</li>
<li>Claim.created: (QI) Resource creation date</li>
<li>Claim.provider: (QI) Party responsible for the claim</li>
<li>Claim.priority: Desired processing ugency</li>
<li>Claim.payee.type: Category of recipient</li>
<li>Claim.careTeam.sequence: Order of care team</li>
<li>Claim.careTeam.provider: Practitioner or organization</li>
<li>Claim.supportingInfo.sequence: Information instance identifier</li>
<li>Claim.supportingInfo.category: Classification of the supplied information</li>
<li>Claim.diagnosis.sequence: (QI) Diagnosis instance identifier</li>
<li>Claim.diagnosis.diagnosis[x]: (QI) Nature of illness or problem</li>
<li>Claim.procedure.sequence: (QI) Procedure instance identifier</li>
<li>Claim.procedure.procedure[x]: (QI) Specific clinical procedure</li>
<li>Claim.insurance: Patient insurance information</li>
<li>Claim.insurance.sequence: Insurance instance identifier</li>
<li>Claim.insurance.focal: Coverage to be used for adjudication</li>
<li>Claim.insurance.coverage: Insurance information</li>
<li>Claim.accident.date: When the incident occurred</li>
<li>Claim.item.sequence: Item instance identifier</li>
<li>Claim.item.productOrService: Billing, service, product, or drug code</li>
<li>Claim.item.detail.sequence: Item instance identifier</li>
<li>Claim.item.detail.productOrService: Billing, service, product, or drug code</li>
<li>Claim.item.detail.subDetail.sequence: Item instance identifier</li>
<li>Claim.item.detail.subDetail.productOrService: Billing, service, product, or drug code</li>
</ul>

<b>Primary code path:</b> type
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-organization](StructureDefinition-qicore-organization.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Organization.identifier.use: (QI) usual | official | temp | secondary | old (If known)</li>
<li>Organization.identifier.value: (QI) The value that is unique</li>
<li>Organization.identifier.use: (QI) usual | official | temp | secondary | old (If known)</li>
<li>Organization.identifier.value: (QI) The value that is unique</li>
<li>Organization.active: Whether the organization's record is still in active use</li>
<li>Organization.name: Name used for the organization</li>
</ul>

<b>Primary code path:</b> type
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-flag](StructureDefinition-qicore-flag.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Flag.status: (QI) active | inactive | entered-in-error</li>
<li>Flag.code: (QI) Coded or textual message to display to user</li>
<li>Flag.subject: (QI) Who/What is flag about?</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-immunizationevaluation](StructureDefinition-qicore-immunizationevaluation.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>ImmunizationEvaluation.status: (QI) completed | entered-in-error</li>
<li>ImmunizationEvaluation.patient: (QI) Who this evaluation is for</li>
<li>ImmunizationEvaluation.date: (QI) Date evaluation was performed</li>
<li>ImmunizationEvaluation.targetDisease: (QI) Evaluation target disease</li>
<li>ImmunizationEvaluation.immunizationEvent: (QI) Immunization being evaluated</li>
<li>ImmunizationEvaluation.doseStatus: (QI) Status of the dose relative to published recommendations</li>
</ul>

<b>Primary code path:</b> targetDisease
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-observation-clinical-result](StructureDefinition-qicore-observation-clinical-result.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Observation.status: (QI) registered | prliminary | final | amended | corrected | cancelled | entered-in-error | unknown</li>
<li>Observation.category: (QI) Classification of  type of observation</li>
<li>Observation.code: (QI) Clinical Test or Procedure Name</li>
<li>Observation.subject: (QI) Who and/or what the observation is about</li>
<li>Observation.component.code: Type of component observation (code / type)</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

### [qicore-simple-observation](StructureDefinition-qicore-simple-observation.html)
<!--Begin Generated Intro Tag (DO NOT REMOVE)-->
<b>Must Have:</b>
<ul>
<li>Observation.status: (QI) registered | prliminary | final | amended | corrected | cancelled | entered-in-error | unknown</li>
<li>Observation.category: (QI) Classification of type of observation</li>
<li>Observation.code: (QI) Type of observation (code / type)</li>
<li>Observation.subject: (QI) Who and/or what the observation is about</li>
<li>Observation.component.code: Type of component observation (code / type)</li>
</ul>

<b>Primary code path:</b> code
<br></br>
(PCPath) This element is the primary code path for this resource

<!--End Generated Intro (DO NOT REMOVE)-->

