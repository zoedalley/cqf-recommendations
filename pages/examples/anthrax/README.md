---
layout: example-default
title: Anthrax Post-Exposure Prophylaxis Example
---

# README
This README.txt file describes the contents of this software delivery. Unless otherwise noted, 
this software carries an Apache 2.0 license.

(c) 2019 The MITRE Corporation. All Rights Reserved. Approved for Public Release: 19-2048. Distribution Unlimited.

## Overview
The contents of these directories constitute the updates made to the Anthrax Post-Exposure
Prophylaxis CDS Artifact as part of Task 1 of Part 2 of the Adapting Emergency Preparedness
and Response Guidelines to the Digital Age (Clinical Decision Support) project. During Part
1 of said project, an Anthrax Post-Exposure Prophylaxis CDS Artifact was developed and validated
by the Health FFRDC (operated by The MITRE Corporation). The updates made to the CDS Artifact
are in response to feedback regarding the desire to include the most recent Fast Healthcare
Interoperability Resources (FHIR) specification and standards.

## Contents
This software delivery includes the following directories, which are each described below.
- cql: Contains the Clinical Quality Language (CQL) code that constitutes the updated artifact.
- DetectedIssue: Provides example DetectedIssue FHIR resources produced by the artifact.
- Device: Provides example Device FHIR resources produced by the artifact.
- Flag: Provides example Flag FHIR resources produced by the artifact.
- Library: Library FHIR resources that act as containers for the updated artifact.
- PlanDefinition: Provides example PlanDefinition FHIR resources produced by the artifact.

### cql
The cql directory contains the following subdirectories.
- [FHIRv102](cql/FHIRv102): CQL code for version of artifact that uses a FHIR DSTU2 (v1.0.2) data model.
- [FHIRv300](cql/FHIRv300): CQL code for version of artifact that uses a FHIR STU3 (v3.0.0) data model.
- [FHIRv400](cql/FHIRv400): CQL code for version of artifact that uses a FHIR R4 (v4.0.0) data model.

Each subdirectory contains versions of the following CQL libraries:
- Anthrax_Post_Exposure_Prophylaxis: The main body of the artifact CQL.
- CDS_Connect_Commons: An open-source CQL library with commonly-used functions.
- CDC_Common_Logic: A CQL library with commonly-used functions specific to this task.
- FHIR_Helpers: An open-source CQL library for helping with the FHIR data model.

In addition, each subdirectory may contain one or more text files with version-specific
information.

### DetectedIssue
The artifact CQL has the ability to generate one or more alerts using the FHIR DetectedIssue
resource. The DetectedIssue directory contains examples of the different types of alerts
which can be generated by the CQL. The DetectedIssue directory contains the following
subdirectories:
- [FHIRv102](resources/DetectedIssue/FHIRv102): Example DetectedIssue alerts in FHIR DSTU2 (v1.0.2) format.
- [FHIRv300](resources/DetectedIssue/FHIRv300): Example DetectedIssue alerts in FHIR STU3 (v3.0.0) format.
- [FHIRv400](resources/DetectedIssue/FHIRv400): Example DetectedIssue alerts in FHIR R4 (v4.0.0) format.

Each subdirectory should contain the FHIR resources in JSON format, as well as a text
file that captures the results from validating said resources using the
[FHIR Validator](http://wiki.hl7.org/index.php?title=Using_the_FHIR_Validator).

### Device
The artifact CQL uses a FHIR Device resource to identify itself in the other FHIR resources
that it produces. The Device directory contains the following subdirectories:
- [FHIRv102](resources/Device/FHIRv102): Device resource in FHIR DSTU2 (v1.0.2) format.
- [FHIRv300](resources/Device/FHIRv300): Device resource in FHIR STU3 (v3.0.0) format.
- [FHIRv400](resources/Device/FHIRv400): Device resource in FHIR R4 (v4.0.0) format.

Each subdirectory should contain the FHIR resources in JSON format, as well as a text
file that captures the results from validating said resources using the
[FHIR Validator](http://wiki.hl7.org/index.php?title=Using_the_FHIR_Validator).

### Flag
The artifact CQL has the ability to generate one or more alerts using the FHIR Flag
resource. The Flag directory contains examples of the different types of alerts
which can be generated by the CQL. The Flag directory contains the following
subdirectories:
- [FHIRv102](resources/Flag/FHIRv102): Example Flag alerts in FHIR DSTU2 (v1.0.2) format.
- [FHIRv300](resources/Flag/FHIRv300): Example Flag alerts in FHIR STU3 (v3.0.0) format.
- [FHIRv400](resources/Flag/FHIRv400): Example Flag alerts in FHIR R4 (v4.0.0) format.

Each subdirectory should contain the FHIR resources in JSON format, as well as a text
file that captures the results from validating said resources using the
[FHIR Validator](http://wiki.hl7.org/index.php?title=Using_the_FHIR_Validator).

### Library
FHIR Library resources were generated using the updated artifact CQL, and act as formatted
containers for the artifact and provide key information in context. The Library directory
contains the following subdirectories:
- [FHIRv102](resources/Library/FHIRv102): Library resources in FHIR DSTU2 (v1.0.2) format.
- [FHIRv300](resources/Library/FHIRv300): Library resources in FHIR STU3 (v3.0.0) format.
- [FHIRv400](resources/Library/FHIRv400): Library resources in FHIR R4 (v4.0.0) format.

Each subdirectory should contain the FHIR resources in JSON format, as well as a text
file that captures the results from validating said resources using the
[FHIR Validator](http://wiki.hl7.org/index.php?title=Using_the_FHIR_Validator). Where
appropriate, the resources are also validated against the profile available at:
- [cpg-library](../../StructureDefinition-cpg-library.html)

### PlanDefinition
The artifact CQL has the ability to generate an order set using the FHIR PlanDefinition
and ActivityDefinition resources (the latter or which are contained in the former). The
PlanDefinition directory contains examples of the different types of order sets which can
be generated by the CQL. The PlanDefinition directory contains the following subdirectories:
- [FHIRv102](resources/PlanDefinition/FHIRv102): Example PlanDefinition resources in FHIR DSTU2 (v1.0.2) format.
- [FHIRv300](resources/PlanDefinition/FHIRv300): Example PlanDefinition resources in FHIR STU3 (v3.0.0) format.
- [FHIRv400](resources/PlanDefinition/FHIRv400): Example PlanDefinition resources in FHIR R4 (v4.0.0) format.

Each subdirectory should contain the FHIR resources in JSON format, as well as a text
file that captures the results from validating said resources using the
[FHIR Validator](http://wiki.hl7.org/index.php?title=Using_the_FHIR_Validator). Where
appropriate, the resources are also validated against the profiles available at:
- [cpg-plandefinition](../../StructureDefinition-cpg-plandefinition.html)
- [cpg-activitydefinition](../../StructureDefinition-cpg-activitydefinition.html)