Waste Collection System

Overview

The Waste Collection System is a Java-based application that facilitates waste collection management. The system incorporates Object-Oriented Programming principles, the MVC (Model-View-Controller) architecture, and the Composite pattern to ensure modularity, scalability, and maintainability.

Components

1. Models
TruckDriverModel

Manages data related to truck drivers.
Stores information about registered truck drivers.
WeeklySchedule

Represents the data structure for a weekly schedule.
Stores information about the week number, driver ID, and scheduled routes.

2. Views
TruckDriverView

Handles the presentation of truck driver-related information to the user.
Displays a list of truck drivers with their IDs and usernames.
WeeklyScheduleView

Handles the presentation of weekly schedule information to the user.
Displays the weekly schedule for a driver, including the week number and scheduled routes for each day.

3. Controllers
TruckDriverController

Acts as an intermediary between the TruckDriverModel and TruckDriverView.
Manages user input for truck driver registration and displays the list of registered truck drivers.
WeeklyScheduleController

Manages the flow of data between the WeeklySchedule model and WeeklyScheduleView.
Generates and retrieves weekly schedules for truck drivers.
CollectionCentreController

Manages the process of creating a waste collection report at a collection centre.
Gathers user input for driver ID, route number, and total weight.
Creates a WasteData object and a WasteCollectionReport composite.
Displays the waste collection report to the user.

4. Composite Pattern
WasteData

Represents the leaf component in the composite pattern.
Encapsulates individual data (Driver ID, Route Number, Total Weight).
WasteCollectionReport

Represents the composite structure in the composite pattern.
Composes multiple components, including information about the collection centre, date and time, and waste data.
Implements the display method to present the composite structure.
Non-functional Considerations

The system addresses non-functional requirements through the following tactics:

Performance:
Efficient data structures and algorithms for optimal task execution.
Caching mechanisms to reduce redundant computations.
Exploration of parallelism for concurrent task processing.
Reliability:
Robust exception handling to gracefully handle unexpected errors.
Logging and monitoring features for error tracking and performance metrics.
Redundancy in critical components to provide backup solutions.
Maintainability:
Modular design principles for loose coupling of components.
Comprehensive code documentation to aid understanding and modifications.
Robust automated testing to prevent unintended side effects.
Usability:
User-centric design for an intuitive and positive user experience.
Accessibility considerations for users with diverse needs.
User feedback mechanisms for continuous improvement.
Security:
Data encryption for secure transmission and storage.
Strong authentication and authorization mechanisms.
Regular security audits to identify and address potential vulnerabilities.
Usage

To run the Waste Collection System, execute the WasteCollectionSystem class. Follow the prompts to interact with different components of the system, such as truck driver registration, weekly schedule generation, and waste collection reporting.

Contributors

Imtiyaz 
Feel free to contribute to the project by submitting pull requests or reporting issues.
