---
title: "Worklog Week 10"
date: 2026-07-08
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---

### Objectives for Week 10:

* Complete the source code of the Football Field Booking web application following the Spring Boot architecture.
* Integrate social network login and handle security for configuration files (hide sensitive variables like Facebook/Google Client Keys, DB password).
* Package the entire source code into a single `.jar` file in preparation for deployment.

### Tasks to be implemented this week:
| Day | Task                                                                                                                                                                                        | Start Date | End Date   | Resources                                 |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | ----------------------------------------- |
| Mon | - **UI Development (View):** <br>&emsp; + Initialize the Spring Boot MVC project structure, integrate the Template Engine (Thymeleaf) and Bootstrap. <br>&emsp; + Build the standard Layout frame for the web (Header, Footer, Menu) and the homepage.                                     | 22/06/2026 | 22/06/2026 |                                           |
| Tue | - **Logic Processing (Controller & Model):** <br>&emsp; + Code core functions: Render the list of football fields on the UI, process the booking information form submitted by the user. <br>&emsp; + Map data from HTML Forms to Entities to save to the DB.                 | 23/06/2026 | 23/06/2026 |                                           |
| Wed | - **Security & Login Integration:** <br>&emsp; + Use Spring Security to integrate Google/Facebook login flows (OAuth2). <br>&emsp; + Separate the `application.properties` file, hide Client Keys, Secret Keys, and the DB password in environment variables.                 | 24/06/2026 | 24/06/2026 |                                           |
| Thu | - **AWS S3 Image Upload Integration:** <br>&emsp; + Code the function (Controller) to receive image files from the user's upload form (field images, avatars) and push them directly to the S3 Bucket using the AWS SDK. <br>&emsp; + Handle displaying S3 image links on the View.                     | 25/06/2026 | 25/06/2026 |                                           |
| Fri | - **Build & Package Project:** <br>&emsp; + Use Maven to build and bundle both Java code and static folders (HTML, CSS, JS) into a single `.jar` file. <br>&emsp; + Test run the `.jar` file locally via the command line to check for broken UI.      | 26/06/2026 | 26/06/2026 |                                           |


### Achievements in Week 10:

* **Application Completion:** Successfully built a seamless web system, from the user interface (Thymeleaf/Bootstrap) to the backend storage logic, all operating smoothly within a single Spring Boot project.
* **Source Code Security:** No more "hardcoding" sensitive information into the code. Learned how to configure the application to automatically read Facebook, Google, and Database Keys from the operating system's environment variables, keeping the source code safe when pushed to Github.
* **Successful Packaging:** Successfully packaged the entire web project into a single `.jar` file, with no missing UI file errors during independent execution.