# Overview

This document provides the Software Requirements Specification (SRS) for the HomeGoods Inventory Management System, including detailed functional and non-functional requirements. It serves as a comprehensive guide for stakeholders, developers and testers to ensure the system is designed and implemented effectively.

# Software Requirements

This section defines the functional requirements, such as user authentication, inventory management and navigation, alongside non-functional requirements like performance, scalability, security and usability ensuring the system meets user and business needs effectively

## Functional Requirements

### User Authentication and Account Management
| ID  | Requirement |
| :--: | :----------: |
| FR1 | The system shall allow store managers to create an account by providing details such as first name, last name, email and password. |
| FR2 | The system shall restrict account creation if any of the required details (first name, last name, email or password) are missing. |
| FR3 | The system shall prevent account creation if the provided email address already exists. |
| FR4 | The system shall authenticate store managers during login using their credentials (email and password). |
| FR5 | The system shall restrict unauthorized users from accessing the application. |
| FR6 | The system shall allow registered store managers to reset their password by providing a valid email address. |

### Navigation and Page Flow
| ID  | Requirement |
| :--: | :----------: |
| FR7 | The system shall navigate to an account creation success page when an account is created successfully. |
| FR8 | The system shall navigate to the password reset page when the "Forgot Password" button is clicked. |
| FR9 | The system shall navigate to the "Item Categories" page after successful login. |
| FR10 | The system shall navigate to the "Add New Category" or "Add New Item" page when the respective button is clicked. |
| FR11 | The system shall navigate to the "Item Types" page when a category is selected. |
| FR12 | The system shall navigate to the "Item Details" page when a specific item is selected. |
| FR13 | The system shall navigate to the "Edit Item Details" page when the "Edit Item Details" button is clicked. |
| FR14 | The system shall navigate to the "Item Categories" page when the "Home" button is clicked. |

### Inventory Management
| ID  | Requirement |
| :--: | :----------: |
| FR15 | The system shall display a list of categories and allow store managers to add new categories. |
| FR16 | The system shall display a list of item types within categories and allow store managers to add new items. |
| FR17 | The system shall restrict adding a new category if the category name is not provided. |
| FR18 | The system shall restrict adding a new item if both the category name and item name are not provided. |
| FR19 | The system shall allow store managers to delete item categories. |
| FR20 | The system shall allow store managers to delete individual items from the inventory. |
| FR21 | The system shall display item details including category, name, price, stock, description, manufacturer, dimensions, weight, warranty and image when an item is clicked. |
| FR22 | The system shall allow store managers to edit item details including name, price, stock, description, manufacturer, dimensions, weight, warranty and image when the "Edit Item Details" button is clicked. |

### Buttons and Alert Messages
| ID  | Requirement |
| :--: | :----------: |
| FR23 | The system shall display an alert message saying, "Do you want to confirm saving this new category? Yes or No" before adding a new category when the "Save" button is clicked. |
| FR24 | The system shall display an alert message saying, "Do you want to confirm saving this new item? Yes or No" when the "Add new item" button is clicked on the "Add Item" page. |
| FR25 | The system shall display an alert message saying, "Do you want to confirm these changes? Yes or No" when the "Save" button is clicked on the "Edit Item Details" page. |
| FR26 | The system shall display an alert message saying, "Are you sure you want to delete category? Yes or No" when a category is selected for deletion. |
| FR27 | The system shall display an alert message saying, "Deleting this item is permanent. Proceed? Yes or No" when an item is selected for deletion. |
| FR28 | The system shall display an alert message saying, "Are you sure you want to log out? Yes or No" when the "Logout" button is clicked. |
| FR29 | The system shall provide a "Cancel" button on the "Add Item" and "Edit Item Details" pages, allowing the store manager to discard any unsaved changes. |
| FR30 | The system shall provide a "Back" button to return to the previous page. The button shall return to item categories when on the item types page, return to item types when on the item details page. |

### Search Functionality and Header Features
| ID  | Requirement |
| :--: | :----------: |
| FR31 | The system shall provide search functionality on the categories and item types pages to search by names. |
| FR32 | The system shall display the total inventory count of categories and the number of items within each category on the inventory page when clicking the "Count" button in the header. |
| FR33 | The system shall display the stock count of each item type on the inventory page. |
| FR34 | The system shall provide a Light/Dark theme button for switching between modes. |
| FR35 | The system shall provide a "Logout" button to allow store managers to log out of the application. |

## Non-Functional Requirements

