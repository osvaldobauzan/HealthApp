## Overview


I created two different programs, both written in Python, to address distinct issues. Both projects connect to or utilize a cloud-based database: Firestore.

Health App:
The Health App stands as the inaugural endeavor, stemming from the imperative need to meticulously document and manage sleep patterns. This innovative Python-based program seamlessly captures the precise hours of sleep on designated days, creating a comprehensive sleep log. Once recorded, users enjoy the convenience of effortlessly reviewing, modifying, and even deleting these sleep entries. This app not only serves as a personal sleep tracker but also lays the foundation for fostering healthy sleep habits by providing insightful data.

Track Pack App:
Introducing the Track Pack App, a dynamic Python solution to the perennial woe of parcel tracking from myriad providers such as Amazon and various mail services. This sophisticated program empowers users to effortlessly register incoming packages, offering a streamlined interface to monitor their transit progress. Whether it's awaiting delivery or already in transit, users can seamlessly check the status of their packages, modifying pertinent details as needed. The Track Pack App revolutionizes the package tracking experience by centralizing information and simplifying the management of shipments, ultimately ensuring that users stay in control of their deliveries.

[Software Demo Video]([https://youtu.be/uH2P9PjFGdw])


# Cloud Database Description:

The chosen cloud database for these projects is Firestore. Firestore is a NoSQL, document-oriented database provided by Google Cloud Platform, offering real-time synchronization and seamless scalability. It is designed to facilitate the storage and retrieval of data in a flexible and efficient manner, making it an ideal choice for applications that demand dynamic, real-time updates and collaboration.

Firestore operates on a collection-document model, where data is organized into collections, and each collection contains individual documents. This schema-less approach allows for versatile data modeling and supports the storage of complex, nested structures, making it well-suited for a wide range of applications.

# Database Structure:

1. Health App:
   - Collection: `SleepLogs`
     - Document: Each document corresponds to a specific day's sleep log.
       - Fields:
         - `Date`: The date of the sleep entry.
         - `HoursSlept`: The recorded hours of sleep for that day.
         - *(Additional fields as needed, depending on the desired features.)*

2. Track Pack App:
   - Collection: `PackageTracking`
     - Document: Each document represents a registered package.
       - Fields:
         - `TrackingNumber`: The unique identifier for the package.
         - `Provider`: The service provider handling the package (Amazon, Mail service, etc.).
         - `Status`: The current status of the package (e.g., In Transit, Delivered).
         - `Details`: Additional information about the package.
         - *(Additional fields for tracking history, delivery address, etc.)*

This structured approach allows for efficient retrieval and manipulation of data, ensuring that each app can seamlessly interact with Firestore to provide users with a smooth and responsive experience while maintaining data integrity and security.

## Development Environment

The software for both the Health App and Track Pack App was crafted using a set of powerful tools to streamline the development process. Here's a breakdown of the tools employed:

Integrated Development Environment (IDE):

IDE Used: PyCharm
Description: PyCharm is a robust integrated development environment for Python, providing intelligent coding assistance, a graphical debugger, and extensive support for web development. Its user-friendly interface and powerful features enhance productivity and facilitate efficient code navigation.
Version Control:

Version Control System: Git
Repository Hosting: GitHub
Description: Git, a distributed version control system, was utilized for code versioning and collaboration. GitHub served as the remote repository, enabling seamless collaboration, code review, and version tracking.
Cloud Database Service:

Database Service: Firestore (Google Cloud Platform)
Description: Firestore, a NoSQL cloud database, was chosen for its scalability, real-time synchronization, and seamless integration with Python. It provides a robust and flexible foundation for storing and retrieving data in a cloud environment.
Programming Language:

Language Used: Python
Description: Python, a versatile and user-friendly programming language, served as the core language for both projects. Its simplicity, readability, and extensive library support make it an ideal choice for rapid development and diverse application scenarios.
Libraries:

Firestore Library: google-cloud-firestore

Description: This Python library facilitates the interaction with Firestore, allowing seamless integration of the cloud database into the applications. It provides functions for data manipulation, retrieval, and management.
Additional Libraries: (Specific libraries used for features, such as date handling, HTTP requests, etc.)

(Include any relevant libraries depending on the specific functionalities implemented in each app.)
By leveraging these tools, the development process was not only efficient but also facilitated collaboration, version control, and integration with cloud services, ensuring the successful creation of the Health App and Track Pack App.

## Useful Websites


- [FireStore Tutorial](https://firebase.google.com/docs/firestore?hl=es)
- [FireStore Docs](https://cloud.google.com/firestore/docs)
- [CRUD Creation](https://cosasdedevs.com/posts/como-crear-un-crud-en-python-parte-1-estructura-y-clase/)

## Future Work

- Connect to Amazon API for packs info
- Make them more user - friendly
- Host them in the web
