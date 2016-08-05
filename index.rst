:tocdepth: 1

.. sectnum::

.. _scope:

Scope of Document
=================

This document describes the operational concepts for the emerging LSST DPP group which will operate
the system that will be delivered by the LSST construction project. This system will be incrementally
stood up and operated by the construction project as part of validation and verification activities
within the construction project.

The concept of operations covers approximately 40 distinct services, The operations concepts
are initially developed in Google docs. It is the vision to  migrate these documents to
ReStructuredText as they mature.  Therefore, initially, we will provide pointers to documents as
the level of drafting within the working group becomes suitable to expose the documents to the
LSST construction project.

.. _overview:

Level 1 Services
================

Main Camera Data Prompt Processing Service
------------------------------------------

The prompt processing of raw data acquired from the main LSST camera
by the DM system. The prompt processing service is primarily presented
to the the Observing Operations as an OCS-controllable device.

`Main Camera Data Prompt Processing Service  <https://docs.google.com/a/illinois.edu/document/d/1hv0_ZhkPXt2xCUcMU5J94SjnEr2ZH8JK43PsqJJn_6k/edit?usp=sharing>`_

This figure illustrates a logical conception of the service.

`Logical Conception of the Main Camera Data Prompt Processing Service  <https://drive.google.com/open?id=0B4OAryR7BjSiU1BfVndSNzRRQ0U>`_



Main Camera Data Archiving Service
----------------------------------

The main camera data archive service is presented to Observing
Operations as a OCS-controllable device.  The service constructs raw
data files from exposures in the camera data system, and meta-data
residing in OCS.  The files so constructed are ingested into the data
backbone.

`Main Camera Data Archiving Service <https://drive.google.com/open?id=1-2jV-VovfVpJO62C2PmVXSUWaXB0gFfZ4pgp6I1d3k0>`_

This figure illustrates a logical conception of the service.

`Logical Conception of the Main Camera Archiving Service  <https://docs.google.com/document/d/1ZolFLDtRbOxKhC6CMLXMRmy3zvQbiyE2kYkc_odSR6c/edit?usp=sharing>`_


Alert Distribution Service
--------------------------

The Alert Distribution service a service which connects programs
generating alert information to event brokers.

`Alert Distribution Service <https://docs.google.com/document/d/1z_j-b41BHwpfXoeRAwTVA76Uzp8Xodx3vOLFDAnVnrY/edit?usp=sharing>`_

A figure that illistrates a repesentative logical structure is here:

`Alert Distribution Figure <https://drive.google.com/open?id=0B4OAryR7BjSiWHEtYlFpX3lQM2M>`_

Auxiliary Telescope  Data Processing and Archiving
--------------------------------------------------

Ingest data from spectrophotometer into Data Backbone.
TBD whether or not processing is needed.

** Pre-phase 1**

Telemetry Gateway
-----------------

Capabilities for system information sent from the DM system to the OCS system.
This service covers the transmission of all telemetry into the OCS system.

** In phase 2 discussion which resuled in need for clarification

Observatory Operations Data Services
------------------------------------
Provide access to designated datasets from the LSST science data archive as needed by observatory operations to the stipulated service levels

** In phase 2 discussion which resuled in need for clarification


OCS-Driven Batch Services
-------------------------
Service to expose the  batch production service as an OCS command-able device at service levels with observatory needs.

** Need being discussed.

EFD Replication
---------------
Service to acquire a copy of the Event and Facilities database information at NCSA


Commissioning Cluster Services
------------------------------

Provide a software production environment deployed upon the
commissioning cluster which consists of TBD features, supporting TBD
computations of TBD capacity

Summit Data Services
--------------------

Summit data services refer to presistent data storage at the summit
site, Most likely to satisfy use cases related to sustaining
operations should the fiber be cut, or for any other need that would
emerge.

This Need is under discussion. 


Offline L1 Processing
---------------------

Offline Level 1 processing is processing that occurs in the a batch context, instead of the context of the Prompt Processing under OCS control.

The concepts for this process are presented in the "Level 1 Producition Services" section of this document prepared for the LOPT/TOWG

`<https://docs.google.com/document/d/1KFwL38iIKbvDhhcbPcwjWr-CDg9cPvZuq0PFzSBmbPc/edit>`_


First Order Scientific Quality Assurance
----------------------------------------

First Order Scientific Quality for Level one is described in the "Level 1 Production Services" section of this document prepared for the LOPT/TOWG.
The additional quality assessment concepts presented in the section "Level 2 production services" in the level system also apply.

`<https://docs.google.com/document/d/1KFwL38iIKbvDhhcbPcwjWr-CDg9cPvZuq0PFzSBmbPc/edit>`_


Level 1 Complete Test Environment
---------------------------------

Level 1 Complete Test Environment a capablity need to for testing Level 1 Service Changes.

The concepts for this process are presented in the "Level 1 Production Services" section of this document prepared for the LOPT/TOWG

`<https://docs.google.com/document/d/1KFwL38iIKbvDhhcbPcwjWr-CDg9cPvZuq0PFzSBmbPc/edit>`_


Level 2 Services
================

This document describes the operational concept for batch production operations. Batch operations consists of executing large or small processing campaigns that use released software configured into pipelines to produce data products, such as calibrations and DRP products.

The basci concept of batch produciotn apply to these level 2 servince elements:
These concepts apply to these Batch oriented servicesL

