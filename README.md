# SafeBond

**Objective:**

SafeBond aims to develop a comprehensive platform enabling individuals in workplaces or healthcare facilities to maintain real-time communication with their families via chat and video functionalities. The platform will also incorporate health monitoring features, including tracking vital signs such as heart rates. In the event of a health emergency, such as a significant drop in vital signs, the application will automatically call designated family members with an automated message, informing them of the situation and the individual’s location to enable swift assistance.

---

## SRS
(Software Requirements Specification) for SafeBond

### 1. Introduction

1.1 **Purpose**

The purpose of this SRS document is to describe the requirements and specifications for the SafeBond platform. SafeBond will provide real-time communication between individuals in workplaces or healthcare facilities and their families, health monitoring, location tracking, and emergency alert features to ensure the safety and well-being of users.

1.2 **Scope**

SafeBond will be a comprehensive platform that includes the following key features:

-  Chat and video communication between users and family members.
-  Continuous health monitoring, focusing on vital signs such as heart rate.
-  Location tracking to monitor the user’s movements.
-  An automated emergency alert system that will call designated family members with an automated message in case of health emergencies and provide the individual's location.

  
1.3 **Definitions, Acronyms, and Abbreviations**

SafeBond: The platform name.
SRS: Software Requirements Specification.
UI: User Interface.
API: Application Programming Interface.


1.4 **References**

No external references have been used in the creation of this SRS at this stage.
But we will add in the future:
Technical articles on similar systems or technologies (e.g., location tracking, health monitoring APIs).
Programming standards you're following (e.g., design patterns, coding guidelines).
Framework or API documentation you’ll use (e.g., .NET Core, chat/video APIs).
Any books or tutorials relevant to the project.

1.5 **Overview**

This document outlines the functional and non-functional requirements of the SafeBond platform, detailing the system features, external interface requirements, and constraints to be considered during the system's development and deployment.

---

### 2. Overall Description

**2.1 Product Perspective**

SafeBond is developed as a standalone system that operates independently to provide seamless communication, health monitoring, and emergency alert functionalities. While the platform is self-sufficient in delivering its core features, it integrates with a few external services to enhance its overall capabilities:

- Mobile Platforms: SafeBond is primarily designed for Android and iOS mobile devices. The mobile app serves as the primary interface for users to communicate, monitor health, and manage emergencies.
- Desktop Platforms: A desktop version of the SafeBond app will be available for Windows, Linux, and Mac OS, providing extended accessibility to users across multiple devices. The desktop version offers similar features as the mobile app.
- Web Access: While the web interface has limited functionality, it will allow users to briefly access their accounts for signing in/out and generate a barcode for easy mobile app installation. It acts as a supporting interface rather than a fully functional platform.
- Health Monitoring APIs: SafeBond integrates with external APIs to track users' vital signs such as heart rate, enabling real-time health monitoring. These APIs connect with wearable devices or other healthcare systems, ensuring accurate and continuous data flow.
- Location Services: The system relies on GPS-based location services to track users’ movements. This information is critical in emergencies, helping family members, friends, and healthcare staff locate users swiftly and accurately.
- Emergency Response: SafeBond links with nearby hospitals and emergency services based on the user's location. In health crises, the platform notifies the nearest hospitals, providing essential information like the user's location and health status to ensure timely medical intervention.

By leveraging mobile, desktop, and web platforms, along with health monitoring and location tracking services, SafeBond creates a comprehensive, all-in-one solution to ensure the safety and well-being of its users.



**2.2 Product Features**

SafeBond provides a range of essential features, ensuring seamless communication, health monitoring, and emergency management for users. The key features include:

- Real-time Communication: Secure chat and video communication between users and their families, friends, and healthcare staff.
- Health Monitoring: Continuous tracking of vital signs such as heart rate, enabling timely health monitoring.
- Emergency Alerts: In the event of a health emergency, SafeBond automatically triggers calls to family members with an automated message, providing the individual’s health status and location.
- Location Tracking: Monitors the user’s movement and provides real-time location information to designated contacts.
- Finding Nearest People: Identifies the nearest friends or family members based on location to ensure quick help during emergencies.
- Linked to Nearest Hospitals: During emergencies, SafeBond will also notify and provide location information to the nearest hospitals, enabling faster medical response.


**2.3 User Classes and Characteristics**

- Family Members: These users receive emergency alerts and communicate with the patient via chat or video.
- Patients: Individuals using SafeBond to stay connected with family and healthcare staff. Their health data and location are monitored.
- Nearest Friends: Friends in the immediate vicinity who can respond quickly to emergencies or assist the patient.
- Healthcare Staff: Medical personnel monitoring the patient’s health and responding to emergencies.
- Nearest Hospitals: Emergency centers or hospitals that are notified during critical health events for quick response.


**2.4 Operating Environment**

1. Mobile App: SafeBond will be primarily available as a mobile application for Android and iOS.
2. Web Access: A web-based interface will provide limited functionality, such as signing in/out and generating a barcode for mobile app installation.
3. Desktop App: A cross-platform desktop application will be developed, compatible with Windows, Linux, and Mac OS.


**2.5 Design and Implementation Constraints**

1. The need for integration with specific APIs (e.g., health monitoring APIs)
2. Legal requirements (e.g., data privacy and healthcare regulations like HIPAA)


**2.6 Assumptions and Dependencies**

1. Assumed availability of internet connectivity for real-time communication.
2. Dependency on third-party APIs for health tracking.



