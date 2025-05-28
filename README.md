# frontend-engineering-team-working-style-guide

### Context 

For the past 3.5 years, I am ([Vishwajeet Vatharkar](https://vishwajeetv.com)) working as an Engineering Manager with a small technology team (30 engineers total) of a medium sized Agri-tech company based in Pune, India ([AgroStar](https://corporate.agrostar.in)). I have systematically built a team of 6 engineers from scratch, the "UI Engineering Team". The team is considered to be a high performance, successful and happy group, with 0 voluntary attrition, and good individual growth. Over the years I have learned a lot about team management, and have tried distilling my thoughts about team management into a "working style guide" for my team. Although this is something that was created for AgroStar, I believe many other engineering leaders can find this helpful as a framework for working style guide for their teams, hence I am sharing it here.

Original context - "As the frontend engineering team at AgroStar continues building & scaling people, products, processes, it becomes essential to document the working style that has been driven mostly by intuition, common sense, and thought process by the Engineering Manager.  
As we grow and aim towards building strong, independent individuals, it is important to document the philosophies and principles that guide simple day-to-day decision making.   
'Civilization advances by extending the number of important operations which we can perform without thinking of them.' In this document, we have documented these in the form working style guide."

I have removed AgroStar specific parts from this document, so this can be useful for any small to medium sized frontend engineering teams across the world.

### How to use this document?

This document is meant to be read and used by the members of the UI engineering team. This document acts as a “working guide” for the daily tasks and decision making, and exhaustively covers most of the important activities of the team.

Generally, readers should refer to the “Outline” of the document (on the left) and/ or search for the topic of interest and look for the details as and when needed.

### Why is the UI Engineering Team built?

The core function of the UI Engineering Team is to build good quality solutions for solving business and user problems, with primary focus on building user interfaces for the same.

### Core Principles

These are the foundations upon which this working style document is built.

1. Building strong and independently capable individuals.  
2. Trust is a Core Value that can act as a compass and guiding hand.  
3. Self-organization is essential.  
4. Continuous improvement is inculcated. Ask “is there a better way to do this?”  
5. Curiosity, inquisitiveness, asking “why”, and first principle thinking.  
6. High pragmatism, sensible prioritization, and lean, simplified approaches.  
7. Innovation via product thinking & building.  
8. Sustainability of and for people, practices, processes.

This working style document is divided into multiple sub-domains that are essential in day to day work of the UI Engineering team.

## Table of Contents
- [Solution Engineering Practices](#solution-engineering-practices)
  - [Fundamental principles](#fundamental-principles)
  - [Solution Design](#solution-design)
  - [Coding Practices](#coding-practices)
  - [Contract design](#contract-design)
  - [Estimation](#estimation)
  - [Developer Testing](#developer-testing)
  - [Release Practices](#release-practices)
    - [Versioning](#versioning)
    - [Managing user behavior expectation](#managing-user-behavior-expectation)
    - [Backward compatibility](#backward-compatibility)
    - [Release monitoring](#release-monitoring)

- [Task Allocation Practices](#task-allocation-practices)
  - [The input variables](#the-input-variables)

- [Engineering Quality Management Practices](#engineering-quality-management-practices)
  - [Solution, Progress, Code Reviews](#reviews)
  - [Stakeholder Experience](#stakeholder-experience)

- [People Management Practices](#people-management-practices)
  - [Trust](#trust)
  - [Work timings](#work-timings)
  - [Complimentary Offs](#complimentary-offs)
  - [Leaves](#leaves)

- [Performance Management & Appraisal Practices](#performance-management--appraisal-practices)
  - [Performance & Compensation Review Process](#performance--compensation-review-process)
  - [Promotions](#promotions)

- [Team Building & Cohesion Practices](#team-building--cohesion-practices)
  - [Celebrations](#celebrations)
  - [Rewards & Recognitions](#rewards--recognitions)

- [Team Hiring & Recruitment Practices](#team-hiring--recruitment-practices)

- [Learning & Development](#learning--development)
  - [Learning & Development Programs](#learning--development-programs)
  - [Domains of Expertise](#domains-of-expertise)
  - [Activities](#activities)
    - [Engineering reader's club](#engineering-readers-club)
    - [Public Speaking & Writing](#public-speaking--writing)
    - [Mentorship](#mentorship)

---
1. ### Solution Engineering Practices

   1. #### Fundamental principles

      1. Think about the user and the problem holistically.  
      2. Figure out a pragmatic, and efficient way to solve the problem, under the constraints of requirements and supporting systems.  
      3. Quality requirements are highly subjective. Build “good enough” software. However, if all things equal, we will strive to provide the best quality solution.   
      4. Understand that building software and writing code can be the least efficient way to solve a problem, though not always.  
      5. In case of a doubt regarding effectiveness of a solution, best to trust the product manager’s intuition. But ask “why” and don’t hold back if not satisfied with the answer.

   2. #### Solution Design

      1. If a solution involves building software, then for a “sufficiently complex” software/feature, it is a good idea to create a solution design document.  
      2. This document should contain below (non-complete list)  
         1. Overview of Why is this problem being solved.  
         2. Overview of the problem statement (Deeper problem statement details are written in requirements document or JIRA)  
         3. The approach for major state management philosophies.  
         4. The APIs (if any) used for rendering the UI and performing behaviors.  
         5. The flow of the API calls and interactions between them.  
         6. Any functional and non-functional constraints.  
         7. Known limitations of the solution.

   3. #### Coding Practices

      1. “Code is an expression of thoughts involved in solving a problem”.  
      2. **“Code is a Document of the solution created mainly for other humans to read and occasionally for computer systems to execute”**.  
      3. While writing code, engineers to follow the exhaustively documented guidelines for relevant frameworks and stacks. (example is AgroStar specific, removed)
      4. If you feel like you are writing complex code, always think twice and try figuring out a simpler approach to solve the same problem. Sometimes thinking out of the box helps\!  
      5. Code comments are *generally* not needed when the basic readability principles are followed. Unless you are writing something very niche to the domain, think twice before writing a code comment. Sometimes simplifying the logic and function names make the code self-documenting.

   4. #### Contract design

      1. UI engineers should continue building full-stack context towards the application/feature being built. Contract design can be driven by the UI engineers too depending on the context and complexity of the overall solution.  
      2. Doing a double-check of whether the contract will satisfy requirements of the solution is important. Do not blindly assume that it will happen.  
      3. Engineers to ensure that the API design best practices are followed, including naming conventions, while designing and accepting a contract.

   5. #### Estimation 

      1. “Predictability \> Quality \> Speed\*” for any P0 items.  
      2. \[\* This does not mean speed is not important, sometimes that is the most important thing, but we drive speed via product simplification, and breaking it down into meaningful incremental iterations.\]  
         \[In some circumstances, Quality \> Predictability, especially when criticality is lower or the task is exploration oriented.\]  
      3. For business to build confidence, Predictability is paramount, and being as accurate in estimations as possible improves predictability, and eventually improves quality of the software and quality of life for engineers. (because we have to worry less about last minute crunch)  
      4. Focusing on right solution design helps increase predictability by reducing the unknowns.  
      5. The more ambiguous the requirements or the solutions are, the more time we should add as a “buffer” while estimating. It also means it is always better to get clarity as much as possible.  
      6. Estimation would typically involve these steps \-  
         1. **Break down problems** to all the different pieces of logic \- i.e. what are all the areas where logical changes are needed.  
         2. List down all the things that need to be done (tasks) based on the approach as per design document.  
         3. Identify the tasks that are not clear and get the clarity on those.  
         4. Identify the tasks that need other people to work on it.  
            1. Make this list public in the right forum (and follow up on it with the people with their estimates too).  
      7. Change is fundamental to software development, even during the development cycle. But we should reevaluate and communicate the estimations when change is planned.  
      8. Always account for people factor in estimations, based on the predictability and past experiences of yourself, and others, add appropriate buffers. Yes, factor this in even for engineers in other functions.  
      9. Always account for significant buffers for integration. Typically, any solution that depends upon the backend, at least include one additional day for integration and integration dev-testing. Based on solution complexity you should increase this buffer.  
      10. Typically the product managers and engineering managers will guide you for the predictability accuracy needs of the solution. And you need to adjust the estimations to include more buffers if more accuracy is required.  
      11. Often but not always, the engineering manager or group leader will nudge you towards changes in estimates for either \-   
          1. To reduce the estimate help you grow by making it slightly above your comfort zone.  
          2. To increase the accuracy by increasing the estimate via pointing at unknowns and assumptions.

   6. #### Developer Testing

      1. The quality of the software produced is impacted by the quality of dev testing, which in turns determines the quality and capability of the software engineer.  
      2. The guideline is \- the basic and happy flows must be dev-tested and must work well, and for those flows, the developer should have confidence that even if those get deployed without any formal QA process or PM & UX review, these flows won't break.  
      3. The solution is only considered “dev-done” when it is “complete” in terms of working solution for all the exhaustive set of functional, non-functional, and design requirements that you have scoped, and you have tested it to be working by yourself. Anything missing should be called out as an out of scope for the current iteration.  
      4. The formal QA process should only be needed for covering corner cases and side effects on the parent or external systems.  
      5. The PM & UX review process should only be needed to cover the impact from the user's perspective.

   7. #### Release Practices 

      1. ##### Versioning

         1. We follow “Semantic Versioning” \[Major.Minor.Patch\] like 1.4.2 applied in the context of User Interfaces \-   
            1. Major version change when an entirely new Core application flow is introduced, or one of the Core flow is significantly altered (or breaking change for the existing behavior of the user).  
            2. Minor version change when an entirely new “feature” is introduced, or a minor but noticeable change in existing core flow.  
            3. Patch version change when a minor tweak or hotfix is released which does not noticeably change anything for the user.

      2. ##### Managing user behavior expectation

         1. Especially when Major release is happening, a communication about the change should get shared with the users, preferably on the user interface itself in a discoverable way.

      3. ##### Backward compatibility

         1. When a capability is introduced via Android/Native mechanisms, distribution to the users of which needs explicit action from users like updating the app, a concepts of “graceful degradation” and “progressive enhancement” needs to be applied while building the solution  
         2. Means, users with latest versions should be able to use the feature with highest possible capability/quality.  
         3. However, users on the lower version should be able to at least partially use the capability if the system makes it possible.  
         4. For any functionality that is critical to the core flow for the user which can not be backward compatible, appropriate messaging needs to be there for asking users to update etc.

      4. ##### Release monitoring

         1. After every release, the engineer who was involved in building the feature, should proactively monitor for and react to (if needed) \-   
            1. Any critical user feedback from the product management or user groups that something may be breaking for them critically.  
            2. Continually monitoring Sentry for any new errors that are occurring against the latest released version, and build potential fixes for them and releasing them as hotfixes.  
            3. Monitoring user behavior analytics systems like Clevertap for any potential challenge breaking the core flow, either system or UX. Consider what needs to be monitored, and proactively add logs or events for the same.

2. ### Task Allocation Practices

   1. Task allocation is a system of delicate balance between different priorities and philosophies to help teams grow, with sustainability of people, product, processes. 

   2. #### The input variables

      1. The historical context of an individual with a certain domain or product.  
      2. Team growth strategies of the engineering manager.  
      3. The solution’s \-   
         1. Complexity   
         2. Predictability requirements & urgency  
         3. Quality requirements.   
         4. Vastness  
         5. Coordination needs.  
      4. The individual’s persona, profile, growth objectives.  
      5. The individual’s comfort level towards the nature of a solution.  
      6. The individual’s compatibility working with certain groups.  
      7. The individual’s own growth ambitions.  
      8. The individual’s recent workload.  
      9. The individual's specific personal situations and flexibility needs.  
   3. The goal of the effective task allocation system is “to sustainably deliver good quality software, predictably, as a team, while maintaining a good stakeholder experience”  
   4. When “highly predictable, ***urgent*** solution” is needed, typically the individual with the most historical context towards the domain will get allocated the task, and a right mentor may help and nudge them whenever needed.  
   5. But in many cases the requirements are more skewed towards **quality** and exhaustiveness, and not urgency. In such cases, the heuristics would be \-   
      1. If the individual demonstrated the ability to build good quality solutions.  
      2. The historical context in the domain *may or may* *not* be considered.  
      3. If the team growth strategy needs to build context of the product to additional individuals.  
      4. If the individual has expressed interest in working with that domain.  
   6. If the solution is skewed more towards building a **complex** but long lasting solution, then the heuristics would be \-  
      1. Past experience in building complex solutions.  
      2. The manager’s strategy towards helping individuals grow in roles / positions & elevating via working at levels beyond their comfort zone.  
      3. Typically, either a senior engineer, or a potential senior (but mature engineer) will work on these complex solutions.  
   7. For Simple yet **Vast** solutions, the heuristics would be  
      1. The individuals with past experience in building vast solutions.  
      2. The individuals with the most consistent planned continuous availability for the near future.  
   8. For **simple**, trivial solutions, the priority would be to build the context with more individuals, and if everyone has similar context, the person with least professional experience will pick it.  
   9. Special consideration \- recent work-load \- if any individual completes a solution of either a *vast or complex* feature, the next one to two tasks would be simpler and trivial in nature. This gives a cooling off period and sustainability, balance.  
   10. Special consideration \- individual compatibility with groups \- in some rare occurrences if compatibility issues are not easy to fix, we would try to re-shuffle the allocation. But it is highly advisable to fix those issues by either direct discussion or managerial interventions as early as possible.  
   11. Special consideration \- temporarily impacted individual capacity, availability, capability \- in such circumstances, the tasks which require least amount of coordination with peers and other functions, along with simple and well defined solutions are considered.

3. ### Engineering Quality Management Practices

   1. “Good engineers build good quality solutions”. Quality of the software/ solution is the best way to understand the capability of the engineer.  
   2. The prioritized order that defines of Software Quality, assuming it is functionally complete (i.e. Dev Testing done as per above doc) :   
      **User Experience & Usability \> Reliability \> Performance \> Supportability**  
   3. Note that this does not talk about Code Quality or Architecture Quality *directly*.  
   4. So whenever we are developing software, it is critically important to internalize that User Experience/ Customer Experience/ Usability. Nothing else comes even closer. **Our users don’t care if we have built software using React or Flutter or jQuery. Also, our users don’t care if it is a Backend issue or UI issue.** Tech stacks are just means to the end i.e creating a good user experience.  
   5. Also it means issues even in other layers of the stack need to be gracefully handled. UIs should not “crash” no matter what goes wrong. Defensive coding practices are important to be followed.  
   6. There are standard formatting guidelines and practices for media and content. For example, currency formatting. It is expected that engineers will stick to these formatting practices (by using standard library functions). Also, engineers are expected to follow basic grammar standards for interfaces in the English language. For non-english languages, engineers can take help from copywriting teams.  
   7. The UX designs should be considered as a guideline towards the expected software. Typically in case of a direct to consumer product, the expectation would be to more closely match the design. However, iterations for simplification are acceptable. Overall, if the designs are not consistent with existing products, engineers are expected to revise it to make it consistent.

   8. #### Reviews 

      1. To improve the quality of the solution, a continuous *Solution Review* process is implemented and followed. Peers as well as group leads are expected to suggest improvements for the solution if and when needed. But the responsibility of getting it reviewed is on the individual not on the reviewer.  
      2. Similarly, *Code Reviews* are implemented to improve the consistency, style, readability and maintainability of the code that is written to build the solution. Group leaders will publish guidelines for coding for the particular stack, which will serve as a baseline for the code review. Above and beyond the guidelines, pragmatic decisions based on past experiences to be incorporated into the reviews.  
      3. Code reviews have these goals \-  
         1. Improving Quality of the codebase, including readability and maintainability.  
         2. Making it easy to onboard a new member to the coding style of the existing system.  
         3. Code reviews acts as a tool for engineers/ leaders with a high level of expertise and context regarding the programming/ building of the system with engineers having less context.  
      4. Part of the review process is to review the UX as well, by the group leader or peers, so the UX/PM feedback cycle is reduced.  
      5. **Opportunity to do Code Review is “earned” right** \- that is, any engineer who is consistently getting just a few comments as part of code review will earn the right to do code review for others. This earned right is not directly linked to the seniority level in the org, but senior engineers are expected to earn this right more quickly.  
      6. However, code reviews should not become ritualistic and should not be applied without considering the context. For example, a super quick MVP built by an individual may not need to be code reviewed for the first release as long as the individual has consistently demonstrated quality in such initiatives.  
      7. Typically, any major business critical software built in a distributed fashion (i.e. with 2+ engineers) will have code reviews.

   9. #### Stakeholder Experience

      1. Building good quality solutions is just one part of excelling in the engineering domain, the other significant part is about what is the experience we are building for our stakeholders, these can be our peers, fellow product managers, Quality assurance folks, leads and managers, among others.  
      2. Always remember, “Do unto others as you would have them do unto you”. Ask yourself, If you were in their shoes, would the experience you are creating for them be pleasant? If not, always retrospect, and seek guidance and direct feedback. Periodically connecting with stakeholders for feedback does wonders.  
      3. EM will independently connect with key stakeholders for the team members to seek feedback on stakeholder experience created by the team members, and figure out ways to improve it.  
      4. In the long run, remember this quote \- “People will forget what you said, people will forget what you did, but people will never forget how you made them feel.”

4. ### People Management Practices

   \[Disclaimer \- AgroStar specific. Removed. \]

   1. When it comes to people management, a fairly self-organized, common-sense driven approach is recommended.

   2. #### Trust

      1. Trust is the key factor. It is assumed that everyone in the team is **working with the best intent.**  
      2. Everyone is aligned towards common high level goals and values.  
      3. Further, **everyone** we work with, members of other functions, and stakeholders, will also **have the best intent** while working with you.  
      4. Essentially, trust is the basic assumption & foundations for the people management practices.  
      5. A non-complete list of examples of what can break trust \-   
         1. A conscious yet false communication of status or completeness of the tasks.  
         2. As a full time employee or full time contractor or intern, working with multiple organizations / or contracts. \[This fundamentally breaks trust by misaligning task alignment as well as focus\]

   3. #### Work timings

      1. Software Engineering is a fairly creative field, as such, we strongly believe in measuring the outcome, not the input or timing.  
      2. Having said that, it is highly recommended to have significant hours of overlap with the group you are working with for coordination and discussions.  
      3. On remote working days, we don’t need to specifically create a static work schedule. Team members are supposed to figure out the most efficient working hours for themselves without hurting the ability to coordinate.  
      4. On work from office days, team members are supposed to have a good amount of overlap for in-person interactions.  
      5. Key rule of thumb while especially picking non-regular work hours is \- whether those hours are significantly multiplying your productivity due to focus time. For example some people find it very productive to work in very early mornings. That is encouraged, as long as you are not significantly disrupting the coordination with other team members.  
      6. In order to make flexible work schedules more effective, an “async-first” work style is recommended. Where many of the coordination happen via written communication that can be read, processed, replied at any time, rather than real-time. Again, a fair amount of pragmatism and common sense needs to be applied. Things that are best done in sync, should be done in sync. For example PM/UX reviews on UI.  
      7. Engineers are expected to have fair balance for their work schedule by effective estimation of tasks, and including proper buffers, so that they don't overextend themselves. Any engineer who “has to” work for extended hours is either inefficient or inaccurate at estimation. There is NO “glory” in working for extended hours. Having said that, as mentioned above, we won't discourage people from working late on their own out of their passion or work style. The key is that anyone should not feel that “they have to work late and that's the only way to finish XYZ”. Any such instances should only be treated as a rare exception and have to be notified to the manager / leader.

   4. #### Complimentary Offs

      1. The purpose of holidays and weekly offs is to decompress and maybe enjoy with people and systems close to the individuals, and maybe pursue recreational or learning or leisure activities.  
      2. It is strongly advised NOT to work on weekends or holidays. (Again, no one is stopping anyone to work on something out of their own passion)  
      3. Complimentary offs are only considered in cases of rare exceptions where people need to extend over holidays and weekends due to critical business needs. “Weekend / holidays working and then comp off” MUST NOT be a “plan”. It has to be treated as a rare exception.  
      4. Using “complimentary offs” as a work schedule flexibility mechanism is not recommended, only exceptionally will be approved.

   5. #### Leaves 

      1. (This section is too specific to AgroStar, still I want to convey the philosophy, hence sharing without significant changes) Personal planned and unplanned leaves are an essential part of creating a sustainable, satisfying, fulfilling work environment.  
      2. Team members are expected to be self-organizing about taking leaves \- i.e. thinking of the leave balance, planning and applying leaves.  
      3. Generally, applying leaves in system and just informing the manager and key stakeholders would be enough. Managers or leaders will not be “not approving” paid / balanced leaves unless a rare or extreme circumstance occurs  
      4. However, team members are expected to be responsible and plan well while taking leaves \-   
         1. While working on a task, finish the task (including release and monitoring) before going on leave.  
         2. Ensure proper handover of recent work is given to the peers before going on leave.  
      5. Casual leaves \- it is encouraged to take casual breaks and leaves occasionally, even without a reason, just to relax. The reporting manager would nudge the team member to take breaks/leaves if such a need occurs. As a suggestion from experience, such a leave is most effective when taken in the middle of the work week, i.e. Wednesday.  
      6. Medical leaves \- it is perfectly fine to take leaves for any physical or psychological illness, distress, recovery, treatment, planned or unplanned. Urgency & mechanism of informing such leaves does not need to be systematic or formal. In lack of such notification, at times the manager will try to connect and check just to get the idea. Confidentiality in such cases will be treated with priority.  
      7. Sabbaticals and long term unpaid leaves \- Such leaves need to be discussed with manager, HRBP, department head, and are subjected to approvals.

5. ### Performance Management & Appraisal Practices

   1. Performance Management is a continuous process, not a one-off event.  
   2. Every team member would have certain roles and responsibilities defined as part of their goal plan. Along with this, the engineering manager would publish a general, team wide accessible document highlighting the expectations from different roles. (Example of a goal template for a specific year (example is AgroStar specific, removed) 
   3. Typically the engineers are expected to at least meet the expectations from the position/ role that they have.   
   4. The Engineering Manager is expected to share feedback on performance in every opportunity possible throughout the year (considering practical situations too). Earlier the feedback is shared, the better.  
   5. The Engineering Manager is also expected to call out and celebrate specific achievements by the team members, timely. (closer to the event the better)  
   6. Typically the engineering manager will share the cases of outstanding performance with the other EMs and department head / top management whenever practically possible.

   7. #### Performance & Compensation Review Process 

      1. AgroStar Specific, Removed

   8. #### Promotions

      1. Typically when an engineer is consistently exceeding the expectations from the current role, and at least meeting the expectations from the next role, for a significant amount of time, a promotion MAY get recommended.  
      2. However, this is NOT a rule. Promotions depend upon a lot more factors including budget, org level positions, balance, appetite, and other factors. Promotions are subjective in nature.  
   9. Along with performance, the behavior and style of interaction is expected to be either coherent with organizational and team values or can be constructively different.  
      **“The culture of the team is defined by the worst behavior that the team tolerates”**  
   10. Cases of non-performance/ not meeting expectations are expected to be handled in a timely manner also considering the practicality of the situation. As a rule of thumb, **if** **either non-performance or behavior of the individual is leading to a negative contribution in the team, it is not acceptable.**  
       \[A negative contribution is defined as \- if the presence of the individual in the group or team is leading to less efficiency/ morale/ productivity of the team as compared to if that individual was Not in the group\]

6. ### Team Building & Cohesion Practices

   1. The basic principle of any team is “**The Whole is Greater than the sum of its parts**”   
      A well built, jelled, cohesive team is supposed to significantly over perform than the extent at which the individuals will perform if they were not part of the team.  
   2. Along with Trust (as discussed above, along with the principle of assuming the best intent from others), **Respect** is a key factor while building the team.  
      It is critical for us to understand that every individual is part of the team because they are contributing to the team in a unique way.  
   3. It does not matter what their position, background, age, gender, etc. Every individual is unique, different, and brings positive contribution in their own ways. Individuals should not objectively claim to be “generally better than others”, although they can be doing specific things in different and better ways than others. A public confrontation of such is not encouraged either by individuals or group leaders.  
   4. Individual differences including personality, opinions, personal values, are respected, and if possible encouraged to be shared. We, as individuals, and as a civilization, EVOLVE & grow because of the differences and uniqueness we have as humans. A monotonous group of individuals with the exact same thought process does not evolve. We as a team will evolve when we respect our differences.  
   5. It is highly encouraged for individuals to socially bond with one another outside core work relations. Any number of things (non-complete list), like watercooler conversations, outing, team dinners, team building activities, life-timeline, values connect etc can be conducted. At times, these can be organized or nudged by group leaders, or HRBPs etc, but individuals and groups can organize on their own too. Usually, participation in such events is voluntary, but highly encouraged. The group will ensure to make these events as much comfortable as possible for individuals with different personality styles, including individuals who are introverts. Individuals should feel free to not participate in specific activities, and no one should feel forced to participate in something that they had to because they attended the activity.  
   6. In casual discussions, generally controversial or sensitive topics are best to be avoided. Individuals should nudge each other if the topics being discussed are sensitive or not comfortable.  
   7. Guidelines for dating and relationships/partnerships among individuals in the team will follow the organizational guidelines for the same.  
   8. In general, building an inclusive, diverse team is considered important, and efforts will be made to ensure that.  
   9. Individuals are encouraged to “understand” each other, and support each other in ups and downs. If someone is struggling with something on a personal or professional front, supporting them as well as discussing the same with the group leader is encouraged. Group leader is supposed to extend help/ or try helping the individuals or take help from the org if relevant, for the same. (Helping others does not mean over-extending oneself or burning oneself out. Also it is important to notify the team leader if you are picking other tasks.)

   10. #### Celebrations

       1. Team members and leaders should find opportunities, like achievements of the team members, major releases, personal occasions like birthdays, work anniversaries, among others, to hold celebrations for the same, either inside the office or outside.  
       2. In the case of celebrating specifically for an individual, it is a good idea to think about their individual preferences and choices to create a 7 star experience for them\!  
       3. Generally, based on the circumstances, the celebration will include the biggest possible group who is relevant for the celebration, however due to lack of availability (esp not being in Pune) leads to impacting the timeliness of celebrations, the general guideline is the celebration should still be held with at least “core” participants of the celebration. A larger event can always happen later.

   11. #### Rewards & Recognitions

       1. Removed details as it is too specific to AgroStar

7. ### Team Hiring & Recruitment Practices

   1. Hiring is one of the core responsibilities of an Engineering Manager. *It is not the responsibility of just the recruiters*. Recruiters are there to Assist the engineering manager, not vice versa. Means EM must take the ownership of the process.  
   2. It is suggested that EM should write the job description that is being hired for.  
      The job description should \-   
      1. Set context about the organization.  
      2. Specifically call out the specific job responsibilities concisely.  
      3. Should have a list of must haves and good to haves.  
      4. Should NOT be picked from generic templates or Gen-AI.  
   3. EM should post about the position in publicly accessible social media site, like LinkedIn etc, and spread the word via social media and tech community channels like Whatsapp or Discord or similar.  
   4. EM should spend time in responding to messages to applicants/candidates, and reach out to potential strong candidates. Recruiter would assist here.  
   5. EM to shortlist candidates based on the potential for conversion. Recruiter to assist here.  
   6. The interview process guidelines are independently documented here (AgroStar specific, removed) Vary significantly based on the position. However, along with skills and potential, significant importance must be given to culture fit and behavior.   
   7. Current and potential senior engineers in the team will get involved in the interviewing process. It is an important responsibility to be trained for \- how to conduct good interviews and build good intuition towards selecting the right candidate based on the org needs.  
   8. After a candidate is selected, EM can reach out to candidates to get them excited about joining, also solving any potential concerns regarding the same.  
   9. EM should be involved in reference checks.  
   10. In the team, it is highly encouraged to share references from the network. And referral bonuses will also apply as per the org policy.  
   11. However, referred candidates will be shortlisted based on the common criteria that other candidates have. Further, to remove the biases, the referrer would not be part of the interview process of the candidate.  
   12. Typically when there is a significant gap between the recommendations in different interviewers, a “debrief” meeting would be conducted, where a discussion and conclusion will happen based on strengths and weaknesses of the candidate and hiring decision is made. A leader can choose to “champion” for a potential candidate being debriefed, i.e. even with different views, the leader would be confident about the candidate’s potential and can move the needle towards hiring the candidate.  
   13. Rest of the organizational practices regarding hiring to be followed as-is.

8. ### Learning & Development

   1. Learning & Development investment creates a path of engineer’s professional growth, helping individuals grow into world-class engineers and problem solvers.  
   2. Any systematic as well as impromptu investment in learning is known to yield very good returns.  
   3. While “task based” learning is the best way to learn certain professional skills, and we actively work towards creating such opportunities among team members (by allocating tasks outside the comfort of the individuals), such learning tends to have “knowledge gaps”, further, growing an individual professionally needs more things than just completing tasks in engineering. Hence, EM will run key programs to promote Learning throughout the year.

   4. #### Learning & Development Programs

      1. For the UI Engineering team, relevant “domains of expertise” are defined.  
      2. Every engineer will be responsible for making themselves more skilled in these domains of expertise over time.  
      3. Team members are encouraged to spend at least one hour per week in learning & development activities  
      4. Active participation in such programs is linked towards an individual's performance review, with certain weightages based on role.

   5. #### Domains of Expertise

      1. Application Development  
      2. Application Architecture & Design  
      3. User Experience & User Interface Design  
      4. Product, Program, Business Management  
      5. Communication Skills

   6. #### Activities

      \[This is an incomplete list of suggested activities, program is not to be limited to these.\]

      1. ##### Engineering reader’s club

         1. A voluntary book/ podcast/ blog/ video course discussion group, which can periodically meet together to discuss certain topics that help with engineer’s professional growth and development.  
         2. Reading/ book based career vision setting and guidance, by aligning specific book reading based on the role.

      2. ##### Public Speaking & Writing 

         1. individuals are encouraged to speak and write about their topics of interest and expertise  
         2. EM and team members will create such avenues, whether it is inside the org or outside publicly.  
         3. Team members are encouraged to speak at meetups and conferences.

      3. ##### Mentorship

         1. Mentoring Others \- “teaching is the best way to learn”  
         2. Finding and following a mentor \- this can be outside the team and org boundary, individuals are encouraged to find mentors to learn from.  

### Epilogue

Original Epilogue - "This document sets guidelines for working of the UI engineering team. It should serve as a general guidance for anyone inducted to the team, as well as a compass for everyday decision making in the team.  
It is important to note that 'guidelines are not rules'. A good amount of pragmatism needs to be applied while following these guidelines.  
This is a live document, and the author will try to keep it updated based on org needs, industry changes, and team needs, with a versioned changelog."
This is based on what works very well for AgroStar's frontend engineering team. Feel free to adapt this to what suits best for your teams!

Cheers\!

Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

