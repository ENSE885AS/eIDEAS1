<p>
  <img align="left" src="./Documentaion/uofr_logo.jpg" alt="U of R logo" height="90px"/>
  <img align="right" src="./Documentaion/ehealth_logo.png" alt="eHealth logo" height="90px"/>
</p>

<br/><br/><br/><br/>

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Project Documentaion](#project-documentaion)
  - [1 INTRODUCTION](#1-introduction)
    - [1.1 Purpose](#11-purpose)
    - [1.2 Scope](#12-scope)
    - [1.3 Background](#13-background)
    - [1.4 Assumptions and Constraints](#14-assumptions-and-constraints)
      - [1.4.1 Constraints](#141-constraints)
    - [1.5 Document Overview](#15-document-overview)
  - [2 SYSTEM DESIGN](#2-system-design)
    - [2.1	Context Diagram](#21%09context-diagram)
    - [2.2	Data Flow Diagram](#22%09data-flow-diagram)
    - [2.3	Logical Data Model Diagram](#23%09logical-data-model-diagram)
  - [3 FUNCTIONAL REQUIREMENTS](#3-functional-requirements)
  - [4 OTHER REQUIREMENTS](#4-other-requirements)
    - [4.1 Interface Requirements](#41-interface-requirements)
      - [4.1.1 Hardware Interfaces](#411-hardware-interfaces)
      - [4.1.2 Software Interfaces](#412-software-interfaces)
    - [4.2	Data Conversion Requirements](#42%09data-conversion-requirements)
    - [4.3	Hardware/Software Requirements](#43%09hardwaresoftware-requirements)
    - [4.4	Operational Requirements](#44%09operational-requirements)
      - [4.4.1 Security and Privacy](#441-security-and-privacy)
      - [4.4.2 Audit Trail](#442-audit-trail)
      - [4.4.3 Reliability](#443-reliability)
      - [4.4.4 Recoverability](#444-recoverability)
      - [4.4.5 System Availability](#445-system-availability)
      - [4.4.6 General Performance](#446-general-performance)
      - [4.4.7 Data Retention](#447-data-retention)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


# Project Documentaion

## 1 INTRODUCTION

### 1.1 Purpose
The purpose of this document is to describe in details the system proposed to be implemented to address the eHealth need for a system which can gather the employees ideas, sort it, follow it up through the whole process, enable interaction between employees on departement level as well as on organization level.

### 1.2 Scope
This document describes the system functionality, describing the methodology applied in details, detailing the functional requirements, mentioning each interface, its links, menus,  pop up menus and icons.

### 1.3 Background
eHealth Saskatchewan (eHS) is a Treasury Board Crown within the province of Saskatchewan providing Information Technology (IT) support to Saskatchewan’s health sector. Through the vision “Empower Patients. Enable Care,” eHS has a goal and purpose to improve the quality of health care across the province for both patients and health care providers. In the organization’s ongoing effort to achieve this goal and purpose, eHS focuses on the sustainability of their services by fostering an internal culture of innovation. In operationalizing a culture of innovation, eHS employees are encouraged to individually and collaboratively trial new ideas and innovations through Plan, Do, Check, Act (PDCA) cycles with the goal of improving quality, cost, delivery, safety, and engagement within eHS.

A tool was developed called Challenge 100 which unfortunately didn’t succeed in fulfilling the goals it has been design for, where many deficiencies are reported which hundred reaching the ultimate goal.

An initiative has been taken to re-brand the tool to “eIDEAS” and re-envisioning the people, process, and technology interactions through a current and future state process mapping activity. Through this, the team assessed and redeveloped the design, delivery, and tracking methods to support eHealth's ongoing journey to transform the way they work. eHS wants the re-imagined eIDEAS tool to empower a sustainable internal culture of innovation, better enabling the sharing of ideas and the visibility of individual and collaborative work. The focus of eIDEAS is to begin with an idea at the local level (maximum of one work unit), visualizing the work from following key activities.

![alt text](https://raw.githubusercontent.com/semo94/eIDEAS1/master/Documentaion/Diagrams/aactivites.png)

### 1.4 Assumptions and Constraints
Assumptions are future situations beyond the control of the project, whose outcomes influence the success of a project. Examples of assumptions include: availability of a technical platform, legal changes and policy decisions.

#### 1.4.1 Constraints
Constraints are boundary conditions on how the system must be designed and constructed.  Examples include: legal requirements, technical standards, strategic decisions.
●	Constraints exist because of real business conditions.  For example, a delivery date is a constraint only if there are real business consequences that will happen as a result of not meeting the date.  If failing to have the subject application operational by the specified date places the organization in legal default, the date is a constraint.
●	Preferences are arbitrary.  For example, a date chosen arbitrarily is a preference.  Preferences, if included in the FRD, should be noted as such.

### 1.5 Document Overview
The document is divided into three main sections, an Introduction shedding light about the purpose and scope of this document, followed by a Methodology describing in a simple way how the tool will work and ends up with a Functional Requirements section listing the tool parts and pieces.

## 2 SYSTEM DESIGN

### 2.1	Context Diagram
![alt text](https://raw.githubusercontent.com/semo94/eIDEAS1/master/Documentaion/Diagrams/Context.png)

### 2.2	Data Flow Diagram
![alt text](https://raw.githubusercontent.com/semo94/eIDEAS1/master/Documentaion/Diagrams/DFD.png)

### 2.3	Logical Data Model Diagram
![alt text](https://raw.githubusercontent.com/semo94/eIDEAS1/master/Documentaion/Diagrams/LogicalDataModel.png)

## 3 FUNCTIONAL REQUIREMENTS

TBA

## 4 OTHER REQUIREMENTS
The web application (eIDEAS) shall be easy to use by all employees by decreasing the amount of scrolling the page for information and less number of clicks to achieve the desired output. The web application shall allow multiple users within the scope(team) to enter their ideas without affecting the performance of the application.

### 4.1 Interface Requirements
The user interface will accept input from mice and keyboard only.

#### 4.1.1 Hardware Interfaces
A web server application will be able to serve any authenticated user over the internet via URL.

#### 4.1.2 Software Interfaces
The web application will interface with employee accounts (Active directory list) for authentication. Also, the web application will interface with a database (mysql or NoSql). NoSql provides search like queries to look for some words under idea column.

### 4.2	Data Conversion Requirements
Data will be stored in database as plain text except large words can be replaced by one character.

### 4.3	Hardware/Software Requirements
The web application will require following hardware and software needs.
2.0 GHz CPU speed, 1 GB of RAM, 64 GB of HDD.
Microsoft Windows 10 or later, Mac OS.
Internet explorer 11, Mozilla Firefox, Google chrome or Safari internet browser.

### 4.4	Operational Requirements
The web application will ask for dialogue prompt when data is not saved before proceeding to another screen. When the user types in some predetermined values (e.g team name, staff name), the system will generate suggestion list to choose the rest of the value. Any disabled field will be provided with a description of the reason behind it.

#### 4.4.1 Security and Privacy
All authenticated user should protect their account information. User must log out when accessing the information at public computer. The data may be lost or not readable when exposed under computer attack or viruses. The private information can be disclosed to unauthenticated users when not logged out on public computers.

#### 4.4.2 Audit Trail
Activities will not be recorded in primary version, but can be implemented in later versions of the web application.

#### 4.4.3 Reliability
Any damage to the application from power shutdown can result in loss of unsaved data Any physical damage to the hardware will result in loss of data since last backup.

#### 4.4.4 Recoverability
In the event of unavailability of the application, the web application should be back up running within 24 hours of the first reported time.

#### 4.4.5 System Availability
The web application will be available to user 22 hours (4 AM to 2AM next day) of each day of the week. System will be out of service for the rest for backup.

#### 4.4.6 General Performance
The response time for a query or update can vary substantially depending upon the volume of the data. User will be provided with a waiting screen to a maximum of 10 seconds and then error will be presented.

#### 4.4.7 Data Retention
The user data will be retained in the database for one year before backing up permanently on a storage device.
