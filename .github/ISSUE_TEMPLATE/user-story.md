---
name: User Story
about: This template defines a user story
title: ''
labels: ''
assignees: ''

---

**As a** [role]
**I need** [function]
**So that** [benefit]

### Details and Assumptions
    * [document what you know]

### Acceptance Criteria
    gherkin
    Given [some context]
    When [certain action is taken]
    Then [the outcome of action is observed]

# All my 10 user stories

### 1. Finish user stories
**As a** product owner  
**I need** complete user stories documented in GitHub  
**So that** developers clearly understand the scope and features of the application  

### Details and Assumptions
* Stories must follow the agreed template  
* All required stories must be captured before development starts  

### Acceptance Criteria
```gherkin
Given I am on the GitHub repository  
When I review the documentation  
Then I should see at least 10 well-structured user stories
```

---

### 2. Initialize and populate MongoDB
**As a** backend developer  
**I need** a MongoDB database initialized and seeded with sample data  
**So that** the application has a working persistence layer for development and testing  

### Details and Assumptions
* Use MongoDB Atlas or a local instance  
* Include seed data for gifts, users, and comments  

### Acceptance Criteria
```gherkin
Given MongoDB is running  
When I connect using the application’s connection string  
Then I should see the database created with predefined collections and sample data
```

---

### 3. Run skeleton application
**As a** developer  
**I need** a runnable skeleton version of the application  
**So that** the project structure is validated and everyone can start from a common baseline  

### Details and Assumptions
* The skeleton should include backend and frontend setup  
* Backend uses Express + MongoDB, frontend uses React  

### Acceptance Criteria
```gherkin
Given the repository is cloned  
When I run npm start for backend and frontend  
Then I should see the skeleton app running without errors
```

---

### 4. Implement a landing page and navigation
**As a** user  
**I need** a landing page with navigation links  
**So that** I can access different sections of the application easily  

### Details and Assumptions
* Landing page must show branding and a welcome message  
* Navigation includes Home, Gifts, Login/Signup  

### Acceptance Criteria
```gherkin
Given I open the app in a browser  
When I view the landing page  
Then I should see navigation links that route correctly to other pages
```

---

### 5. Add authentication components and logic
**As a** user  
**I need** login and signup functionality  
**So that** I can create an account and access personalized features  

### Details and Assumptions
* Use JWT authentication  
* Include forms for login and signup  

### Acceptance Criteria
```gherkin
Given I am on the login page  
When I enter valid credentials  
Then I should be redirected to my dashboard with a valid session
```

---

### 6. Implement Gifts details page
**As a** user  
**I need** a gift details page  
**So that** I can view information about a specific gift  

### Details and Assumptions
* Each gift should have title, description, image, and comments  
* Accessible from search results or gift listings  

### Acceptance Criteria
```gherkin
Given I am on the gifts listing page  
When I click on a gift  
Then I should see a dedicated gift details page with its full information
```

---

### 7. Implement a search component
**As a** user  
**I need** a search function  
**So that** I can quickly find gifts by name or category  

### Details and Assumptions
* Search should be case-insensitive  
* Display results dynamically  

### Acceptance Criteria
```gherkin
Given I am on the gifts page  
When I search for "flowers"  
Then I should see all gifts matching the keyword "flowers"
```

---

### 8. Design and implement the comments feature
**As a** user  
**I need** to add comments to a gift  
**So that** I can share feedback or reviews  

### Details and Assumptions
* Only logged-in users can comment  
* Comments should display username, timestamp, and text  

### Acceptance Criteria
```gherkin
Given I am logged in and viewing a gift  
When I submit a comment  
Then the comment should appear immediately below the gift details
```

---

### 9. Containerize the services and applications
**As a** DevOps engineer  
**I need** the application containerized using Docker  
**So that** it can run consistently across different environments  

### Details and Assumptions
* Each service (frontend, backend, database) has its own Dockerfile  
* Use Docker Compose for orchestration  

### Acceptance Criteria
```gherkin
Given I run docker-compose up  
When all containers start  
Then the application should be accessible in a browser without manual setup
```

---

### 10. Deploy backend and frontend
**As a** product owner  
**I need** the backend and frontend deployed to a live environment  
**So that** users can access the application publicly  

### Details and Assumptions
* Backend deployed on Render/Heroku/other cloud provider  
* Frontend deployed on GitHub Pages or Vercel  

### Acceptance Criteria
```gherkin
Given the deployment is complete  
When I visit the application URL  
Then I should be able to use all features in a production environment
```