### Performance
| ID  | Requirement |
| :--: | :----------: |
| NFR1 | The system shall provide a response time of 2-3 seconds for any search functionality under normal conditions. |
| NFR2 | The system shall respond to user actions (e.g. adding items, navigating pages) within 5 seconds during peak usage hours. |
| NFR3 | The system shall handle up to 500 concurrent users without significant performance degradation. |
| NFR4 | The system shall process inventory updates within 2 seconds ensuring seamless user experience during high activity. |
| NFR5 | The system shall process password reset requests within 3 seconds under normal conditions. |

### Scalability
| ID  | Requirement |
| :--: | :----------: |
| NFR6 | The system shall support the addition of unlimited categories and items without affecting performance. |
| NFR7 | The system shall allow seamless scaling of the backend infrastructure to support increased traffic as inventory grows. |
| NFR8 | The system shall be designed to handle future expansions such as new features or larger datasets without requiring downtime. |
| NFR9 | The application shall maintain responsiveness regardless of the increase in the number of users or inventory size. |
| NFR10 | The system shall have robust performance monitoring tools to track response times, resource utilization and error rates. |

### Security and Usability
| ID  | Requirement |
| :--: | :----------: |
| NFR11 | The system shall validate user credentials (email and password) from the backend during the login process. |
| NFR12 | The system shall restrict unauthorized users from accessing inventory data and management features. |
| NFR13 | The system's interface shall be intuitive and user-friendly, requiring minimal training for store managers. |
| NFR14 | The system shall provide clear and concise error messages with instructions for corrective action. |
| NFR15 | The application shall use consistent design patterns and layouts across all pages. |

### Compatibility
| ID  | Requirement |
| :--: | :----------: |
| NFR16 | The system shall be compatible with all major browsers including Chrome, Firefox, Safari and Edge. |
| NFR17 | The system shall be responsive ensuring usability across various devices (desktops, tablets and smartphones). |
| NFR18 | The system shall support cross-platform functionality working seamlessly on Windows, Mac, Linux, Android and iOS. |
| NFR19 | The application shall be compatible with various screen sizes. |
| NFR20 | The system shall ensure consistent display and functionality across all supported devices and browsers, maintaining uniformity in layout, features and content. |

### Availability and Data Consistency
| ID  | Requirement |
| :--: | :----------: |
| NFR21 | The system shall maintain an uptime of 99.9%, ensuring store managers can access the platform with minimal downtime. |
| NFR22 | The system shall ensure that all changes made to inventory are immediately reflected in the database and UI. |
| NFR23 | The system shall synchronize data in real-time to avoid inconsistencies and delays. |
| NFR24 | The system shall detect and resolve data conflicts caused by simultaneous updates, prioritizing the latest valid input while alerting affected users. |
| NFR25 | The system shall ensure seamless communication between the front-end and back-end components. |

# Change Management Plan
This section describes the strategy for handling modifications during system implementation. It covers techniques for integration, training, problem solving and continuing assistance to guarantee a smooth transition and outstanding results.

## Training Plan

**Objective:**  
Ensure all store managers understand and can effectively use the system to manage inventory.

**Training Methods:**  
- **Interactive Workshops:** Conduct initial hands-on workshops where managers can interact with the system.  
- **User Guide:** Provide a detailed user manual, including step-by-step instructions and screenshots.  
- **Video Tutorials:** Create short, targeted videos demonstrating core functionalities like login, adding/editing items and using search.  

**Topics Covered:**  
- User Authentication and Session Management  
- Navigating the Dashboard and Categories  
- Managing Items (Add, Edit, Delete)  
- Using Search and Filters  

## Integration with Existing Ecosystem / Software

**Objective:**  
Ensure the seamless integration of the Home Goods Inventory Management System into the customer’s existing software and processes.

**Integration Steps:**  
1. **Environment Compatibility Testing:**  
   - **Cross-Browser Testing:** The system will be tested on major browsers, including Chrome, Firefox, Safari and Edge to ensure consistent performance.  
   - **Device Compatibility:** The system will be responsive and tested on various devices (desktops, tablets and smartphones) to ensure usability.  
   - **Cross-Platform Support:** As a web-based application, the system will run smoothly on Windows, macOS, and Linux without additional configuration.  

2. **Data Synchronization:**  
   - **Firebase Backend:** Real-time data synchronization between the React front-end and Firebase backend ensures consistent and up-to-date inventory data.  
   - **Future Integration Potential:** While the system currently operates independently, it can be extended to sync with existing inventory databases through custom development if required.  

3. **Role-Based Access Control (RBAC):**  
   - **Firebase Authentication:** The system uses Firebase Authentication to manage user roles and permissions.  
   - **Role Alignment:** User roles within the application can be mapped to existing organizational roles, ensuring appropriate access control.  

4. **API Integration:**  
   - **Current Scope:** The system provides a standalone solution using Firebase. Custom APIs can be developed in the future to integrate with ERP, accounting, or other business tools.  
   - **Data Flow Testing:** Once integrated, thorough testing will be conducted to ensure accurate data exchange between systems.  


