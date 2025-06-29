# Requirement Analysis in Software Development.





## What is Requirement Analysis?

### Overview of Requirement Analysis

Requirement Analysis bridges the gap between the initial concept of a project and its technical implementation. It focuses on understanding what the system should do (functional requirements) and how it should perform (non-functional requirements, such as performance, security, or scalability). The process typically includes the following key activities:

**Requirement Gathering:**

This initial step involves collecting high-level information about the system's purpose and stakeholder needs. Techniques include stakeholder interviews, questionnaires, observation, and reviewing existing documentation.

Example: For a hotel booking system, gathering might involve identifying that users need to search for rooms, make reservations, and process payments.

**Requirement Elicitation:**

Elicitation is a more focused and interactive process to extract detailed requirements from stakeholders. It uses techniques like workshops, focus groups, brainstorming sessions, or prototyping to uncover specific needs and clarify ambiguities.

Example: Eliciting details about the booking system, such as whether users need filters for room types or support for multiple payment methods.

**Requirement Modeling:**

Requirements are organized and represented in structured formats to facilitate understanding and analysis. Common modeling techniques include use case diagrams, data flow diagrams, entity-relationship diagrams, or user stories.

Example: Creating a use case diagram to show how a customer interacts with the hotel booking system to reserve a room.

**Requirement Analysis and Specification:**

This step involves analyzing requirements for clarity, consistency, and feasibility. Requirements are documented in a Software Requirements Specification (SRS) document, which serves as a formal agreement between stakeholders and developers.

Example: Specifying that the booking system must handle 1,000 concurrent users with a response time of under 2 seconds.

**Requirement Prioritization:**


Not all requirements are equally important. Prioritization involves ranking requirements based on factors like business value, user impact, or project constraints (e.g., time, budget). This ensures that critical features are developed first.

Example: Prioritizing the ability to book a room over adding a feature for personalized room recommendations.

**Requirement Validation:**

Validation ensures that the documented requirements accurately reflect stakeholder needs and are feasible to implement. Techniques include reviews, walkthroughs, prototyping, or simulation with stakeholders.

Example: Stakeholders review the SRS for the hotel booking system to confirm that all necessary features, like cancellation policies, are included.


### Why is Requirement Analysis Important

Requirement Analysis is a pivotal phase in the Software Development Lifecycle (SDLC) that ensures a software project aligns with stakeholder needs and project goals. Below are three key reasons why Requirement Analysis is critical, with detailed descriptions:

**1. Ensures Alignment with Stakeholder Needs and Expectations**

* Description: Requirement Analysis involves gathering, eliciting, and validating requirements through direct engagement with stakeholders (e.g., clients, end-users, or business analysts). This process ensures that the software addresses the actual needs and expectations of those who will use or benefit from it. By clarifying ambiguities and resolving conflicting requirements early, Requirement Analysis creates a shared understanding between stakeholders and the development team, reducing the risk of delivering a system that fails to meet user needs.
* Impact: Without proper alignment, the final product may miss critical features or include unnecessary ones, leading to user dissatisfaction or project failure. For example, in a hotel booking system, Requirement Analysis ensures that essential features like room reservations and payment processing are prioritized based on user input, avoiding costly missteps.

**2. Reduces Development Costs and Risks**

* Description: Identifying and resolving issues in requirements during the analysis phase is significantly less expensive than fixing them in later SDLC phases, such as design, coding, or testing. Studies, like those from the Standish Group, indicate that correcting defects in requirements during development or post-release can cost 10–100 times more than addressing them early. Requirement Analysis mitigates risks by ensuring requirements are clear, feasible, and testable, minimizing scope creep and rework.
* Impact: For instance, if a requirement for a hotel booking system to support 1,000 concurrent users is overlooked, addressing it after development could require major architectural changes. Early analysis prevents such costly oversights and reduces project risks.

