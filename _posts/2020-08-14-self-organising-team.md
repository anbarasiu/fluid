---
layout: post
title: Self Organising Engineering Team
description: What could an ideal self-organising engineering team look like?
summary: Nascent set thoughts on self-organising engineering teams, as I try to gather and put together a better model for understanding.
tags: engineering systems
---

What could an ideal self-organising engineering team look like?

We assume a common structure for an engineering team, comprising product engineers, designer(s) and a product manager. Ideally an individual would be able to execute independently or contribute significantly in terms of the below. The ideal team member handles all of these for a particular problem statement. Note that we don't deal with product features, instead we deal with customer pain points or problem statements.


1.  Technical
    
2.  Managerial
    
3.  Contextual
    

### Technical (How)

-   Understands the problem statement in terms of the customer need and could propose an appropriate technical solution.
    
-   Can independently execute and implement the technical solution without a senior guide.
    
-   Can break down the problem into defined units of work.
    
-   Can implement solutions with the quality of code as agreed with peers, and can contribute to evolve the quality in terms of, scaling codebase and engineering pipelines for agility with minimum bugs.
    

### Managerial (When)

-   Can self-manage by estimating timelines for the broken-down units of work and collating it.
    
-   Is committed to agreed timelines and takes ownership to place their work into the hands of the customer (for example, code deployed to production or closing a communication loop with a stakeholder).
    
-   Can identify blockers/potential delays in delivery and flag them to the team.
    

### Contextual (What)

-   Can propose and weigh multiple solutions to a problem statement in order to identify the best approach for the customer segment that we’re serving.
    
-   Can help in scoping the problem to realistic sizes, for each iteration.
    

## Hiring

The team composition will matter more than the individual team members, in that the team members can work together as one cohesive unit. Each team will vary based on the stage of the company, the maturity of the product, the nature of working relationships with the stakeholders.

Define minimum thresholds in key skills that each potential hire needs to meet. Every additional hire needs to add something to the team in terms of complementary skills so that individual strengths and weaknesses can balance out. There are always tradeoffs to make, so we might be hiring for potential in a certain area. In that case, look for evidence of rate of growth in an adjacent area.

## Operating

Focus on creating the right environment for everybody to excel. 

Create cadences to minimise cognitive overload on processes, rather enable team for deep work and focus on solving customer problems, while the cadences run as background processes to aid in maintaining shipping momentum.

**Minimise ambiguities**

Product engineering and delivery, is ultimately an exercise in visualising and leavening multiple abstract ideas in people's heads, into a solid product that can be experienced by the human senses. This leads to a fine balancing act in minimising ambiguities at multiple steps along the way, while identifying the right amount of effort to spend on it, as subjectively determined by the team composition. This is a two-way reinforcing feedback loop between product and engineering.

**Engineering**

Seek to minimise ambiguity in

-   The need for the problem
-   The scope of the problem
Product Requirements Documents (PRDs) capture both the above and feed into the appropriate solution, to help the engineers working on the problem. The AI generators are solving this better with apps like Lovable generating high fidelity prototypes in a few minutes.
-   The solution decided
Technical Design Documents, Architecture Design Records (ADRs) and Request for Clarification (RFCs) have been historically relied upon to help the engineers visualise the solution and to identify tradeoffs and bottlenecks. It's turtles all the way down and it's all about how much we need to drill down into defining specs as per the maturity of the team. 
-   The engineer should be able to answer the question ‘Do I have full clarity of how to implement and get to production?’, else should ask questions to resolve any unknowns.
    
**Product**

Seek to minimise ambiguity in 

-   Estimated timelines (When will it be ready?)
-   Scope of the solution in iterations (What exactly is the customer going to get?)
Sprint boards have been relied upon to get a sense of the progress and planning epics with milestones can give a sense of the timelines.
    

### Parameters (Feedback loops)

The levers that the team could continually tweak to get to the point of being totally self-organised.

**Velocity**

-   Measure and improve time taken from requirement planning to delivery on production. Honestly I wouldn't focus on getting a quantitative measure of this. The correct answer is "it depends" on the business timelines and whether the team is able to sustain the momentum of delivery. Any time the momentum falls, the root cause for that could be any of 
- Code and architecture. In this case, it's time for a refactor by identifying the areas that slow down people. 
- Processes. It could be anything like a release pricest or a QA process. If there's a bottleneck here, question if the process is still solving the problem in a way that it was originally intended to. A system is always how it currently behaves and not how it was designed. 
- People. Is there a morale problem in the team or an individual? Is there a lack of skill for the current set of customer problems being solved by the team? Is there an individual weighing down the team?
    
-   Time to deploy (CI/CD pipelines)

-   Fail-fast feedback loops
An environment where the team can face failures safely, without impacting the customer. Tactical things would involve:
- automated tests running on every pull request, that assist code reviews
- any bugs identified to feed into the automated test suite, to avoid a future regression. This also requires active maintenance by the team to ensure this serves as a good feedback layer.
- a development environment with error tracking and it's own monitoring and alerting systems. 
- nightly regression tests that can catch issues across the system
- be as aggressive as possible about the pipeline durations so that they always run as quickly as possible. Parallelize runs wherever possible.
    

**Quality**

-   Static code analyses, linting tools, to eliminate nit-picks and differences over coding styles in reviews

-   Code reviews. AI code review tool integration as the first pass check, so that team members need only verify functional requirements. 
    
-   Automated test suites (Unit tests, Integration tests and End-to-end tests)
    
-   QA process (manual and exploratory). Dependent on the product. For example, a payment product might involve exploratory testing to identify 
flows that aren't straightforward and to identify potential fraud scenarios. Whereas in a SAAS product with no operational touch points, it maybe possible to automate all the flows.

**Maintainability**

-   Monitoring with defined Service-level indictors and Service-level objectives

-   Observability with logs and traces.

-   Alerting

-   Dashboards with ownership

