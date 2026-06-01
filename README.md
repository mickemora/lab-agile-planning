# Lab Agile Planning

This repository contains an Agile planning lab focused on defining, organizing, and managing user stories for a simple counter service.

The project demonstrates how Agile teams capture requirements as user stories, define acceptance criteria, prioritize work, track issues, and plan functionality incrementally.

## Project Overview

The lab centers around a service that provides counter functionality. The counter service is represented through GitHub issues written as Agile user stories.

The planned service includes capabilities such as:

- Creating or using a counter
- Incrementing a counter
- Reading the current counter value
- Persisting counter values across restarts
- Supporting multiple counters
- Resetting counters
- Removing counters
- Updating counters to new values
- Deploying the service to the cloud

This repository is not primarily a code implementation repository. Instead, it is a planning and project management exercise that uses GitHub Issues to model Agile product backlog items.

## Main Objective

The objective of this lab is to practice Agile planning techniques using GitHub as a project management tool.

The lab demonstrates how to:

1. Write user stories
2. Capture requirements from different stakeholder perspectives
3. Define acceptance criteria
4. Organize work as GitHub issues
5. Track open and closed backlog items
6. Think about product functionality incrementally
7. Connect user needs to technical implementation considerations

## Agile User Story Format

The issues in this repository follow the common Agile user story format:

```text
As a [role],
I need [capability],
So that [benefit].
```

This format helps clarify:

- Who needs the feature
- What capability is required
- Why the feature matters

## Product Backlog Summary

The backlog describes a counter service with the following user stories and feature areas.

### Counter Service

The foundational story defines the need for a service that has a counter.

The service should allow users to track how many times something was done. The issue also identifies the need to increment the counter and retrieve the current value.

### Persist Counter Across Restarts

The service should persist the last known count so users do not lose their counter values after the service restarts.

The issue notes that Redis may be used as the persistence layer and that the counter can be stored as a name-value pair.

### Multiple Counters

The service should allow users to manage multiple counters so they can track several counts at the same time.

### Reset Counter

System administrators should be able to reset a counter back to zero when counting needs to restart.

### Remove Counter

Users should be able to remove a counter when it is no longer needed or when a new counter needs to be created.

### Update Counter Value

Users should be able to update a counter to a new value when needed.

### Deploy Service to the Cloud

The backlog includes remaining work related to deploying the service to the cloud.

## Repository Structure

```text
.
└── README.md
```

Most of the project information is managed through GitHub Issues rather than source code files.

## Key Agile Concepts Demonstrated

This lab demonstrates several Agile and product management concepts:

- User stories
- Product backlog management
- Acceptance criteria
- Stakeholder roles
- Feature prioritization
- Incremental planning
- Issue tracking
- Functional decomposition
- Requirements refinement
- Cloud deployment planning

## Example User Stories

### Counter Creation / Usage

```text
As a User,
I need a service that has a counter,
So that I can keep track of how many times something was done.
```

### Counter Persistence

```text
As a Service Provider,
I need the service to persist the last known count,
So that users don't lose track of their counts after the service is restarted.
```

### Multiple Counters

```text
As a User,
I need to have multiple counters,
So that I can keep track of several counts at once.
```

### Counter Reset

```text
As a System Administrator,
I need the ability to reset the counter,
So that I can redo counting from the start.
```

## Potential Technical Architecture

Although this repository focuses on Agile planning, the backlog suggests a possible architecture for implementation.

A simple counter service could include:

```text
Client / API Consumer
        ↓
Counter Service API
        ↓
Business Logic Layer
        ↓
Redis Data Store
        ↓
Cloud Deployment Environment
```

Potential technical components could include:

- REST API
- Counter service logic
- Redis for persistence
- Cloud hosting platform
- Automated deployment pipeline

## How This Lab Can Be Used

This repository can be used to practice:

- Writing product backlog items
- Managing work through GitHub Issues
- Defining acceptance criteria
- Planning an MVP
- Thinking through product increments
- Preparing work for future implementation
- Connecting Agile planning with cloud-native service design

## Suggested MVP Scope

A practical minimum viable product could include:

1. Create or initialize a counter
2. Increment the counter
3. Retrieve the current counter value
4. Persist the counter value
5. Reset the counter

After the MVP, the service could be extended to support multiple counters, deletion, value updates, and cloud deployment.

## Potential Enhancements

Future improvements could include:

- Add a project board to visualize backlog status
- Add labels for priority, sprint, and story type
- Add story points or effort estimates
- Add acceptance criteria to every issue
- Add a milestone for MVP release
- Add architecture diagrams
- Add implementation code for the counter service
- Add Redis integration
- Add API documentation
- Add cloud deployment instructions
- Add automated tests

## Skills Demonstrated

This lab demonstrates foundational Agile and project management skills, including:

- Agile requirements writing
- Product backlog creation
- GitHub issue management
- User-centered requirement framing
- Acceptance criteria definition
- Incremental planning
- Technical feature decomposition
- Cloud-readiness thinking

## Summary

This repository is an Agile planning exercise for a counter service. It uses GitHub Issues to define user stories, capture requirements, and organize work around a small but practical service. The lab demonstrates how Agile teams convert user needs into backlog items that can later be implemented, tested, and deployed.