**3. Facilitates Effective Resource Allocation and Prioritization**
* Description: Requirement Analysis includes prioritizing requirements based on their business value, urgency, or impact, ensuring that limited resources (time, budget, personnel) are allocated to the most critical features first. This is especially important in projects with constraints, as it maximizes value delivery. By focusing on essential requirements, teams can deliver a functional product within scope and avoid wasting effort on low-priority features.
* Impact: In a hotel booking system, prioritizing core functionality (e.g., booking and payment processing) over secondary features (e.g., user reviews) ensures the system meets critical needs within budget and timeline constraints, enhancing project efficiency and success.


### Key Activities in Requirement Analysis


**1. Requirement Gathering**
* Involves collecting high-level requirements from stakeholders, users, and clients.

* Focuses on understanding what the customer needs and expects from the system.

* Usually done through interviews, surveys, questionnaires, and observation.

* It is the starting point of the requirements engineering process.

**2. Requirement Elicitation**
* Goes deeper than gathering by exploring and uncovering hidden or unstated requirements.

* Uses techniques like brainstorming, prototyping, workshops, and use case scenarios.

* Encourages collaboration between stakeholders and analysts to clarify expectations.

* Helps reveal conflicts, ambiguities, and assumptions in initial inputs.

**3. Requirement Documentation**
* Converts gathered and elicited requirements into structured and formalized formats.

* Creates artifacts such as Software Requirements Specifications (SRS), user stories, and use cases.

* Ensures consistency, clarity, and traceability of all requirements.

* Serves as a reference for developers, testers, and stakeholders throughout the project.

**4. Requirement Analysis and Modeling**
* Involves examining and organizing requirements to identify gaps, redundancies, or conflicts.

* Uses models like data flow diagrams (DFDs), entity-relationship diagrams (ERDs), or UML.

* Categorizes requirements into functional and non-functional types.

* Helps stakeholders visualize system behavior and system structure.

**5. Requirement Validation**
* Ensures that documented requirements accurately reflect stakeholder needs.

* Typically involves reviews, walkthroughs, inspections, and requirement traceability matrices.

* Aims to detect errors, omissions, and inconsistencies early before development starts.

* Validated requirements reduce rework, save time, and improve project success.



### Types of Requirements


**1\. User Management**

**Functional Requirements:**

- Define what the system **should do** regarding users.
- **Examples**:
  - Users must be able to create an account with email and password.
  - Users can log in and log out securely.
  - Admins can deactivate or delete user accounts.
  - Users can update personal information such as name, email, and contact number.

**Non-Functional Requirements:**

- Define **how well** user-related functions perform.
- **Examples**:
  - Passwords must be stored securely using encryption (e.g., bcrypt).
  - Login attempts must be rate-limited to 5 per minute to prevent brute-force attacks.
  - The system should support up to 10,000 registered users concurrently.

**2\. Booking Management**

**Functional Requirements:**

- Define core booking features.
- **Examples**:
  - Users can search for available properties or services by date and location.
  - Users can make, update, or cancel a booking.
  - The system sends a confirmation email upon successful booking.
  - Admins can view and manage all bookings in the system.

**Non-Functional Requirements:**

- Address performance and usability aspects of bookings.
- **Examples**:
  - The booking confirmation email should be sent within 60 seconds.
  - System uptime for booking services must be at least 99.5%.
  - Booking transactions must be ACID-compliant to avoid double booking.

**3\. Payment Integration**

**Functional Requirements:**

- Describe the actions around processing payments.
- **Examples**:
  - Users can pay using credit/debit cards or mobile money.
  - The system must generate an invoice after each successful payment.
  - Refunds must be processed by admins through the dashboard.

**Non-Functional Requirements:**

- Cover the security and reliability of transactions.
- **Examples**:
  - All payment data must be transmitted over HTTPS.
  - Payment gateway must comply with PCI-DSS standards.
  - The system must handle 100 payment requests per minute without failure.

**4\. Notifications**

**Functional Requirements:**

- Actions for notifying users.
- **Examples**:
  - Users receive email and/or SMS notifications for booking confirmations, cancellations, or reminders.
  - Admins get notified when a high-value booking is made.

**Non-Functional Requirements:**