Annual Release Processing: Processing of payloads of tested workflows
at NCSA and satellite sites through and including ingest of release
products into file stores, relational databases, and the Data
Backbone, including system quality assurance.

Calibration Processing: processing of payload tested workflows at NCSA
and satellite sites through and including ingest of release products
into file stores, relational databases, and the Data Backbone,
including initial quality assurance. Calibration production occurs at
various cadences from potentially daily to annual, depending on the
calibration data product.

Special Programs and Miscellaneous Processing: Includes processing
other than specifically enumerated.

Batch framework upgrade testing: Test suite run after system upgrades
and other  changes to verify operations.

Payload Testing Verification and validation: of workflows from the
continuous build system on the production hardware located of NCSA and
satellite sites.


`Batch Production Services <https://docs.google.com/document/d/1MVe0qdHt5RNTN8KkIxWzd24nNbxA5ZWghajoak3i0HU/edit?usp=sharing>`_

The additional concepts for this process are presented in the "Level 2
Production Services" section of this document prepared for the
LOPT/TOWG

`<https://docs.google.com/document/d/1KFwL38iIKbvDhhcbPcwjWr-CDg9cPvZuq0PFzSBmbPc/edit>`_


Data Backbone Services
======================

The presentation of this concept of operations is expected by August 31, 2016

Data Access Hosting Services
============================

The presentation of this concept of operations is expected by August 31, 2016


Development Support Services
============================

The presentation of this concept of operations is expected in a future planning period.

Miscellaneous Services
======================

The presentation of this concept of operations is expected in a future planning period.



Authentication and Authorization
--------------------------------

The Authentication and Authorization concept of operations has been prepared and
is in the submission process in the LSST systems change control process.


ITC Provisioning and Management
===============================

The presentation of this concept of operations is expected in a future planning period.


Chilean ITC
-----------
Provide equipment for Chilean DAC, Base Center, and the DPPD designated support for the Observatory Operation Support Services. Provide for local administration in Chile.

NCSA ITC
--------
Provide equipment for US DAC, Archive Center, and the DPPD designated support for the Observatory Operation Support Services. Provide for local administration at NCSA.


Wide Area Network Services
--------------------------
Provide connectivity between border routers of La Serena, NCSA, CC-IN2P3 and other designated sites.

Detailed conops will be in a future planning period.


Service Management Processes
============================

Broadly oversee and evolve services described herein. “What are we doing, what are we planning on doing, and how well are we doing it.”

Detailed conops will be in a future planning period.


Service Design
--------------
Building a servince catalog and arranging for changes to the service offering, including internal supporting services.

Detailed conops will be in a future planning period.


Service Transition
------------------
Service transtion process provide for specifiing neeed changess, and assessing the quality of proposed changes,
controlling the order and timing of inserting changes  into the system.

Detailed conops will be in a future planning period.

Change management:
+++++++++++++++++
An authorized stream of changes to be requested, and for the insertion
of changes into the reliable production system, and the assessent of the success of these changes 

Detailed conops will be in a future planning period.


Release management:
++++++++++++++++++

Release management interacts with project producing a specfic change, to ensure that
a complete change is presented to change management for approval into the live system.
Examples areas that are typically a concern -- documention, security concerns.

Configuration Management: provides an accurate model of the components in the live
system sufficent to understand changes, and support operations.

Detailed conops will be in a future planning period.

Service Delivery
----------------
Service Delivery is a set of processes needed to operates the current system.  The servince delivery
processes must statisfy the detailed service delivery concepts presented elsewhere in this concept of
operations doumentation ensemble. 

Request Response
++++++++++++++++
Detailed conops will be in a future planning period.

Incident response
+++++++++++++++++

Incident response concept processes are documented in in material developened for the
LOPT/TOWG working groups. 

The concepts for this process are presented in the "Incident Response" section of this document prepared for the LOPT/TOWG

`<https://docs.google.com/document/d/1KFwL38iIKbvDhhcbPcwjWr-CDg9cPvZuq0PFzSBmbPc/edit>`_

Problem Management
++++++++++++++++++

Problem management processing are documented in material develope for the LOPT/TOWG working groups.

The concepts for this process are presented in the "Problem Management" section of this document prepared for the LOPT/TOWG

`<https://docs.google.com/document/d/1KFwL38iIKbvDhhcbPcwjWr-CDg9cPvZuq0PFzSBmbPc/edit>`_

.. _changerecord:

Change Record
=============


+-------------+------------+----------------------------------+--------------+
| **Version** | **Date**   | **Description**                  | **Owner**    |
+=============+============+==================================+==============+
| 1.0         | 5/22/2013  | Initial Version                  | Kian-Tat Lim |
+-------------+------------+----------------------------------+--------------+
| 1.1         | 10/9/2013  | Updates resulting from Process   | Kian-Tat Lim |
|             |            | Control and Data Products        |              |
|             |            | Reviews                          |              |
+-------------+------------+----------------------------------+--------------+
| 1.2         | 10/10/2013 | TCT approved                     | R Allsman    |
+-------------+------------+----------------------------------+--------------+
| 2.0         | 08/05/2016 | Beginning to render working group| D Petravick  |
|             |            | schema as more complete view of  |              |
|             |            | operational need as a basis for  |              |
|             |            | planning.                        |              |
+-------------+------------+----------------------------------+--------------+
