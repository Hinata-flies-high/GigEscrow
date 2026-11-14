
# GigEscrow

A freelance milestone escrow management and dispute-resolution dashboard for clients, freelancers, and arbitrators.

## Overview

GigEscrow is a web-based prototype designed to make freelance project agreements, milestone progress, payment status, work submissions, and dispute records easier to manage in one place.
Clients can create contracts, divide projects into milestones, and simulate funding. Freelancers can view funded milestones and submit their work for review. Clients can approve submissions and simulate payment releases, while arbitrators can review disputed milestones and record a resolution.
The goal is to provide all parties with a clearer, shared record of the project workflow.

NOTE: GigEscrow is an educational demo. It does not hold, transfer, or process real money. All users, contracts, transactions, and amounts are sample data. Decisions made in the prototype have no legal effect.

## Problem Statement

Freelance projects often involve multiple separate conversations and records for agreements, deliverables, payments, and disagreements.

This can create uncertainty:
- Freelancers may be unsure whether funds have been set aside before beginning work.
- Clients may be unsure whether submitted work meets the agreed requirements.
- When disagreements occur, the relevant terms, submissions, and payment records may be scattered across different places.

GigEscrow aims to bring these details together in a single dashboard, with milestone-based payment tracking and a structured dispute-resolution workflow.

## User Roles


Client : Create contracts, add milestones, simulate funding, review submissions, approve or dispute work 
Freelancer : View milestones and funding status, submit work, track approvals and disputes 
Arbitrator : Review disputed milestones, examine project records, and record a resolution 

## Core MVP Features

The following features form the minimum viable product (MVP) described in the project requirements.

1. Contract and Milestone Management
- Create contracts with project details and freelancer information.
- Add milestones with a title, deliverable, due date, and amount.
- Validate required fields before saving.

2. Simulated Escrow Funding
- Allow clients to fund individual milestones.
- Update milestone status from `Draft` to `Funded`.
- Display escrow balances and transaction information.
- Use simulated transactions only; no real payments are processed.

3. Work Submission and Review
- Allow freelancers to submit work notes and a link or file name.
- Update the milestone status to `Submitted`.
- Allow clients to approve submissions and simulate payment release.
- Allow clients to request changes.

4. Dispute Management
- Allow a client or freelancer to raise a dispute with a reason and statement.
- Keep the milestone amount locked in the simulated escrow while the dispute is open.
- Provide an arbitrator with a dispute queue and relevant milestone history.
- Allow the arbitrator to record one of three outcomes:
  - Release the amount to the freelancer.
  - Refund the amount to the client.
  - Split the amount between both parties.

5. Role-Based Actions
- Provide separate views for clients, freelancers, and arbitrators.
- Restrict actions according to the selected role.
- Display appropriate feedback when an action is not permitted.

6. Data Persistence and Responsive UI
- Store sample application data using browser `localStorage` or JSON.
- Provide a responsive interface for laptop and phone-width screens.
- Include form validation and clear success, warning, and error messages.

## Additional Features

These features are planned as enhancements after the core MVP is functional.

### Good-to-Have Features
- Search contracts, milestones, and disputes.
- Filter records by status.
- Export milestone or transaction tables as CSV or PDF.
- Add a simple switch between Freelancer, Client, and Arbitrator views.

### Stretch Features
- Explore React with Vite as an alternative frontend setup.
- Add charts for escrow amounts held, released, and refunded using Chart.js.
- Explore Leaflet for displaying sample client and freelancer locations.

## Technology Stack


HTML5:Page structure and semantic content 
CSS3 : Styling and responsive layouts 
JavaScript : Application logic, interactions, validation, and workflow 
Bootstrap 5 : Responsive UI components and layout 
localStorage / JSON : Local persistence of sample data 
Git and GitHub : Version control and collaboration 

React + Vite, Chart.js, and Leaflet are optional learning/stretch technologies rather than required MVP dependencies.

## Application Workflow

1. Contract creation: The client creates a contract and adds milestones.
2. Funding: The client simulates funding for a milestone.
3. Work submission:The freelancer submits work against a funded milestone.
4. Review: The client reviews the submission and approves it, requests changes, or raises a dispute.
5. Dispute resolution: If a dispute is raised, the arbitrator reviews the available records and records a decision.
6. Status and history: The application updates the relevant statuses, balances, and activity history.

## Planned Screens

- Home / Role Selection
- Dashboard
- Contracts
- Contract Details
- Milestone Details
- Dispute Queue
- Dispute Details
- About / Help

## Scope and Limitations

This prototype focuses on demonstrating the workflow and application logic.

The following are outside the scope of this project:
- Real payment processing or payment gateway integration.
- Real bank accounts or holding actual funds.
- Real identity verification.
- Server-side user accounts, authentication, or login.
- Messaging and email notifications.
- Legally binding arbitration.
- Taxes, invoicing, and platform fees.

A production escrow platform would require appropriate payment infrastructure, a trusted backend, and relevant legal and regulatory arrangements.

## Project Status

Currently in the planning and development phase. Features will be implemented and tested incrementally, beginning with the core contract, milestone, funding, submission, and dispute workflows.

## Team

- Khushi Shah
- Aayushi Sharma

Mentor / Reviewer: Madhushri Tangali


