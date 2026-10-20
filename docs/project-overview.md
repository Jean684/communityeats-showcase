# CommunityEats — Project Overview

## Project Context

CommunityEats was developed as part of **Software Engineering: Process and Tools (COSC2299)** at **RMIT University**.

It was a university team project where we worked in an Agile/Scrum environment to design and build a platform connecting students looking for affordable meals with local home cooks.

The system had separate experiences for Buyers, Cooks and Administrators, which meant we had to think about how different users would interact with the platform and how those workflows connected together.

This repository is a portfolio showcase only. The original source code is not included due to intellectual property restrictions.

---

## The Problem

The idea behind CommunityEats was to make it easier for students to find affordable and convenient meal options, while also giving local home cooks a way to offer food within their community.

The platform was designed around three main user groups:

- **Buyers** can discover meals and interact with local cooks.
- **Cooks** can manage their profiles, meal listings and verification.
- **Administrators** can manage users and review verification requests.

---

## Team & Development Process

CommunityEats was developed as a team project using Scrum.

We worked across three main stages:

- Sprint 0
- Sprint 1
- Sprint 2

Throughout the project, we used:

- Git and GitHub
- Feature branches
- Pull requests
- GitHub Projects
- Sprint planning
- Testing and review
- Tutor feedback to refine requirements and implementation

Working this way gave me more experience with what it actually feels like to build software in a shared codebase, where changes from one person can affect someone else’s work.

---

## My Role

My main contributions focused on registration and verification workflows.

### Buyer & Cook Registration

I worked on registration interfaces for different user roles, helping support separate Buyer and Cook account flows.

This involved making sure the registration process matched the role each user was signing up for and integrated properly with the rest of the application.

### Verification Submission

I developed verification submission functionality that allowed Buyers and Cooks to:

- Upload supporting evidence
- Add notes
- Submit verification requests
- View their current verification status

One thing I had to think carefully about here was keeping the scope clear. Submission was about collecting evidence and setting the request to Pending, while the actual review decision belonged to the admin workflow.

### Admin Verification Management

I also contributed to the administrative side of verification, including:

- Viewing submitted verification requests
- Supporting both Buyer and Cook requests
- Inspecting individual submissions
- Reviewing uploaded evidence
- Approving or rejecting requests
- Updating verification status

This was one of the more interesting parts of the project because it connected the user-facing flow with the admin side of the system.

---

## Technical Approach

CommunityEats was built using:

- Java
- Spring Boot
- Spring Security
- MySQL
- HTML / CSS
- Maven
- Docker
- Git & GitHub

The application followed a layered structure using controllers, services, repositories and the database.

A typical request flowed through the system like this:

**User → Browser → Security → Controller → Service → Repository → MySQL → View → Browser**

Working with this structure helped me understand how responsibilities are separated across different parts of a Spring Boot application rather than putting everything in one place.

---

## Testing

Testing was a regular part of the project rather than something we only did at the end.

My work included:

- Running the Maven test suite
- Updating tests when features changed
- Debugging failing tests
- Checking role-specific workflows
- Regression testing after changes
- Testing verification approval and rejection behaviour

At one point, the full project test suite completed with:

**293 tests, 0 failures**

Seeing the full suite pass after integrating different features was probably one of the more satisfying parts of the project.

---

## Challenges

### Keeping Verification Features in Scope

One challenge was making sure different user stories did not start overlapping too much.

For example, verification submission and admin review could easily have become one large feature. Instead, Buyers and Cooks were responsible for submitting evidence and receiving a Pending status, while administrators handled approval and rejection separately.

Keeping those responsibilities separate made the implementation cleaner and helped avoid duplicated logic.

### Integrating Team Work

Another challenge was working in a shared codebase where multiple people were developing different parts of the system at the same time.

A change that worked perfectly on its own could still cause issues once it was merged with someone else’s work.

This gave me more experience with:

- reading code written by other people
- working around existing structures
- resolving integration issues
- testing beyond just the feature I had personally changed

---

## What I Learned

CommunityEats helped me become much more comfortable working on a larger application rather than just building isolated features.

It strengthened my understanding of:

- Spring Boot application structure
- Role-based authentication and authorisation
- Database-backed workflows
- Feature scoping
- Testing and debugging
- Pull request workflows
- Working with changing requirements
- Collaborating within an existing codebase
- Agile/Scrum development

The biggest thing I took away from the project was learning how much software development depends on the connections between different parts of the system — and between different people on the team.

---

## Portfolio Notes

The screenshots in this repository use demonstration data and are included to show the overall product and the areas I contributed to.

The original project source code is not publicly included because the project contains intellectual property belonging to multiple parties.