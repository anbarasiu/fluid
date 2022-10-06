---
layout: post
title: Self Organising Team
description: What could an ideal self-organising team look like?
summary: Nascent set thoughts on self-organising teams, as I try to gather and put together a better model for understanding.
tags: engineering systems
---

What could an ideal self-organising team look like?

Ideally an individual would be able to execute independently or contribute significantly in terms of the below.

1.  Technical
    
2.  Managerial
    
3.  Contextual
    

### Technical (How)

-   Understands the problem statement in terms of customer need and could propose an appropriate technical solution.
    
-   Can independently execute and implement the technical solution without a senior guide.
    
-   Can break down the problem into defined units of work.
    
-   Can implement solutions with the quality of code as agreed with peers, and can contribute to evolve the quality in terms of, scaling codebase and engineering pipelines for agility with minimum bugs.
    

### Managerial (When)

-   Can self-manage by estimating timelines for the broken-down units of work and collating it.
    
-   Is committed to agreed timelines and takes ownership to place their work into the hands of the customer (for example, code deployed to production or communication loop with a stakeholder).
    
-   Can identify blockers/potential delays in delivery and flag them to the team.
    

### Contextual (What)

-   Can propose and weigh multiple solutions to a problem statement in order to identify the best approach for the customer segment that we’re serving.
    
-   Can help in scoping the problem to realistic sizes, for each iteration.
    

## Hiring

Define minimum threshold levels, how to identify expected characteristics/potential.

## Operating

Focus on creating the right environment for everybody to excel

Create cadences to minimise cognitive overload on processes, rather enable team for deep work and focus on solving customer problems, while the cadences run as background processes to aid in maintaining shipping momentum

**Minimise ambiguities**

Product engineering and delivery, is ultimately an exercise in visualising and leavening multiple abstract ideas in people's heads, into a solid product that can be experienced by the human senses. This leads to a fine balancing act in minimising ambiguities at multiple steps along the way, while identifying the right amount of effort to spend on it, as subjectively determined by the team composition. This is a two-way reinforcing feedback loop between product and engineering.

**Engineering**

Seek to minimise ambiguity in

-   The need for the problem
-   The scope of the problem
Product Requirements Documents (PRDs) capture both the above and feed into the appropriate solution.
-   The solution decided
Technical Design Documents, Architecture Design Records (ADRs) and Request for Clarification (RFCs) have been historically relied upon
-   Answer the question ‘Do I have full clarity of how to implement and get to production?’, else ask questions to resolve any unknowns
    
**Product**

Seek to minimise ambiguity in 

-   Estimated timelines (When will it be ready?)
-   Scope of the solution in iterations (What exactly is the customer going to get?)
    

### Parameters (Feedback loops)

The levers that the team could continually tweak to get to the point of being totally self-organised.

**Velocity**

-   Measure and improve time taken from requirement planning to delivery on production
    
-   Time to deploy (CI/CD pipelines)
    

**Quality**

-   Static code analyses, linting tools, to eliminate nit-picks and differences over coding styles in reviews

-   Code reviews
    
-   Automated test suites (Unit tests, Integration tests and End-to-end tests)
    
-   QA process (manual)
    

**Maintainabiilty**

-   Monitoring with defined Service-level indictors and Service-level objectives

-   Observability with logs and traces

-   Alerting

-   Dashboards with ownership

