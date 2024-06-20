# Time Tracker Web Application Development Documentation

## :star: Project Overview
The Time Tracker web application enables users to track their working hours, manage sessions, and generate reports based on their work patterns. The application will be hosted on a cloud platform and accessible to anyone with an internet connection.

## :clipboard: High-Level Requirements
1. **Cloud Hosting and Accessibility**
   - :cloud: Host the site on a cloud platform (e.g., AWS, Azure, GCP).
   - :globe_with_meridians: Ensure the site is accessible via the internet.

2. **User Navigation**
   - :mag: Visitors can navigate to various sections: Homepage, Product Details, About Us, Contact Us, Sign In, Sign Up, Copy Rights, and Author/Developer Page.
   - :arrows_clockwise: Redirect users based on authentication status (e.g., Logo redirects to Homepage if not signed in, Dashboard if signed in).

3. **Account Management**
   - :lock_with_ink_pen: **Sign Up:** Form with email verification, unique username, and PIN creation.
   - :key: **Sign In:** Authentication with username and password, including "Forgot Username" and "Forgot Password" functionalities.
   - :no_entry: **Account Deletion:** User-initiated with double confirmation.

4. **Time Tracking Dashboard**
   - :stopwatch: Start, pause, and resume shifts/sessions.
   - :clock1: Display clocks for session duration and current local time.
   - :bar_chart: Calculate and display worked hours (shift, day, week, month).
   - :memo: Generate reports for average worked hours (shift, day, week, month).

## :page_facing_up: Detailed Requirements

### :cloud: Cloud Hosting and Accessibility
- **Task:** Set up a cloud environment on a provider such as AWS, Azure, or GCP.
- **Deliverables:** 
  - A live URL (e.g., www.timetracker.com)
  - SSL certificate for secure access

### :mag: User Navigation
- **Task:** Design and implement the site's navigation structure.
- **Deliverables:**
  - Navigation menu with links to Homepage, Product Details, About Us, Contact Us, Sign In, Sign Up, Copy Rights, and Author/Developer Page.
  - Conditional redirection based on user authentication status.
  - **About Us Page:** Link to GitHub profile.
  - **Contact Us Page:** Display email and LinkedIn profile.
  - **Product Details Page:** Describe the project and its features.
  - **Footer:** Include Copy Rights section.
  - **Author/Developer Page:** Include LinkedIn and GitHub profile links.

### :lock_with_ink_pen: Account Management
- **Sign Up:**
  - **Task:** Create a registration form with email verification.
  - **Deliverables:**
    - Form fields: Email, Username, PIN, Confirm PIN
    - Email verification with OTP
    - Form validation for username and PIN
    - Thank you email on successful registration

- **Sign In:**
  - **Task:** Create a login form with username and password.
  - **Deliverables:**
    - Form fields: Username, Password
    - "Forgot Username" and "Forgot Password" functionalities
    - Eye toggle for password visibility
    - Tooltip for input box information
    - Redirection to Dashboard on successful login
    - Error message on failed login

- **Account Deletion:**
  - **Task:** Implement account deletion with double confirmation.
  - **Deliverables:**
    - Confirmation dialog
    - Database update to remove user data

### :stopwatch: Time Tracking Dashboard
- **Task:** Develop the dashboard to manage and display time tracking information.
- **Deliverables:**
  - Start, pause, and resume session functionality
  - Clocks for session duration and current local time
  - Calculation and display of worked hours (shift, day, week, month)
  - Report section with averages (shift, day, week, month)

## :construction: Development Phases

### Phase 1: Setup and Basic Navigation
- **Tasks:**
  - Cloud setup and hosting
  - Implement the basic structure of the site with navigation links
- **Deliverables:**
  - Live URL
  - Initial site structure with navigation

### Phase 2: User Authentication
- **Tasks:**
  - Develop and integrate the Sign Up and Sign In pages
  - Implement email verification, and forgot username/password functionalities
- **Deliverables:**
  - Fully functional Sign Up and Sign In pages
  - Email verification system
  - Forgot Username and Forgot Password functionalities

### Phase 3: Dashboard Development
- **Tasks:**
  - Create the dashboard with time tracking and reporting features
  - Ensure functionality for starting, pausing, and resuming sessions
- **Deliverables:**
  - Time tracking dashboard
  - Session management functionalities

### Phase 4: Final Touches and Testing
- **Tasks:**
  - Implement account deletion
  - Conduct thorough testing (unit tests, integration tests, and user acceptance tests)
  - Optimize for performance and security
- **Deliverables:**
  - Account deletion feature
  - Comprehensive test reports
  - Optimized and secure application

## :hammer_and_wrench: Tools and Technologies
- **Frontend:** HTML, CSS, JavaScript (React, Vue.js, or Angular)
- **Backend:** Node.js (Express.js), Python (Django/Flask), or Ruby on Rails
- **Database:** PostgreSQL, MySQL, or MongoDB
- **Email Service:** SendGrid, Mailgun, or AWS SES
- **Hosting:** AWS (EC2, S3), Azure, or GCP
- **Version Control:** GitHub

## :bulb: Use Cases

### Use Case 1: User Registration
**Description:** A user registers for a new account.
**Steps:**
1. User navigates to the Sign Up page.
2. User fills out the registration form with email, username, and PIN.
3. User receives an OTP via email and enters it for verification.
4. User submits the form and receives a thank you email.
5. User is redirected to the welcome page.

### Use Case 2: User Login
**Description:** A user logs into their account.
**Steps:**
1. User navigates to the Sign In page.
2. User enters their username and password.
3. System validates the credentials.
4. Upon successful validation, user is redirected to the dashboard.
5. If validation fails, an error message is displayed.

### Use Case 3: Time Tracking
**Description:** A user starts, pauses, and resumes a session.
**Steps:**
1. User logs into the application.
2. User starts a new session, and the session clock begins.
3. User pauses the session, and the session clock stops.
4. User resumes the session, and the session clock continues.
5. User views the session details and reports on the dashboard.

## :bookmark: Conclusion
This documentation outlines the development process for the Time Tracker web application, providing detailed requirements, development phases, and use cases to ensure a clear and structured approach. By following this guide, developers can systematically build and deploy the application, ensuring all features and functionalities are implemented as specified.
