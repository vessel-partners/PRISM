PRISM Read.me

# About

The award-winning PRISM (**P**ROMIS **R**eporting and **I**nsight **S**ystem from **M**innesota) is an application that enhances the quality of clinical discussion between healthcare providers and patients by allowing for PRO collection and continued patient engagement outside of the clinical setting.

PRISM was developed by a multi-disciplinary team including [Perk Health](https://www.perkmotivation.com), a digital health design and development company, and faculty, staff, alumni and physicians from the [University of Minnesota](https://healthinformatics.umn.edu/news/prism) (Carlson School/MILI, CTSI/Institute for Health Informatics, School of Medicine), along with Fairview/HealthEast's [Kidney Stone Institute](https://www.fairview.org/services/kidney-stone-institute), and consultant Elisha Friesema.

> “This app is an innovative tool that will advance value- and person-centered care by ensuring that information generated by patients is a major driver in their care,” said AHRQ Director Gopal Khanna, MBA. “PRISM will help overcome challenges in collecting and integrating standardized PRO data into health information technology systems.”

The code posted here represents the first version of PRISM that was implemented at MedStar Health as a result of winning the grand prize in AHRQ's Step-Up App challenge. This app is continually being enhanced in functionality and interoperability by the PRISM Team. 

# Devloper Links

The PRISM App consists of a Frontend Hybrid mobile app built using Angular and Ionic and Backend built AWS Lambda and other services. To get up and running with the project, please fully install the Backend before moving on to Frontend. The Frontend configuration depends on the backend.

Important Files:
- [Frontend Readme](frontend/README.md)
- [Backend Readme](backend/README.md)
- [Install Backend Dependencies](backend/docs/install-dependencies.md)
- [Run backend for development](backend/docs/run-for-development.md)
- [Deploy backend to Production](backend/docs/how-to-deploy.md)

For technical and design questions please contact help@perkhealth.me

# Features

**Patient-Facing App for Patient Reported Outcome (PRO) Collection** 

PRISM provides a simple and highly usable way for patients to complete Patient Reported Outcome (PRO) surveys from a mobile app or mobile web interface including computer adaptive PROMIS measures. 

**Patient Engagement and Education** 

The app was designed to encourage patient participation through visualizations of PRO scores, population comparisons, and trends over time. The app also has a placeholder section for personalized educational materials. 

**Multi-Platform**

PRISM includes iOS and Android apps along with mobile web interfaces through a hybrid mobile architecture. 

**FHIR Compliant API**

PRISM uses FHIR and Smart on FHIR for interoperability and integration with an external assessment center (EAC) and the Hub.

**Smart on FHIR User Management** 

PRISM supports Smart on FHIR for seamless integration with a user management provider including single sign on and secure authorization and authentication. 

# Architecture

Diagram

- prism, eac, hub, provider app

PRISM was built leveraging Amazon's AWS serverless products as a way to demonstrate the ability to use modern development practices in a project that mandated adherence to healthcare standards and regulations including HIPPA and FHIR. While this presented some challenges, the team feels this allowed us to speed the initial prototype development considerably, simplified several stages of early development, and provides a useful case study. 

Due to often sparse EHR support for FHIR, PRISM was built in concert with Perk Health's Hub product to provide a means for patient account creation, invitation, user authorization and authentication, FHIR data storage, and APIs for the in-EHRs provider apps to pull and view patient data.      

To administer Computer Adaptive PROMIS assessments PRISM integrates with an external assessment center created by Northwestern University. 

# Development

PRISM underwent extensive usability testing with patients at Health East's Kidney Stone Institute where the ability for patients to complete physical function and other PROMIS measures, interact with score trending, peer group comparisons, and relevant recommendations for follow-up actions and education materials aimed to further engage patients in their care were shown to be highly usable. 

Patient Reported Outcomes captured by the app are integrated into the EHR and available for providers to use, in real-time, during their clinical care and shared decision making with the patient. This integration is provided via Perk Health's Healthcare Hub which supplies FHIR compliant data storage, user sign in/on, authentication, authorization, and APIs for MedStar's provider facing app to display results within multiple EHRs. 

[https://www.ahrq.gov/news/newsroom/press-releases/stepup-app-phase2-winners.html](https://www.ahrq.gov/news/newsroom/press-releases/stepup-app-phase2-winners.html)

# License

Link: Apache 2.0 license