## Issue Resolution and Support Plan

**Objective:**  
Ensure prompt identification, reporting, and resolution of any discovered issues to maintain smooth system operations.

**Support Channels:**  
- **Dedicated Support Email:** Provide a dedicated support email where store managers can report issues or request assistance.  

**Issue Resolution Process:**  
- **Continuous Monitoring:** Utilize Firebase logs to monitor system health and proactively detect potential issues before they impact users.  
- **Software Updates:** Regularly release updates to fix bugs, enhance performance, and introduce new features. Notify users in advance about upcoming updates and provide documentation for any significant changes.  

# Traceability links
This section maps requirements to artifacts, ensuring they are addressed throughout the project.

## Use Case Diagram Traceability

| Artifact ID |      Artifact Name       | Requirement ID         |
| :---------: | :----------------------: | :---------------------: |
| UseCase1    | [Create Account](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR1, FR2, FR3, NFR14 |
| UseCase2    | [Login](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR4, FR5, NFR11 |
| UseCase3    | [Reset Password](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR6, NFR5 |
| UseCase4    | [System Navigation](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR7 - FR14, FR29, FR30, NFR2 |
| UseCase5    | [Inventory Management](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR15 - FR22, NFR2, NFR4 |
| UseCase5_1    | [Alert Messages](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR23 - FR28 |
| UseCase6    | [Search Functionality](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR31, NFR1 |
| UseCase7    | [Stock Count](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR32, FR33 |
| UseCase8    | [Dark/Light Theme](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR34, NFR13 |
| UseCase9   | [Logout](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg) | FR35 |

## Class Diagram Traceability

| Artifact Name | Requirement ID |
| :------------: | :------------: |
| [Login](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Class1.jpg) | FR4, FR5, FR6, FR8, FR35, NFR5, NFR11 |
| [Create Account](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Class1.jpg) | FR1, FR2, FR3, FR7, NFR14 |
| [Category](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Class1.jpg) | FR9, FR10, FR14, FR15, FR17, FR19, FR31, FR32, FR33, FR34, NFR1, NFR4 |
| [AlertMessage](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Class1.jpg) | FR23-FR28 |
| [ItemTypes](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Class1.jpg) | FR11, FR16, FR20, FR30, NFR1 |
| [AddItem](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Class1.jpg) | FR10, FR16, FR18, FR29, NFR4 |
| [ItemDetails](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Class1.jpg) | FR12, FR21, FR30 |
| [EditItemDetails](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Class1.jpg) | FR13, FR22, FR29, NFR4 |

## Activity Diagram Traceability

| Artifact ID | Artifact Name | Requirement ID |
| :---------: | :---------------------------: | :------------: |
| Activity State1 | [Create Account](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR1, FR2, FR3, FR7, NFR14 |
| Activity State2 | [Login](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR4, NFR11 |
| Decision Node1 | [Is Login Success? No](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR5 |
| Decision Node2 | [Forgot Password? Yes](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR6, FR8, NFR5 |
| Activity State3 | [Access Inventory Dashboard](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR9, FR14, NFR2 |
| Decision Node3 | [Toggle Dark Mode? Yes](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR34, NFR13 |
| Decision Node4 | [View Stock Count? Yes](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR32, FR33 |
| Activity State4 | [View Categories](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR9, FR15 |
| Decision Node5 | [Add/Delete Category? Yes](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR10, FR15, FR17, FR19, FR23, FR26, NFR4 |
| Activity State5 | [View Item Types](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR11, FR16 |
| Decision Node6 | [Add/Delete ItemType? Yes](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR10, FR16, FR18, FR20, FR24, FR27, FR29, NFR4 |
| Activity State6 | [View Item Details](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR12, FR21 |
| Decision Node7 | [Edit Item Details](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR13, FR22, FR25, FR29, NFR4 |
| Activity State7 | [Logout](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg) | FR28, FR25 |

# Software Artifacts
This section contains all diagrams related to Home Goods Inventory Management.  

[Usecase Diagram](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Usecase.jpg)  
[Class Diagram](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Class1.jpg)  
[Activity Diagram](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Final_Activity.jpg)  
[Class Responsibility Collaborator Cards](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Class_Responsibility_Collaborator_cards.pdf)  
[Class Specification](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Class_Specification.pdf)  
[Object Diagram](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Object_Diagram.pdf)  
[Sequence Diagram](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Sequence_Diagram.pdf) 
[State machine Diagram](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/State_machine_Diagram.pdf)  
[Windows Navigation Diagram](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/artifacts/Windows_Navigation_Diagram.pdf)  

