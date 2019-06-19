DRAFT DRAFT DRAFT DRAFT DRAFT

# Technology Budgeting and Oversight Playbook

## Rethinking budgeting for custom technology


By [Robin Carnahan](mailto:robin.carnahan@gsa.gov), [Randy Hart](mailto:randy.hart@gsa.gov), and [Waldo Jaquith](waldo.jaquith@gsa.gov)

---

## Table of Contents

* **[Introduction](#introduction)**
	* [Who This Playbook Is For](#who-this-playbook-is-for)
	* [Moving Control Back to Government](#moving-control-back-to-government)
	* [Who We Are](#who-we-are)
* **[Basic Principles of Modern Software Design: Prerequisite Concepts](#basic-principles-of-modern-software-design-prerequisite-concepts-)**
	* [Human-Centered Design](#human-centered-design)
	* [Agile Software Development](#agile-software-development)
	* [Product Ownership](#product-ownership)
	* [DevOps](#devops)
	* [Building with Loosely-Coupled Parts](#building-with-loosely-coupled-parts)
	* [Modular Contracting](#modular-contracting)
* **[Software Budgeting Plays](#software-budgeting-plays)**
	1. [Think about risk in a new way](#think-about-risk-in-a-new-way)
	2. [Procure software services, not software](#procure-software-services-not-software)
	3. [Hire tech talent in-house](#hire-tech-talent-in-house)
	4. [Minimize the cost of change](#minimize-the-cost-of-change)
	5. [Limit total spending](#limit-total-spending)
	6. [Limit contract sizes](#limit-contract-sizes)
	7. [Expand your vendor pool](#expand-your-vendor-pool)
	8. [Fund systems, not monoliths](#fund-systems-not-monoliths)
	9. [Measure success based on iterative outcomes, not project milestones](#measure-success-based-on-iterative-outcomes-not-project-milestones)
	10. [Require demos, not memos](#require-demos-not-memos)
	11. [Share your software](#share-your-software)
	12. [Budget for software as an operational expense]()
	13. [Ask technical questions of agencies]()
* [Appendix: Questions to Ask](#appendix-questions-to-ask)

---

## Introduction

Only 13% of large government software projects are successful.<sup id="reference-1"><a href="#footnote-1">1</a></sup> Government's software procurement process is broken.

Government is increasingly reliant on modern software and hardware to deliver essential services to the public. The success of any major government initiative depends on the success of underlying software infrastructure. Federal, state, and local government agencies all face budget and staffing constraints while struggling to modernize legacy technology systems that are out-of-date, inflexible, expensive, and ineffective.

When accessing government digital services, the American public deserves access to the same world-class technology that's available in the commercial marketplace. As government leaders, we must be good stewards of public money by demanding easy-to-use, cost-effective, sustainable digital tools for use by the public and civil servants.

Acquiring and maintaining modern technology tools in a cost-effective and sustainable way is a serious challenge faced by every level of government. Public trust in government depends on meeting this challenge.

To address this, government must first overcome a number of other related challenges, including:

- Simultaneous need to use, maintain, and modernize complex, outdated legacy systems
- Locked-in, proprietary, legacy, commercial arrangements that can create technical and financial barriers to improving digital service to the public
- Risk-averse, siloed organizational cultures, and budget cycles that inhibit the adoption of modern, agile software design practices
- Hiring, staffing, and other resource constraints that have led to an overreliance on outsourcing technology projects and decisions

The recommendations in this playbook are premised on these guiding principles:

- The public deserves access to world-class technology when using government digital services
- Taxpayers should not have to pay more than once for the same software tools and systems
- Technology, policy, and user needs change often, so government software tools should be designed to make it fast and cheap to respond to those changes
- The public is best served by a robust and competitive market for private-sector technology services, and that ecosystem is best supported by prioritizing open standards, interoperability, and modular IT systems
- User needs should be at the center of everything
- Privacy and security must be baked in from the beginning
- Interoperable and open are better than monolithic and proprietary
- Government is responsible for its mission of delivering services to the public and must take ownership of the technology systems designed to do that job — neither the mission nor the technology used to deliver on the mission can be effectively outsourced.

### Who This Playbook Is For

This playbook is designed for executives, budget specialists, legislators, and other "non-technical" decision-makers who are tasked with funding or overseeing government technology projects. It provides guidance about the basic principles of modern software design and procurement with the goal of helping leaders better set major software projects up for success by asking the right questions before funding projects and identifying the right outcomes to use to judge the project's success.

This is written specifically for procurement of custom software, but it's important to note that commercial off-the-shelf software (COTS) is often custom. Software vendors often promote their offerings as COTS, knowing that it will need to be modified to function within each government environment. When COTS is modified in _any_ way, it becomes custom software, at which point the bulk of the advice in this playbook applies. On the other hand, little of this advice applies to Software as a Service (SaaS), because SaaS is inherently not customizable.

### Moving Control Back to Government

Government has outsourced increasing amounts of work to technology vendors over the past several decades. Although each of these changes were done for sensible reasons, the cumulative effect is to leave government with minimal oversight and control over key portions of its mission, a hapless spectator witnessing not even the actual work being done, but merely vendors' descriptions of the work.

If a government database designed to track the welfare of at-risk children doesn't work, or the unemployment database crashes and people don't get their checks, or the DMV has to fall back to paper after their terminals stop working, it's government that gets the blame. It's the government, not an outside vendor, that is responsible for providing those core services, regardless of the cost. Outsourcing the work of creating the technical infrastructure to private-sector experts provides a temporary façade of security, but the reality is that if a technology project fails (or is over budget or behind schedule), it's the _governor's_ name that often ends up in the newspaper headlines.

There is an alternative: shift a substantial amount of control back to government and return government to the position of ensuring the success of its mission.

In this approach, government — in partnership with an outside vendor — works with end-users of the planned system to determine what their needs are and how to meet those needs through software. Government and the vendor create a backlog of features to be added to the software, and the vendor uses that as a long, detailed to-do list, which is constantly modified in response to evolving needs. Every couple of weeks, the completed work is handed over to government for government inspection. There, its audience can start to use it, and government and the vendor can see if they have successfully addressed the users' needs. It's this tight feedback loop — research, develop, deliver, repeat — that government must own, because it is the best way to ensure that users get the software tools they need and that government gets what it's paying for.

The key to this approach is understanding that software development is not a mysterious and incomprehensible magic, but instead a straightforward trade practiced by millions of Americans that is easily grasped and even mastered by government employees.

The process by which government has been procuring custom software for the past few decades does not work. We know it doesn't work. The model described in this playbook does work. We know it works. Change might feel risky, but what's _really_ risky is how we're procuring software right now.

### Who We Are

We work for [18F](https://18f.gov/), the federal technology team within the [General Service Administration](https://www.gsa.gov/), partnering with clients in federal, state, and local governments to teach them how to procure custom software quickly, efficiently, and successfully. Our team, collectively, has many years of experience in government procurement, software development, and state-level elective office.

In work funded by GSA's [10x](https://10x.gsa.gov/), over the course of a year we met with state legislators, legislative fiscal staff, state budget officers, contracting officers, and gubernatorial policy advisors. This playbook came of learning from and teaching hundreds of people from dozens of states. We're grateful to the many people who contributed their time and knowledge throughout that process.

## Basic Principles of Modern Software Design: Prerequisite Concepts

Every technology project necessarily requires teams with unique technical experience. However, a project's odds of success will improve if the non-technically trained government leaders tasked with funding and overseeing digital modernization projects understand six basic concepts of modern software development: **human-centered design**, **agile software development**, **DevOps**, **building with loosely-coupled parts**, **modular contracting, and product ownership**. You don't have to be a technologist to understand these general concepts. Once you get them, you can't be snowed by jargon or buried in technical detail — these are tools you can wield to fully understand any software project.

### Human-Centered Design

All software development should be centered on the needs of the software's actual end-users, the specific humans who are expected to use it. These may be applicants for benefits, call center workers, case workers, or any of innumerable other groups. In human-centered design, all work is in the service of those end-users' needs. That work is identified and prioritized in close and regular collaboration with end-users, and is informed by (but not subservient to) any technical constraints. The technical team and end-users regularly review the work, as it is being performed, and the development work is not considered finished until those end-users agree that their needs have been met. Designing with and for users reduces project risks by ensuring the software is solving users' problems.

In short, human-centered design says to do what the actual, relevant humans need, and not what their boss's boss _thinks_ that they need.

### Agile Software Development

Detailed, long-term plans for major, custom software projects have long been the norm in government. But, sadly, they are never correct. It's time for government executives and budget officials to stop asking for them.

Planning an entire project upfront is known as "waterfall" development. Imagine planning a month-long family vacation of driving around the United States. Under waterfall, this would entail planning up front each day's agenda, including the route driven, booking every hotel room and deciding on every meal in advance, pre-buying tickets for admission to attractions, etc. This would never work because things change, unexpected options come up, and no rational person would want to lock in every decision at the start of the journey when they don't know what the journey holds. Instead, most people would map out the general route to be taken and plan a few major stops — the specifics would be sorted out as they progressed along the way.

"[Agile software development](https://agile.18f.gov/)" refers to using this trip-planning methodology for building and modernizing software systems. Instead of relying on years of costly planning and "requirements gathering" before beginning to write actual software, agile development projects are planned only in broad strokes, with a well defined description of the overall project goal and a strong preference for _just getting started_. A small, empowered, self-motivated team (usually 5-9 people, including developers, product managers, user researchers, writers, and/or security experts) is dedicated to accomplishing that goal, using human-centered design, working in two-week cycles to deliver some actual working software.

On day one, the team plans only what they'll do for the next two weeks. Each task they'll work on is in the form of a "user story" — an individual need that users have.<sup id="reference-2"><a href="#footnote-2">2</a></sup> The collection of user stories to be worked on is called the "backlog." The team works on a selected group of user stories for two weeks and, at the end, the team reviews the work that they did, tests it with end-users, and then plans the next two weeks by pulling more user stories from the backlog. Repeat. Each of these two-week cycles is referred to as a "sprint."

In the beginning, the software they produce may not seem like much (and may even be replaced by something else later), but it will gradually and systematically inform the project's technical approach and help the team sensibly integrate the project into an agency's existing legacy system.

Functioning software is delivered at the end of each sprint, without exception — fully-tested, fully-documented, ready to be used. In this way, value is delivered constantly, until the software is good enough to be deployed for broad use. The team continues to work until they accomplish all of the goals or they run out of money, whichever happens first.

All code is owned by government and delivered to government at the end of each sprint. The vendor owns nothing. They are paid for their employees' time, not for software.

By coupling agile with human-centered design, a development team can constantly iterate toward solving the needs of end-users in ways that would have been impossible to learn about up front.

Last year the U.S. Department of Defense's Defense Innovation Board released the draft document "[Detecting Agile BS](https://media.defense.gov/2018/Oct/09/2002049591/-1/-1/0/DIB_DETECTING_AGILE_BS_2018.10.05.PDF)," which provides a useful synopsis of agile practices, and a series of questions to help non-technical leaders understand whether those practices are being followed.

### Product Ownership

Taking back ownership of government software projects requires government teams to focus on outcomes, not outputs. This means shifting from some of the traditional Program Management Body of Knowledge practices to a product-oriented mindset.

The product owneris the key person for any software project, and _must_ be a government employee. The product owner works with users, stakeholders, technologists, and the vendor to envision the direction for the product, with an eye toward delivering value to end-users as quickly as possible. They iteratively prioritize and define the work for the product team, as part of the agile process. They measure progress against clear performance indicators, and communicate with stakeholders and the cross-functional team that is building the product.

The product owner should know the users of the system, the business (for example, Medicaid insurance or DMV services), and policy constraints. They don't need to be strong technologists.

A strong product owner ensures that the vision is clear, the strategy is clear, there is space for teams building the software to learn, and that they are building or buying the right thing to incrementally show value to users. They prioritize ruthlessly to ensure that the product serves user needs, and that activity and attention is focused on the highest-priority needs. This positioning ensures that the product owner understands everything that the development team is doing and that the needs of government are fully represented.

This is different than typical project management in government IT. The product owner won't have Gantt charts or a detailed 5-year plan. But they will have a vision for the outcomes that will be delivered to users, and have a path to executing.

### DevOps

Historically, the teams building software have been separate from the teams that manage the IT infrastructure that hosts the software. A vendor might spend years building new software, and then a government IT team (or a vendor filling that role) might then require many months of work to get that software to function correctly on their servers. This is usually accompanied by frustration and finger-pointing, and can lead to project failures. To address this, government agencies often insist that the vendor building the software also host it indefinitely on the vendor's infrastructure, which has the effect of ruling out most software vendors (who are not in the hosting business), and creating vendor lock-in with its associated high prices. This approach is not working.

DevOps is the practice of coordinating the work of the two groups to automate the work that goes into testing software and moving it to a live server where people can use it — merging software **dev**elopment and system **op**erations. Under DevOps, testing software quality is automatic, testing software security is automatic, merging multiple developers' work is automatic, and moving completed software to servers is automatic. (The incorporation of security testing in DevOps is sometimes labeled as "DevSecOps.") Developers cannot merely hand their completed work to the system operations team declaring "hey, it works for us" — they are responsible for their code working properly.

## Building with Loosely-Coupled Parts

Large, complex software projects tend to collapse under the weight of administration. Each new member added to a project team increases the complexity of the entire team's interactions. The contributors need to coordinate carefully to avoid conflict between their efforts. No single developer can understand the entire system that they're contributing to, necessitating new supervisory roles like "software architects," with whom developers must check before doing any work. As a team grows, they're forced to spend increasing amounts of time managing the project, and decreasing amounts of time actually doing the work.

To avoid this fate, it's smarter to break large projects into a handful of small, quasi-independent software projects. In this model, each component communicates with other components through simple, modular standards, so that any one piece can be swapped out at any time. Instead of building a monolith that everybody will lament in a few years, you build a little ecosystem, in which each piece can be upgraded and modified easily, as changing needs will demand. Each component is maintained by a single agile team, which documents the component's application programming interface (API) — the grammatical rules that other components can use to communicate with it. The teams' need to coordinate is minimal, because they can simply follow the API documentation for the other components that they need to interface with.

When each component uses abstracted APIs (think of them as common standards for using that technology), this is known as using "[service-oriented architecture](https://en.wikipedia.org/wiki/Service_oriented_architecture)" (SOA). This is the same as the concept of "interchangeable parts" that made the industrial revolution possible. Standardized couplings are the underlying concept behind cloud computing, electrical outlets, USB, Legos, trains, and countless other modern products and practices.

Building IT systems using loosely coupled parts, connected by open and available APIs, is the "magic bullet" that allows for flexible, sustainable systems that meet user needs and cost less over time.

### Modular Contracting

By combining human-centered design, Agile, product ownership, DevOps, and building with loosely-coupled parts, it's possible to break up a large, risky contract into a handful of smaller contracts. A contract should be small enough that the agency will have no compunction about changing functionality or firing a non-performing vendor. The rest of the vendors will continue working, so the total loss of velocity will be minimal. A new vendor should have no difficulty taking over for the old one, since the old one was delivering completed, documented, tested software every two weeks. Small contracts may come in under your state's simplified procurement threshold, meaning that agencies can write an RFP, publish it, and award a contract, all within 90 days or so.

There are vendor teams that specialize in working as we've described here. As a rule of thumb, an agile development team of 5–9 people costs between \$1–2M/year, depending on their geographic location.

This approach will require coordination and buy-in from your procurement teams. Procurement personnel are often accustomed to the traditional approach of outsourcing IT projects: one large procurement based on lengthy RFP documents, asking for lengthy proposals and outdated, waterfall-style certifications and qualifications from vendors. Generally, vendors that use agile, user-centered methods don't have any idea what "CMMI" or "EVMS" is — such standards are no longer considered best practices for creating flexible and cost-effective software systems. This is a barrier to entry for many of the vendors that might be new to government and don't want to expend all of the resources required to write a proposal.

## Software Budgeting Plays

### Think about risk in a new way

Over the past several decades, government agencies have turned away from using in-house staff, relying on outside vendors to build their mission-critical technology. Those decisions were based on rational trade-offs that seemed like lower-risk options, often driven by limited capacity, and knowledge of internal government staff, and promises of cheaper "off the shelf" tools offered by government contractors

Since then, we've learned the hard way — exhibit A: the Affordable Care Act and Healthcare.gov — that while government can easily outsource the work of creating new technology systems, it cannot outsource the risk of failure.

A smarter approach to lowering risk for technology projects is for government agencies to retake control and responsibility for projects, by setting clear expectations about human outcomes and technical standards, related to data security, use, interoperability, monitoring, and evaluation.

The need that's being addressed with a budget request is not a technical problem — it's about fulfilling the agency's mission, and technology is simply a means to that end. It's not a technology project, it's a housing project or a Medicaid project or a licensing project. The risk isn't that technology will fail — the risk is that the agency will fail to fulfill its mission because of a technology problem. Technical knowledge is cheap and abundant, but knowing how to run a state agency is a rare and valuable skill. Government must embrace and own that risk of failure, recognizing that technology vendors are a fungible means to that end.

#### Checklist

- □ The project has a dedicated, empowered product owner who is an employee of the mission agency — not a contractor, and not an employee of the state's IT agency
- □ Stakeholders recognize that the existing approach (waterfall development) fails the majority of the time, and that moving to agile development and modular procurement is, in fact, significantly less risky
- □ Stakeholders regard outside vendors as interchangeable tools to accomplish a goal, rather than as the "owners" of a project or its outcome

#### Key Questions

- Are there identified and trained government employees (not contractors) that will serve as dedicated and empowered product owners to set direction, prioritize, and oversee the work of the development team?
- Is there a chain of support for this new approach within the agency, all the way up to the governor's office, central IT, legal and procurement offices, and over to the legislature? Are any of those stakeholders able to block adoption of this new approach? If so, what is the path to escalating issues, ensuring alignment, and preventing those internal blockers from putting the project at risk?
- What is the agency doing differently to take responsibility for leading the project and owning the results, rather than trying to outsource risk to a vendor through the contracting process?

### Procure software services, not software

Buying custom software is different than buying IT hardware. Don't think of procuring custom software as procuring a _product._ Instead, think of it as procuring a _service_: the service of a team of developers performing work as prioritized by the product owner. This reframing leads to a completely different approach — a much simpler approach — to the RFP and to the contract, and is an important distinction for contracting officers.

The RFP should describe the overall goal of the work, and should include a first attempt at a product backlog, put together by the product owner — a list of user stories that the work is likely to include, clearly labeled as not representing the scope of work, but instead providing an idea of the sort of work likely to be performed. The RFP should acknowledge that there will be constant change to the work based on product decisions and ongoing user research.

The RFP should use a Statement of Objectives, rather than a Statement of Work — that is, it should state the objectives of the project, rather than the specifics of a product that the vendor will produce. Using a SOO instead of a SOW eliminates "change orders" from vendors, because the scope of work is whatever the team is directed to do. (If an ostensible agile vendor mentions change orders, that's a red flag.) Change is expected, and it's easy to change software when it's built in modern ways.

To ensure vendors deliver work that meets the needed technical specifications, it is important that the RFP include a Quality Assessment Surveillance Plan (QASP) that is appropriate for agile development methods, requiring that the software be inspected at the end of each sprint to ensure that it is tested, secure, accessible, documented, and deployed.<sup id="reference-3"><a href="#footnote-3">3</a></sup> Meeting this requirement requires regular demonstrations of actual, working software, not memos or descriptions of what a system is supposed to do in the future.

Historically, there has been pressure to only use firm fixed price contracts, on the assumption that this reduces risk. However, if you are in a position to constantly measure software quality, a time and materials contract — with a ceiling on total spending — allows for more flexibility for the software development team. A time and materials contract also allows for much easier escape clauses if the direction of the work changes or the vendor team is not producing quality software — if their work is inadequate, or their skills prove inappropriate, the contract can be terminated, and the vendor can be replaced.

#### Checklist

- □ The project has a dedicated, empowered product owner who is an employee of the agency — not a contractor, and not an employee of the state's IT agency
- □ There is a backlog of at least a dozen user stories
- □ An agency contracting officer has embraced this project, and is enthusiastic about procuring software in new ways
- □ The RFP will require a cross-functional team of designers, user researchers, and developers
- □ The RFP will be no more than 20 pages in length
- □ A time and materials contract (with a cap) will be used
- □ The simplest-available procurement vehicle that provides access to the targeted vendors will be used
- □ The RFP will be solely about procuring development services — nothing pertaining to procurement of a product will be included

#### Key Questions

- Is the product owner empowered to rapidly make authoritative decisions on behalf of the agency?
- Is the product owner prepared to spend most of their work hours fulfilling the requirements of this new role?
- Is agency leadership prepared to have product decisions led by identified user needs, based on direct conversations between the development team and those users, rather than leadership's personal preferences?

### Hire tech talent in-house

If nobody in the budget office has experience with software development, then the budget office is not well-equipped to consider the request. If nobody in project leadership at the requesting agency has experience with software development, then the agency is not well-equipped to lead the project successfully. While it may be tempting to solve this knowledge gap by relying on somebody from the state's central IT department, or by relying on a vendor, ultimately mission agencies must have the knowledge in-house to comprehend what they need, what they should be asking of vendors, and assess the work done by vendors.

Although all but the most diminutive agencies will have technical staff who can join project leadership, vanishingly few budget offices currently employ software developers. In this scenario, start by checking whether any employees have software development experience. If not, then it's necessary to hire a software developer, if only on contract or seasonally. The personnel cost is miniscule in comparison to state spending on technology. Also, consider authorizing one or more employees to spend some of their training time learning the basics of agile software development — there are coding "bootcamps" throughout the U.S., including some online-only options. But no matter their experience, once an employee has monitored an agile project from start to finish, they'll be better equipped to consider future budget requests for custom software.

Likewise, the mission agency must directly employ enough developers that they can oversee the work being done by vendors. Although software is never "done" — development is necessary constantly, to adapt to changing technology, policy, regulations, laws, and user needs — there will be a point when far fewer developers are necessary to continue that work, and at that point it becomes especially important to have multiple agency employees who fully grasp the software, who are capable of maintaining it. For larger projects, it is necessary to contract for a scrum team to continue work indefinitely, under the oversight of a government product owner. (Under waterfall, this travels under the name of "Operations and Maintenance," but under agile, O&M is simply continued user research, design, software development, etc.)

#### Checklist

- □ There are one or more budget-office employees with experience developing complex, custom software in an agile environment who will assist in evaluating custom-software budget requests
- □ If there are no budget-office employees with relevant experience, the legislature has a contract with a non-conflicted vendor — one with no other contracts with the state and no ties or partnerships with any COTS products
- □ The agency has identified a specific government employee who will be providing technical leadership for the project, along with evidence of their experience developing custom software in an agile environment

#### Key Questions

- When a vendor delivers code at the end of each and every sprint, which government employee is qualified to inspect that code to ensure that it's of a high quality, and will be assigned to do that work? You need a specific name.
- When an agency says that they need \$10M to complete a specific software project, which budget office employee is equipped to know whether that's an appropriate price? Which legislative budget committee employee is equipped to know whether that's an appropriate price? You need specific names.
- When the procurement is complete, who will maintain that software? Does the agency employ people who know how to maintain it? Will they be brought into the development process, so that they can learn about it as it's built, and help ensure that what's being built is something that they'll be capable of supporting?

### Minimize the cost of change

One day, the exciting, new software system will be the old, hated software system. The underlying needs will change constantly, based on changing state and local laws and regulations, changing technology, and changing user needs and expectations. Your state government will exist longer than this software will. It will eventually be necessary to switch to a new system, in whole or in part. Acquiring software as a completed monolith guarantees that it will gradually become unable to support the agency's needs. Instead, optimize for reducing the cost of updating and changing the system, from the beginning.

#### Checklist

- □ Systems, whether cloud-native or being moved to the cloud, will use service-oriented architecture (SOA)
- □ Files will be stored in open, non-patented formats that are supported by multiple vendors
- □ APIs will use open schemas
- □ Open source software will be used instead of commercial software whenever possible, to avoid product lock-in
- □ Government will own all vendor work products
- □ If using COTS components, the vendor will provide a path to leave for a competitor, both contractually and technologically, allowing a cost-effective way to export all stored data

#### Key Questions

- What is the plan for reducing the time and cost of future updates to the system to reflect technology, policy, and potential vendor changes?
- How much will it cost to change the system to reflect needed technology or policy changes?
- Are the APIs open and usable by other vendors?
- Are the data formats standardized, open, and useable by other vendors?
- Keeping a software system up-to-date will take regular, on-going work — what is the plan to do that?

### Limit total spending

Plan to spend no more than \$10 million on an entire project. (There are rare exceptions for extraordinarily complex systems like unemployment insurance, Medicaid Eligibility & Enrollment, and Medicaid Management Information Systems.) The greater the amount of money spent on a software project, the greater the odds of failure.

#### Checklist

- □ The requesting agency understands that they're not being given a small percentage of the resources that they believe that they need — instead, they're being given an entirely new process to procure software, and adequate funding under that model

#### Key Questions

- If the project ostensibly requires \$20M in funding, what value can be delivered to end-users with \$10M? Or \$2M? If the answer is "none," then this is a project doomed to fail.
- If this spending is matched by federal dollars — especially at a highly-leveraged rate, like the 9:1 match provided by the Centers for Medicare & Medicaid Services for Medicaid Management Information Systems — is anybody going get in trouble for leaving money on the table? Is there somebody whose performance is measured by how much grant funding they raise, who has an incentive to demand that \$100M be spent, instead of \$10M?

### Limit contract sizes

Require that no more than \$2 million be spent on any single contract, annually, and that no contract last for more than three years, including option periods. Using a single vendor over a long period of time, or for a large number of teams, may feel more comfortable, but it inevitably leads to vendor lock-in. The effect of this \$2 million limitation is to get no more than two scrum teams from a single vendor. If the project needs more scrum teams, obtain them from another vendor, and have them work separately. (The more people that work on a project, the greater the amount of time that all of those people have to spend coordinating with all of the other people. The solution to this is to have them work in parallel, which is possible when building with loosely-coupled parts.) Having more than one vendor working on your project provides you with more competitive options if vendors need to change.

Limit the RFP, too, keeping it below 20 pages, and spending no more than 60 days writing it. Another benefit: smaller contracts are less likely to be protested.

#### Checklist

- □ If the project will require multiple contracts, the scope of the first contract has been identified, and there is a general idea of what some other contracts may be comprised of
- □ If there will be more than one scrum team, Service-Oriented Architecture (SOA) will be employed
- □ Contracts will be sized within the simplified procurement threshold, so they can be awarded quickly and easily
- □ The identified first project has relatively low technical complexity, low political risk, and high end-user value, so that teams can start practicing working this way while experimenting and learning in a relatively low-risk environment

#### Key Questions

- Have the relevant contracting officers read this playbook?
- Do the contracting officers understand that they're not being asked to do all of the work that goes into a \$50M contract? Do they understand that \$2M contracts are far easier to award and that, under agile, they'll be much easier to manage?

### Expand your vendor pool

New software design and development approaches are not likely to come from vendors used to delivering waterfall-style systems to government agencies. Lower-dollar contracts, using in-state companies are not likely to come from existing vendors. Odds are, there are many qualified small businesses that can deliver agile development programs in your state. Look for the best talent and encourage your teams to embrace distributed working best practices to engage with development teams.

#### Checklist

- □ The RFP will be streamlined (no more than 20 pages), to be comprehensible by software developers who do not normally work with government
- □ The acquisition plan includes reaching out to small vendors to encourage them to bid
- □ The RFP will not be hidden on a registration-required procurement website, but published openly on the web, so that the vendor community can share it
- □ The RFP will require that vendors name their key personnel in their proposals — no more than three people — such as the lead developer or the lead designer
- □ The acquisition plan includes interviewing the finalists about their proposed approach, questioning the named key personnel, _not_ the vendor's sales staff
- □ Vendor employees will not be required to work on-site at a government facility
- □ Vendor teams and the government product owner will be permitted to use a desktop-based video call service (e.g., Zoom), a real-time collaboration tool (e.g., Slack), and a public version-control system (e.g., GitHub)

#### Key Questions

- Is there any benefit — political or otherwise — to awarding contracts to in-state vendors, and might that limit the degree to which you can expand your vendor pool?
- By hiring vendors whose employees who work remotely in rural areas, it's possible to experience significant savings in labor costs — is \$1M/year savings on each scrum team sufficient to overcome any objections to remote teams?
- Has the necessary market research been done to know what vendors will be targeted?

### Fund systems, not monoliths

Don't replace the old legacy system with a new legacy system. Insist on loosely-coupled systems that are built incrementally, that will never need to be replaced wholesale, but instead can just have individual components replaced as the need arises.

#### Checklist

- □ Each contract will deliver value to end-users — they're not for e.g. setting up a database or maintaining servers, but instead e.g. adding a web-based permit application system or redesigning the intake process to simplify it for agency employees
- □ There will be no "enterprise architect," because the architecture will emerge iteratively throughout the agile process
- □ If the project is large enough that it will include multiple scrum teams working simultaneously, there is no expectation that all members of all teams will ever be in meetings together
- □ The RFP will specify the use of service-oriented architecture for each component

#### Key Questions

- Is there a single point of failure that can bring the whole system down? (If so, that's probably a monolith, not a system.)
- If one vendor's contract needs to be terminated for non-performance, can the others continue to work without interruption?

### Measure success based on iterative outcomes, not project milestones

Value must be provided to end-users within a few months of the contract being awarded, and constantly from there on out, _not_ just at the end of the project. Don't measure progress in "story points," lines of code written, person-hours of work, etc.  The only measure of success that matters is what value has been delivered to end-users. This is best assessed by attending semi-weekly sprint reviews and talking to the scrum master and the government product owner.

#### Checklist

- □ The vendor team will use agile
- □ The vendor will be required to deploy functioning software into a government-owned environment at the end of each sprint
- □ The project team will perform user research routinely, both to inform their planned work and to determine whether the work they've done is correct
- □ The RFP will have no mention of a detailed project schedule, and there will be no mention of Gantt charts or Independent Validation and Verification (IV&V)
- □ A legislative staffer will be assigned to provide oversight of this project, and will coordinate with project leadership to monitor progress by periodically attending sprint reviews

#### Key Questions

- Can the requesting agency deliver value to end-users within six months? What, specifically, is that value?

### Require demos, not memos

Historically, progress in software development projects has been measured by comparing the work that has been done to the schedule of work to be done that was established at the outset. This is done by producing artifacts like Gantt charts and lists of completed tasks. This doesn't work, and agile software development is premised on the idea that this doesn't work. Modern software development teams have never heard of "CMMI" or "Earned Value Management Systems," and won't bid on work that includes these requirements.

A better philosophy is _demos, not memos._ Instead of measuring progress by looking at purpose-made artifacts, instead look at the actual work that is being done. Join the reviews that are held at the end of each sprint, where the work done in that sprint is demonstrated. Try out the website. Install the app. Ask for a "[burn down chart](https://en.wikipedia.org/wiki/Burn_down_chart)" — a graph of work that remains to be done and how much time that will take.

An important part of ensuring that progress isn't illusory is for the contract to include a Quality Assurance Surveillance Plan (QASP) that requires, at the end of each sprint, that all work meet specific standards. Here is an example QASP:

| **Deliverable** | **Performance Standard(s)** | **Acceptable Quality Level** | **Method of Assessment** |
| --- | --- | --- | --- |
| **Tested Code** | Code delivered under the order must have substantial test code coverage and a clean code baseVersion-controlled, public repository of code comprising the product, which will remain in the government domain | Minimum of 90% test coverage of all code | Combination of manual review and automated testing |
| **Properly Styled Code** | [GSA 18F Front-End Guide](https://frontend.18f.gov/#js-style) | 0 linting errors and 0 warnings | Combination of manual review and automated testing |
| **Accessible** | Web Content Accessibility Guidelines 2.1 AA standards | 0 errors reported using an automated scanner, and 0 errors reported in manual testing | [Pa11y](https://github.com/pa11y/pa11y) |
| **Deployed** | Code must successfully build and deploy into staging environment | Successful build with a single command | Combination of manual review and automated testing |
| **Documented** | All dependencies are listed and the licenses are documented. Major functionality in the software/source code is documented. Individual methods are documented inline using comments that permit the use of documentation-generation tools such as [JSDoc](http://usejsdoc.org/). A system diagram is provided. | Combination of manual review and automated testing, if available | Manual review |
| **Secure** | OWASP Application Security Verification Standard 3.0 | Code submitted must be free of medium- and high-level static and dynamic security vulnerabilities | Clean tests from a static testing SaaS (such as [npm audit](https://www.docs.npmjs.com/cli/audit)) and from OWASP ZAP, along with documentation explaining any false positives |
| **User research** | Usability testing and other user research methods must be conducted at regular intervals throughout the development process (not just at the beginning or end). | Artifacts from usability testing and/or other research methods with end-users are available at the end of every applicable sprint, in accordance with the vendor's research plan. | Manual review |

Note that the QASP does not require producing any artifacts explicitly for the purpose of monitoring the work — the way to monitor the work is by _monitoring the work._

#### Checklist

- □ An empowered, dedicated government employee will serve as the product owner
- □ There will be no planning or reporting requirements that run counter to agile, i.e. there are no dates by which specific tasks are to be completed and no specifications of exact functionality that will be required, whether in the RFP, the acquisition plan, or legislation
- □ There will be a government-employed software developer who will ensure compliance with the QASP at the end of each sprint
- □ People providing oversight, above the level of the government product owner, are willing to primarily receive "reports" in the form of demonstrations of functioning software and burn down charts, combined with a review of user stories that have been completed and those that remain to be completed
- □ There is an identified person within the agency who is prepared to provide repeated explanations of progress to each level of oversight, because artifacts of measuring progress on an agile project are strange to people accustomed to waterfall artifacts, and will initially require explanation

#### Key Questions

- Is it feasible to provide the end-to-end support for such a radically different approach to measuring progress, from the agency to the governor's office to the legislature? Is there anybody with the power to dig in their heels and demand a Gantt chart, thus potentially making agile methodology non-viable?
- Whose job will it be to report progress up and out of the agency, e.g. to a legislative oversight committee?

### Share your software

The agency's software is likely to be of use, in whole on in part, to other agencies within the state, to agencies in other states, or to local and regional governments within the state. In addition, in many states, [software created as a work of government is inherently in the public domain](http://copyright.lib.harvard.edu/states/), which means an open-records request is all that's necessary for software to become public. If the software is published openly, vendors' employees will be eager to work on it, because it will be a rare case of work that they can add to their portfolio to e.g. show future employers or share with friends — this will help to ensure that you're getting their best work. Also, additional RFPs issued for the project can direct vendors to the code that's already been written, allowing them to see exactly what they'll be working on or interfacing with.

#### Checklist

- □ The RFP will require that software source code be written and maintained in public on a social-coding platform (e.g., [GitHub](http://github.com/)), from day one
- □ The RFP will require that software be explicitly dedicated to the public domain or published under an [pen source license](https://opensource.org/licenses)
- □ The RFP will require that software be strictly separated from data and secrets (e.g., passwords), with automated testing to make sure that separation is maintained
- □ The RFP will require that software be documented sufficiently well that a developer with no connection to the project can use it to run their own copy of the software

#### Key Questions

- Will the state or agency security office panic at the prospect of publishing open-source software, and block deployment of the software?
- Are there other agencies in the state who are likely to benefit from this software? Can they be consulted prior to and during the development process?
- Will the agency's office of general counsel (or its equivalent) object to publishing software in the public domain or under an [OSI-approved open source license](https://opensource.org/licenses)?

### Budget for software as an operational expense

Custom software is never "done." Plan for software to be modified continuously, so that it will serve the agency's needs, rather than vice versa. For small systems, this may require adding one or fewer FTEs to the agency's staff of software developers. For large, flagship systems, this may require procuring a team of developers to continually develop and maintain the software.

Software maintenance is sometimes budgeted for as if it is a different activity than initially building software, but that is a mistake. Maintaining software should mean simply continuing to modify it in response to identified user needs, which change continuously along with laws, regulations, policies, best practices, and technology. This requires the same skillsets, methodology, and tasks as building a system in the first place. A proposal to transition software development into an "operations and maintenance" ("O&M") phase should be seen as a red flag.

Funding can be ramped up over the course of several budget cycles, as the requesting agency demonstrates that they're successfully reducing risk, controlling costs, and delivering iteratively to end users.

Ultimately, this can provide agencies with a predictable source of funding for software projects — replacing unpredictable capital expenditures — while simultaneously providing the legislature with a predictable annual cost for all agency software projects.

Rule of thumb: a "scrum team" of 5–9 developers costs \$1–2M/year, depending on the cost of living in the area where the developers reside.

#### Checklist

- □ The agency plans to procure agile development services
- □ You have talked with the requesting agency to determine if it would be their preference to receive the money over years, as a predictable stream of operational funding, instead of as a lump sum
- □ This approach has been coordinated with the governor's office, the budget office, agencies, the state IT agency, because this is a radical change, relative to agency expectations, and it will require trust and cooperation between all parties
- □ If an agency's request is at a high risk of failure, you will allocate only a few million dollars in the first year, and increase funding as the project delivers value
- □ The agency recognizes that software must be maintained for as long as it is in use, and that maintenance is functionally the same as building software in the first place

#### Key Questions

- Is the requested funding going to be spent within a single budget period?
- Maybe \$50M is being requested, but what value can be delivered to end-users with \$2M? And with the next \$2M? And so on?
- If this project is being funded using federal dollars, is the federal agency amenable to taking an operational approach to the funding?

### Ask technical questions of agencies

Budget requests for custom software often feature non-technical people making a technical proposal to non-technical people. This process doesn't lend itself to asking key questions, such as many of those found throughout this playbook. It is important to ask all of those difficult technical questions, and to insist on getting the right answers. It is no kindness to fund a project that is going to fail. If the agency doesn't know exactly what they want to buy, they're not going to get it.

#### Checklist

- □ The agency will rely on the U.S. Digital Service's [Digital Services Playbook](https://playbook.cio.gov/)
- □ If building a website, the agency will direct the vendor to use the [S. Web Design System](https://designsystem.digital.gov/)
- □ The agency will adhere to the Defense Innovation Board's "[Ten Commandments of Software](https://media.defense.gov/2018/Apr/22/2001906836/-1/-1/0/DEFENSEINNOVATIONBOARD_TEN_COMMANDMENTS_OF_SOFTWARE_2018.04.20.PDF)"
- □ The agency has read this playbook
- □ The rules and questions found in the Defense Innovation Board's "[Detecting Agile BS](https://media.defense.gov/2018/Oct/09/2002049591/-1/-1/0/DIB_DETECTING_AGILE_BS_2018.10.05.PDF)" guide have been applied to and asked of the agency, and their answers are satisfactory

#### Key Questions

- What exactly does the agency want to buy? Why? Who will benefit?
- Which parts of the system will be custom? Which will be COTS? What will be done when a commercial component ends production, e.g. the database company goes out of business?
- Who are the end-users of your system? Have you talked to them? What do _they_ want?
- Are you prepared for when changes need to be made?
- How much will it cost to move to a new system?
- What are you doing to avoid paying expensive change fees in the future?


## Appendix: Questions to Ask

When you are in the position of having to consider a budget request for a custom software project, it will be difficult to consult this entire playbook to find the right questions to ask. Here are some basic, open-ended questions that you can ask to determine if a project is set up for success.

- What is the user need that this project will address?
  - Wrong answer: Anything other than a clear, direct, confident answer.
  - Right answer: The agency has interviewed users and determined specific user needs based on those interviews, and can name several of them.
- What value will be delivered to the users within six months?
  - Wrong answer: "None — it won't be ready by then. We plan to show it to users when everything is finished."
  - Right answer: Specific examples are named.
- Who will be the product owner?
  - Wrong answer: "What is a 'product owner'?"
  - Right answer: A specific person is named or "we're training in-house staff to do that".
- On the team who prepared this request, who has experience developing software?
  - Wrong answer: "Nobody."
  - Right answer: A specific person is named.
- How often is work being deployed into production?
  - Wrong answer: "Once — when it's done."
  - Right answer: "At the end of each sprint."
- Is the project automating testing? Integration? Deployment? Security tests?
  - Wrong answer: "We're...working on that."
  - Right answer: "Yes, from day one."
- If the vendor isn't performing adequately, how difficult will it be to terminate the contract? How long will it take to replace them with another vendor? How much do you think that will cost?
  - Wrong answer: "We would be very reluctant to terminate the contract. It would take months or years to replace them with a new vendor. Significant staff time would be required to do that, and it would set our project back by many months. Once we have a system, we'd have to start all over if we decide to change vendors."
  - Right answer: "It will be a time and materials contract, so we could stop assigning work to the vendor at any time, and that would be the functional end of the contract. We could reissue the RFP and have a new vendor onboarded within six weeks. It would require a small amount of staff time, and it would set the project back only by those six weeks."
- Does the RFP include requirements for how the system will operate?  If so, how many requirements are included?
  - Wrong answer: The agency has spent the past 3 years reviewing its business requirements and has a detailed list (hundreds of pages) of requirements (thousands) to include in the RFP.
  - Right answer: The agency is focused more on the outcomes it wants from a new system and has developed a backlog of user stories to help guide the team's work rather than a detailed list technical requirements
- How many pages is in the RFP?
  - Wrong answer: "We've developed several hundred pages of system requirements along with 50 more pages of standard terms and conditions."
  - Right answer: "Less than 20 pages and we're using the state's simplified procurement threshold to make it easier, cheaper, and faster for new vendors to bid on the project."
- Do you anticipate issuing a fixed price or time and materials contract?
  - Wrong answer: "Fixed price, because it's the best way to control vendor costs."
  - Right answer: "Time and materials, because it's the best way to retain the flexibility we need to respond to user needs, manage to unforeseen technical challenges, and ensure vendors that aren't delivering what we need can be changed without putting the project at risk."
- How much will change orders cost?
  - Wrong answer: Any response that foresees change orders of any kind is bad.
  - Right answer: "We expect the system to change constantly in response to new user needs, new technology and new policy so that's why we're using a time and materials contract and an agile development approach to lower the cost of responding to these changes."
- How will you know if the project is on track and contractors are delivering as promised or if things are off track?
  - Wrong answer: "We're contracting with an independent verification and validation (IV&V) expert to provide us with monthly reports on the project's status."
  - Right answer: "Vendors will provide monthly demonstrations of working software that reflect our priorities, meet the technical standard of the QASP, and provide value to our end-users. If these standards are not met, and value to end-users isn't shown within six months, they'll be terminated."

---

## Footnotes

<small>

<p class="footnote" id="footnote-1">1. Projects valued at $6M or greater, in Europe and the United States, that were completed satisfactorily, on time, and within budget. From The Standish Group's "<a href="https://www.standishgroup.com/sample_research_files/Haze4.pdf">Haze</a>," based on their CHAOS database. <a href="#reference-1">↩︎</a></p>

<p class="footnote" id="footnote-2">2. A user story reads in form of "as a [role], I need [this thing], so I can [accomplish this]." For example, "as a social worker, I need case notes to be cached on my phone, so that I can access case notes in areas without mobile phone service." All technical work is done in the service of addressing a user story. <a href="#reference-2">↩︎</a></p>

<p class="footnote" id="footnote-3">3. For an example QASP, [see the "Deliverables and Performance Standards" section of the <a href="https://github.com/ustaxcourt/case-management-rfq/blob/master/02_SOW.md#deliverables-and-performance-standards">U.S. Tax Court's 2018 EF-CMS RFQ</a>. <a href="#reference-3">↩︎</a></p>

</small>
