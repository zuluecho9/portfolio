# Zach Elwood

**Technical Writer | Communications Specialist | Content Marketing and Strategy | Audio/Video Producer**

---

## What's this? 
This is a portfolio for the writing/communication career of me, Zachary Elwood. 

## About me

I'm an experienced technical writer and all-around communicator, skilled at turning complex concepts into clear, engaging stories and instructions, and at seeing large projects through to completion. In my life I've been:

- A technical writer (Lead Tech Writer at the full-stack observability company New Relic, API tech writer for Amazon Ads APIs)  
- A content marketer and strategist for tech/software companies
- An instructional designer
- A commercial video writer/director/producer
- An author of a newsletter with 140K+ subscribers, and writer/reviewer of content for a social media team with 3M+ followers
- An author and publisher of several successful books (48,000+ sold)
- An independent investigative journalist whose [research](https://apokerplayer.medium.com/zach-elwoods-investigations-into-deceptive-online-activity-60c3b11c2774) has been featured in *The New York Times*, *The Washington Post*, *Buzzfeed*, and more

What ties these diverse endeavors together is a striving for clear, accurate, and engaging communication. 

For details about my roles, see [my LinkedIn](https://linkedin.com/in/zelwood). 

## Featured testimonials

> "Zach is literally the most productive technical writer I've ever worked with. If you're looking for greatness, get in touch with him."
> **— Austin Schaefer**, Head of Dev Docs at Shopify, Former Director at New Relic ([see original post](https://www.linkedin.com/feed/update/urn:li:activity:7396594695725879296))

> "If you're looking to add a technical writer capable of untangling complex ideas and want someone with an unshakeable work ethic who can get tough jobs done for you, talk to Zach. You'll be glad you did."
> **- Mark Buchanan**, Sr. Director of Product Language at New Relic

> "In his time working on my team, I was struck by how quickly he ramped up on new problems and technical concepts."
> **- Avtar Khalsa**, Sr. Software Dev Manager, Amazon Ads APIs

For more testimonials, see [my LinkedIn](https://linkedin.com/in/zelwood)

## Portfolio sections

- [Tech writing examples](#tech-writing-examples)  
- [Content marketing examples](#content-marketing-examples)
- [Coding/scripting experience](#coding-and-scripting-experience)

## Tech writing examples

During my 7.5 years at New Relic, an observability and full‑stack monitoring company with 700+ integrations, I worked on a wide range of highly technical documentation projects. My final role there was Lead Technical Writer (a role above Senior). The projects I worked on spanned multiple technologies, programming languages, types of APIs, and data models.

> Note on aesthetics: The examples below currently lack the styling of the New Relic docs site where they were originally created. Where possible, I link to the public versions, which remain largely unchanged from when I wrote them.

Overview of examples: 

- [Implementation guide](#example-1-new-relic-implementation-guide) 
- [Telemetry data concepts](#example-2-understanding-telemetry-data)  
- [Pricing and billing](#example-3-pricing-and-account-user-model-updates)
- [API overviews](#example-4-api-overview)
- [Distributed tracing API](#example-5-distributed-tracing-api)  
- [Query language](#example-6-querying-data-with-nrql)  
- [Go language agent APIs](#example-7-go-language-agent)  

---

### Example 1: New Relic implementation guide

For one of my final major projects at New Relic, I created a comprehensive implementation guide to help new customers set up the platform efficiently and start getting value quickly. This was challenging due to the sheer number of New Relic features and the wide range of customer sizes and architectures, which made it difficult to define a single setup path that worked for everyone. That complexity was a key reason such a guide hadn’t existed before, despite being a long-standing gap.

This project brought together everything I’d learned about observability and the New Relic platform. It required extensive collaboration with solutions architects, support, and customer success teams, as well as careful judgment to synthesize differing stakeholder views into a clear, practical recommended approach.

#### Sample section

## Implementation part 1: Plan and set up your account

This is the first part of our [implementation guide](https://docs.newrelic.com/docs/new-relic-solutions/get-started/implementation-guide-intro).

When you first sign up for New Relic, there are some important account- and user-related decisions to make. In this stage of the implementation, you'll:

- Decide on some important account-related settings  
- Think about who your New Relic team leads will be  
- Think about what components in your system you should instrument  
- Think about some strategies for organizing your data  

### Initial account setup

When you [sign up for New Relic](https://newrelic.com/signup), you get a *New Relic organization*. This organization is the container for your organization's data, accounts, and users. Here are some important initial things to consider.

### Decide on data center region

When you sign up for New Relic, you must choose which of our two data center regions your organization will be in: US or EU. There are some differences between the regions: for example, they have different API endpoints, and have some feature differences. [Learn more about data center regions](https://docs.newrelic.com/docs/accounts/accounts-billing/account-setup/choose-your-data-center).

### Think about the edition you'll need

A New Relic organization can use New Relic [free, forever](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-pricing-billing/new-relic-one-pricing-billing/#free). When a New Relic organization starts to pay for New Relic, it can be on one of three editions: Standard, Pro, or Enterprise. You can always upgrade your edition later, but for larger organizations it may make sense to look at the editions to understand the features of each and which you'll likely end up on: see our [pricing page](https://newrelic.com/pricing).

### Decide on security compliance needs

New Relic offers a high level of security by default ([read more about our security features](https://newrelic.com/security)). But certain industries require much higher levels of security compliance (for example, healthcare and financial institutions). For these organizations, we offer FedRAMP and HIPAA security compliance. These compliance options require both Enterprise edition ([learn more about editions](https://newrelic.com/pricing)) and our Data Plus option. Data Plus gives you access to some powerful data features, like increased retention and higher query limits. [Read more about the benefits of Data Plus](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-pricing-billing/data-ingest-billing/#data-plus).

For more on our compliance features, see the docs:

- [FedRAMP](https://docs.newrelic.com/docs/security/security-privacy/compliance/fedramp-compliant-endpoints)  
- [HIPAA](https://docs.newrelic.com/docs/security/security-privacy/compliance/hipaa-readiness-new-relic)  

### Decide on team leads

You'll want to decide which of your team members will be your initial New Relic team leads. These will be the team members who do one or more of the following:

- Set up and configure instrumentation  
- Add and manage New Relic users  
- Oversee billing  
- Train your users and answer questions  

Here are some things to consider when adding team leads:

- Assign user type based on expected duties. For administrative duties, you must make your users either core or full platform users. [Learn more about user type](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-user-management/user-type).  
- Assign users to appropriate [groups](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-user-management/user-management-concepts/#understand-concepts). Options for adding admins to groups:  
  - Add them to the default [Admin group](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-user-management/user-management-concepts/#default-groups), which gives access to everything.  
  - Give them the [Group admin role](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-user-management/user-management-concepts/#group-admin), which grants them ability to add/remove users for specific groups.  
  - Create a [custom group](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-user-management/account-user-mgmt-tutorial/#grants-ui).  

We recommend using a spreadsheet to plan out your users' New Relic responsibilities.

---

**READ MORE:** The implementation guide is largely unchanged from when I wrote it in 2023. [Read the rest of the doc here](https://docs.newrelic.com/docs/new-relic-solutions/get-started/implementation-guide-planning-setup). 


## Example #2: Understanding telemetry data

Despite New Relic being a data-focused company, several years into their existence they still had no public document explaining what they meant by the various types of telemetry data (metrics, events, logs, traces) or how those different types of data were handled by the platform. It had been in the docs backlog for years to create such a doc but, surprisingly, it had never been done. Based on my own frustrations trying to understand these things, as someone new to the observability space, and based on seeing a lot of customer confusion, I proposed that I work on this much-needed doc.

I researched this by talking with many SMEs across the company, trying to piece together the intricacies of how the industry generally used these words and how we at New Relic were using these words. I was very proud of this doc and it ended up being one of the most high-traffic docs on the site. One reason for this is that it was useful even to non-New Relic customers in understanding how these terms were being used in the monitoring space.

#### Sample section

## New Relic data types

The New Relic platform is built around the four fundamental telemetry data types we believe are necessary for complete and effective system monitoring: metrics, events, logs, and traces.

### Get started

This doc will give you a fairly technical explanation of our core data types, their structure, and how they're used in our features. You can use most of our features without needing to understand the underlying data structure. But having a better understanding of this can help you get data into New Relic, understand the data you see in our UI, and query your data.

For a simpler explanation of these data types using real-world examples, see Introduction to essential telemetry data types. Another good way to understand your data is to just start querying it.

**Tip**

Access your data easily on one.newrelic.com: Click the Browse data dropdown menu and select the data type (metrics, events, logs, and traces) you want to explore.

### Metrics

First, we’ll explain the definition of metrics from a monitoring industry perspective, and then we’ll explain how New Relic handles metrics. For a list of the metrics we collect, see our documentation on metrics.

#### Metrics in the monitoring industry

In the software monitoring industry, a metric means a numeric measurement of an application or system. Metrics are typically reported on a regular schedule.

Two major types of metrics are:

- Aggregated data. For example: a count of events over one minute’s time, or the rate of some event per minute.
- A numeric status at a moment in time. For example: a CPU temperature reading, or a “CPU% used” status.

Metrics are relatively easy to report and store because a single record can represent a range of time. They can also be aggregated more and more over time. For example, per-minute data may be “rolled up” to per-hour aggregations after some amount of time, and eventually may be rolled up to a per-day aggregation. This approach is efficient for long-term data storage.

Metrics are a strong solution for storing data long-term, and understanding trends over time. One potential downside is that it can be difficult to do detailed analysis of older data that has been aggregated over time; when high detail is required about specific important actions, event data can be used.

#### Metrics at New Relic

Conceptually, "metrics" is a broad, general category. There are various ways New Relic measures and reports metrics but, in practice, when using the New Relic UI, you usually won't have to understand how exactly this happens. In our documentation, we typically will just refer to "metrics," regardless of how that data is reported, unless there's a reason you need to know more (like understanding how to query your data).

**READ MORE:** This doc is largely unchanged from when I wrote it in 2018. Read the rest of the doc here:  
https://docs.newrelic.com/docs/data-apis/understand-data/new-relic-data-types

---







## Content 


## Coding and scripting experience 

I'm far from a professional coder but I have strong general knowledge of software development and deployment. My best language is Python, but I've documented and written code examples for many languages, application frameworks, and types of APIs (with most of that experience coming from my time at New Relic, due to the full-stack breadth of their offerings). AI/LLM tools have dramatically improved my ability to write scripts/code to solve specific technical challenges. 

As evidence of my skills and comfort with coding, check out a [personal coding project](www.linkedin.com/feed/update/urn:li:activity:7401999440531705856) of mine, which involves video and computer-vision algorithms.  


