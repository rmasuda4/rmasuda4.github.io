---
layout: essay
type: essay
title: "A Future In Software Engineering"
# All dates must be YYYY-MM-DD format!
date: 2025-12-04
published: true
labels:
  - Software Engineering
---

<img width="200px" class="rounded float-start pe-4" src="../img/Screenshot 2025-09-10 153521.png">


## TDesign Patterns: The Strategic Playbook of Software Development

Design patterns,simply put, are the solutions to recurring problems in software development and engineering, it is the fact that people often take the same or similar approaches to problems that are alike. One could easily compare it to how experienced players develop strategies for situations they encounter repeatedly in games, when going through a maze people often follow their own unique strategy but use the same strategy almost every time. Design patterns emerged from the collective wisdom of developers who noticed that certain design challenges appeared over and over across different projects; the need to share data between components, the desire to ensure only one instance of a resource exists, or the requirement to protect certain functionality from unauthorized access. Rather than reinventing the wheel each time these problems arise, the software community takes these proven approaches and turns them into reusable templates. These patterns represent decades of collective experience transformed into learnable, repeatable strategies that help developers avoid common pitfalls and mistakes in order to build more maintainable, scalable solutions.



## Personal application and uses

In developing UH Connect, our gamer focused social platform, we've naturally gravitated toward all three major categories of design pattern. Creational patterns form the foundation of how we instantiate objects and manage resources: our Prisma database client operates as a Singleton, ensuring a single point of connection to our PostgreSQL database rather than spawning multiple competing instances. The Factory pattern emerges in our user creation flow, where “createUser” takes raw form data and constructs properly validated User objects with hashed passwords and default profile settings. Structural patterns define how our components relate and interact: React's component-based architecture itself embodies the Composite pattern, allowing us to build complex interfaces from simple, reusable building blocks like our Navbar, Footer, and ProfileCard components that can be nested and combined infinitely. Behavioral patterns orchestrate the runtime interactions within our system: the Observer pattern manifests everywhere React's state management touches, from useState hooks triggering re-renders when user data changes to our authentication system watching for session updates and redirecting users accordingly. Our profile page exemplifies the Template Method pattern, establishing a consistent structure with a header card with user info, biography section, game interests, gaming preferences, and recommendations, that creates a predictable flow while allowing each section's content to vary based on the specific user's data. These three categories creational, structural, and behavioral don't exist in isolation within our codebase; they interweave to create a system where objects are created efficiently, components are organized logically, and behaviors coordinate seamlessly, transforming what could have been tangled spaghetti code into an architecture that both current developers and future maintainers can navigate with confidence.