- Focus on timeliness and delivery reliability.
- **Examples**:
  - 95% of notifications must be delivered within 1 minute of the event.
  - The system should retry sending failed notifications up to 3 times.

**5\. Reporting and Analytics**

**Functional Requirements:**

- Define system reporting features.
- **Examples**:
  - Admins can generate reports showing total bookings by month.
  - Users can view their past booking history in their dashboard.

**Non-Functional Requirements:**

- Describe report availability and system efficiency.
- **Examples**:
  - Reports should be generated in under 5 seconds.
  - Exported reports must be available in PDF and CSV formats.



### Use Case Diagram


**What Are Use Case Diagrams?**

A **Use Case Diagram** is a type of **UML (Unified Modeling Language)** diagram used in software engineering to visually represent the **interactions between users (actors)** and the **system's functionalities (use cases)**.

- It shows **what** the system will do, not **how** it will do it.
- Includes **actors** (users or other systems), **use cases** (tasks/goals), and the **relationships** between them.

**Example:**

In a **booking management system**, a use case diagram might include:

- Actors: _User_, _Admin_
- Use Cases: _Search Property_, _Make Booking_, _Cancel Booking_, _Process Payment_

**Benefits of Use Case Diagrams**

**1\. Clarify System Scope**

- Clearly outlines what functionalities the system must support.
- Helps identify what is inside or outside the boundaries of the system.

**2\. Enhance Communication**

- Provides a simple, visual way for stakeholders (technical and non-technical) to understand the system.
- Encourages collaboration and feedback early in the project.

**3\. Support Requirement Gathering**

- Helps discover and organize functional requirements.
- Identifies user goals, which can guide requirement elicitation.

**4\. Improve System Design**

- Assists developers and designers in understanding user interactions and system features.
- Serves as a foundation for more detailed diagrams (e.g., activity or sequence diagrams).

**5\. Facilitate Testing**

- Use cases can be used to define test scenarios or user acceptance tests.
- Ensures the system meets user needs through traceable actions.



![alx-booking-uc.png](https://drive.google.com/file/d/1ySyEDHUs-MFQE4KTbYSu-vu4VyihYtV9/view?usp=sharing)



### Acceptance Criteria



**Importance of Acceptance Criteria in Requirement Analysis**

**Acceptance Criteria** are a set of predefined conditions that a product or feature must meet to be accepted by the client, user, or stakeholder. They play a crucial role in **Requirement Analysis** for the following reasons:

**Why Acceptance Criteria Matter:**

1. **Clarity and Shared Understanding**
    - They eliminate ambiguity by clearly defining what success looks like for a feature.
    - Developers, testers, and stakeholders all align on the expected behavior and outcomes.
2. **Guides Development**
    - Developers use acceptance criteria to understand exactly what needs to be built.
    - It acts like a mini-contract that ensures the implementation is on track.
3. **Basis for Testing**
    - QA teams use acceptance criteria to write test cases.
    - It ensures that testing focuses on real-world user expectations.
4. **Scope Control**
    - Helps in avoiding scope creep by defining what is in and out of bounds for a given feature.
    - Any functionality outside the criteria is treated as a separate requirement.
5. **Supports Agile and Iterative Workflows**
    - In Agile frameworks, well-written acceptance criteria improve user story quality.
    - It enables better sprint planning and task estimation.

**Example: Acceptance Criteria for the Checkout Feature**

**Feature:** _Checkout – Booking Management System_

**User Story:**  
_As a customer, I want to complete the checkout process so that I can confirm my booking and make a payment._

**Acceptance Criteria:**

1. The checkout page must display a summary of the selected property, check-in/check-out dates, and total cost.
2. The user must be able to enter and save payment details securely.
3. The system must calculate and display applicable taxes and service fees.
4. The payment must be processed via the integrated payment gateway.
5. A confirmation message must be displayed upon successful payment.
6. An email receipt must be sent to the user within 5 minutes of payment.
7. If payment fails, the user must receive an error message with retry options.
8. Booking status should be updated to "Confirmed" only after successful payment.



