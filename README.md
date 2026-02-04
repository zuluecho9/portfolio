# Zach Elwood

**Technical Writer | Communications Specialist | Content Marketing and Strategy | Audio/Video Producer**

---

[![Zach Elwood linkedin header image](https://github.com/zuluecho9/portfolio/blob/main/Zach-image-header.png)](https://github.com/zuluecho9/portfolio/blob/main/Zach-image-header.png)

## What's this? 
This is a portfolio for [Zachary Elwood](https://linkedin.com/in/zelwood)'s technical writing/communication career.

## About me

I'm an experienced technical writer and all-around communicator, skilled at turning complex concepts into clear, engaging stories and instructions, and at seeing large projects through to completion. In my life I've been:

- A technical writer (Lead Tech Writer at the full-stack observability company New Relic, API tech writer for Amazon Ads APIs)  
- A content marketer and strategist for tech/software companies
- An instructional designer
- A commercial video writer/director/producer
- An author of a newsletter with 140K+ subscribers, and writer/reviewer of content for a social media team with 3M+ followers
- An author and publisher of several successful non-fiction/how-to books (48,000+ sold)
- An independent investigative journalist whose [research](https://apokerplayer.medium.com/zach-elwoods-investigations-into-deceptive-online-activity-60c3b11c2774) has been featured in *The New York Times*, *The Washington Post*, *Buzzfeed*, and more

What ties these diverse endeavors together is my passion for clear, accurate, and engaging communication. 

For details about my roles, see [my LinkedIn](https://linkedin.com/in/zelwood). 

## Featured testimonials

> "Zach is literally the most productive technical writer I've ever worked with. If you're looking for greatness, get in touch with him."
> **— Austin Schaefer**, Head of Dev Docs at Shopify, former Director of Documentation at New Relic ([see original post](https://www.linkedin.com/feed/update/urn:li:activity:7396594695725879296))

> "If you're looking to add a technical writer capable of untangling complex ideas and want someone with an unshakeable work ethic who can get tough jobs done for you, talk to Zach. You'll be glad you did."
> **- Mark Buchanan**, Sr. Director of Product Language at New Relic

> "In his time working on my team, I was struck by how quickly he ramped up on new problems and technical concepts."
> **- Avtar Khalsa**, Sr. Software Dev Manager, Amazon Ads APIs

> "Zach is probably the most technically capable and proficient writer I've ever had the pleasure to work with. He's still the #1 contributor to our [docs repo](https://github.com/newrelic/docs-website/graphs/contributors) a year after he left.">
> **- Shawn Kilburn**, previously a docs manager at New Relic

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
- [Pricing and billing](#example-3-pricingbilling-and-accountuser-model-updates)
- [API overviews](#example-4-overview-of-new-relic-apis)
- [Distributed tracing API](#example-5-distributed-tracing-api)  
- [Query language](#example-6-querying-data-with-nrql)  
- [Go language agent APIs](#example-7-go-language-monitoring-agent-apis)  

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

---

### Example #2: Understanding telemetry data

Despite New Relic being a data-centric company, several years into their existence they still had no public doc explaining the various types of telemetry data they collected (metrics, events, logs, traces) or how that data was handled by the platform. It had been in the docs backlog for years to create such a doc but, surprisingly, it had never been done. Based on my own frustrations trying to understand these areas, as someone new to the observability space, and based on seeing a lot of customer confusion, I made the case that I should work on this much-needed doc.

I researched this by talking with many SMEs across the company, trying to piece together the intricacies of how the industry generally used these words and how we at New Relic were using these words. I was very proud of this doc and it ended up being one of the most high-traffic docs on the site. One reason for this is that it was useful even to non-New Relic customers in understanding how these terms were being used in the monitoring space.

#### Sample section

## New Relic data types

The New Relic platform is built around the four fundamental telemetry data types we believe are necessary for complete and effective system monitoring: [metrics](#metrics), [events](#event-data), [logs](#log-data), and [traces](#trace-data) (often referred to as "MELT" in the observability industry).

After you [sign up for a free New Relic account](https://newrelic.com/signup) and [install](https://docs.newrelic.com/docs/using-new-relic/cross-product-functions/install-configure/install-new-relic) any of our monitoring services, you can start working with your data.

### Get started understanding our data

In this doc, we'll give a fairly technical explanation of our core MELT data types, their structure, and how they're used in our features. You can use most of our features without needing to understand the underlying data structure. But having a better understanding of this can help you [get data into New Relic](https://docs.newrelic.com/docs/data-apis/custom-data/get-custom-data-from-any-source), understand the data you see in our UI, and [query and chart your data](https://docs.newrelic.com/docs/query-your-data/explore-query-data/get-started/introduction-querying-new-relic-data).

### Metrics

First, we'll explain the definition of metrics from a monitoring industry perspective, and then we'll explain how New Relic handles metrics.

#### Metrics in the monitoring industry

In the software monitoring industry, a metric means a numeric measurement of an application or system. Metrics are typically reported on a regular schedule.

Two major types of metrics are:

* Aggregated data. For example: a count of events over one minute's time, or the rate of some event per minute.
* A numeric status at a moment in time. For example: a CPU temperature reading, or a “CPU% used” status.

Metrics are relatively easy to report and store because a single record can represent a range of time. They can also be aggregated more and more over time. For example, per-minute data may be “rolled up” to per-hour aggregations after some amount of time, and eventually may be rolled up to a per-day aggregation. This approach is efficient for long-term data storage.

Metrics are a strong solution for storing data long-term, and understanding trends over time. One potential downside is that it can be difficult to do detailed analysis of older data that has been aggregated over time; when high detail is required about specific important actions, [event data](#event-data) can be used.

#### Metrics at New Relic 

Conceptually, "metrics" is a broad, general category. There are various ways New Relic measures and reports metrics but, in practice, when using the New Relic UI, you usually won't have to understand how exactly this happens. In our documentation, we typically will just refer to "metrics," regardless of how that data is reported, unless there's a reason you need to know more (like understanding [how to query your data](https://docs.newrelic.com/docs/using-new-relic/data/understand-data/query-new-relic-data)).

Here are some of the ways metrics are reported and stored across the New Relic platform:

##### Dimensional metrics 

In the monitoring industry, "dimensional" metrics refer to metric data that has a variety of [attributes](https://docs.newrelic.com/docs/using-new-relic/welcome-new-relic/get-started/glossary#attribute) (dimensions) attached, such as duration-related attributes (start time, end time), entity ID, region, host, and more. This level of detail allows for in-depth analysis and querying.

At New Relic, this metric data is attached to our [`Metric`](https://docs.newrelic.com/docs/data-apis/understand-data/metric-data/metric-data-type) data type. This is our primary metric data type and is used by many of our tools, including:

* Our integrations with third-party telemetry services, like our [OpenTelemetry integration](https://docs.newrelic.com/docs/more-integrations/open-source-telemetry-integrations/opentelemetry/opentelemetry-introduction), our [Prometheus integration](https://docs.newrelic.com/docs/infrastructure/prometheus-integrations/get-started/send-prometheus-metric-data-new-relic), and our [DropWizard integration](https://docs.newrelic.com/docs/more-integrations/open-source-telemetry-integrations/dropwizard/dropwizard-reporter).
* The [Metric API](https://docs.newrelic.com/docs/introduction-new-relic-metric-api) (the underlying API used by the above tools).
* The [events-to-metrics service](https://docs.newrelic.com/docs/data-ingest-apis/get-data-new-relic/metric-api/introduction-events-metrics-service).

To query the `Metric` data type, you could use a NRQL query like:

```sql
SELECT * FROM Metric
```

As time passes, metrics are increasingly aggregated into larger time buckets. This is done to optimize your ability to query data over a long period of time.

For more details about `Metric` data, see [`Metric` data structure](https://docs.newrelic.com/docs/telemetry-data-platform/ingest-manage-data/understand-data/metric-data-type). For tips on querying this data, see [Metric query examples](https://docs.newrelic.com/docs/data-ingest-apis/get-data-new-relic/metric-api/view-query-you-metric-data).

Some of our other metric data types are exposed as dimensional metrics and are available for querying. For example:

* [APM metric timeslice data](https://docs.newrelic.com/docs/data-apis/understand-data/metric-data/query-apm-metric-timeslice-data-nrql)
* [Some infrastructure data](https://docs.newrelic.com/docs/query-your-data/nrql-new-relic-query-language/nrql-query-tutorials/query-infrastructure-dimensional-metrics-nrql)

---

**READ MORE:** This doc is largely unchanged from when I wrote it in 2018. [Read the rest of the doc here](https://docs.newrelic.com/docs/data-apis/understand-data/new-relic-data-types). 

---

## Example 3: Pricing/billing and account/user model updates

This project was probably my most important accomplishment during my time at New Relic: overhauling the docs to reflect substantial changes to the pricing model and the account/user model. These were core changes to the platform that impacted many aspects of the customer experience; these changes impacted hundreds of docs. They were also touchy and sensitive changes. Customers can be easily frustrated when there is confusion over how their billing works, or how to manage/provision users (which affects cost). 

This project would have been tough enough if all customers were simultaneously switching over to the new models. Unfortunately, the new ways applied mainly to brand new customers; the older models would continue to be used for thousands of our already existing customers, and we’d slowly migrate older customers to the new ways. Also, the two new models, the pricing model and the account/user model, were not linked; it was possible for customers to update one but not the other. This meant that customers could be in one of four states, which created large challenges in thinking through how to efficiently and cleanly address these four customer segments in the docs. 

The goal was to create clean, simple docs that would not confuse customers — especially new customers, who we didn’t want to bog down with confusing details they didn't need to know. 

I was proud of the architecture and readability of the many docs I created and edited for this project. The work I did received many accolades from across the company. This is a performance review from my manager after that launch (known as Hercules): 

*Thank you for an incredible launch. Honestly, I'm so damn grateful for you that I don't know where to start. Let's start with accounts: You are fearless. The accounts and pricing docs were a crowded billboard of ancient callouts, mysterious tables, purposeless paragraphs. As if that challenge wasn't great enough, we gave you black box of new features labeled only "Pricing and Accounts V2." It would've been easy to throw up your hands, or to just tack the new stuff on top of the old and call it good enough.*

*But rather than do that, you dove in. You pushed PMs and leaders to clarify a cloudy vision. You articulated a whole new user journey for pricing, where our site can focus on helping users and marketing and product can handle the upsell details. You helped define the very name of the new pricing model. You earned you and docs a shoutout from the GM in the wrap-up session.*

*You did all that without neglecting the daily mechanics that make this team great. By my count you've edited 351 docs since Hercules began. Last week, you chased down every hero question to the end of the rabbithole instead of just closing your eyes to hit publish.* 

Here’s a sample from the pricing overview doc (this comes from a [2021 version of the pricing doc](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-pricing-billing/new-relic-one-pricing-billing)): 

## Sample section 

### New Relic pricing 

An explanation of how New Relic One pricing works, and how to view and manage billing.

*This document explains the New Relic One pricing plan. If you’re on our original pricing plan, see [Product-based pricing](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/accounts/original-accounts-billing/product-pricing/product-based-pricing). Not sure which you're on? See [Overview of pricing](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/transition-guide-our-new-pricing-plan-user-model).*

#### How New Relic One pricing works 

Starting July 30, 2020, all of our new customers are on a pricing plan that we call New Relic One pricing. Customers on our original pricing plan are able to transition to this  
[pricing](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/accounts/original-accounts-billing/original-product-based-pricing/overview-changes-pricing-user-model#how-to-transition).

For New Relic One pricing, billing is based on these factors:

- The pricing tier (Standard, Pro, Enterprise). Higher pricing tiers give access to more account-related admin features, more support, longer data retention, and other features ([learn more](https://web.archive.org/web/20210128094340/https://newrelic.com/pricing)).
- The number of [full users](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-pricing-users/users-roles#user-type) (users with access to everything available at that tier). [Basic users](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-pricing-users/users-roles#user-type) are free. Standard tier includes one full user for free, and a max of five.
- The amount of data ingested. 100 GBs per month is free. $0.25 per GB ingested above that.
- For [Applied Intelligence](https://web.archive.org/web/20210128094340/https://newrelic.com/pricing), our intelligent alert/detection system: the number of events above the free included amount. (Note that our alerting functionality is available for free and doesn't count towards this limit.)

> **TIP:** Note that this pricing plan allows you to have an entirely free Standard tier account with one full [user](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/users-roles#user-type) and multiple [basic users](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/users-roles#user-type), provided you're okay with the free included limits.

#### View and manage billing and usage

Some ways to view and manage your billing and usage:

- To view and manage billing settings: from the [account dropdown](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/using-new-relic/welcome-new-relic/get-started/glossary#account-dropdown), click **Manage your plan**.
- To view billing-related usage: from the [account dropdown](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/using-new-relic/welcome-new-relic/get-started/glossary#account-dropdown), click **View your usage**.
- To view and manage data ingest and retention: from the [account dropdown](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/using-new-relic/welcome-new-relic/get-started/glossary#account-dropdown), click **Manage your data**.

You can also do [in-depth queries of your usage data and set up alerts](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-pricing-users/queries-alerts).

Only account owners or users with the **Billing user** role can manage billing and usage.

#### How to update your billing and payment information

Here are the steps:

- Ensure you are an account owner or a user with the Billing user role.
- From [one.newrelic.com](https://one.newrelic.com/), select the [account dropdown](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/accounts-partnerships/education/getting-started-new-relic/glossary#account-dropdown) on the upper right corner of your screen, click **Manage your plan**.
- Next, click **Billing & Invoices**.
- To update your credit card information, click **Manage Payment**.
- To update your billing details, click **Manage Billing**.

#### Billing calculation details

For accounts on New Relic One pricing, some high-level billing information is displayed [in the UI](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-pricing-billing/new-relic-one-pricing-billing/#billing-usage-ui). Here are some more details about how billing works:

---

**READ MORE:**  
To read more of this pricing overview doc, see [this 2021 version of the doc](https://web.archive.org/web/20210128094340/https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-pricing-billing/new-relic-one-pricing-billing/). [Here’s a doc explaining the pricing changes in more detail](https://docs.newrelic.com/docs/accounts/original-accounts-billing/original-product-based-pricing/overview-changes-pricing-user-model).

---

## Example #4: Overview of New Relic APIs

By the time I became Senior Tech Writer at New Relic, I was the go-to person for docs pertaining to the company’s core APIs and their data model. This was largely due to the time I’d spent working through the intricacies of how New Relic handled data and how different teams used data terminology.

One of my projects was to improve the overview of New Relic’s APIs. They lacked a clean overview of their API resources. They had so many APIs, it could be rather confusing to know which API to use for what. This problem was exacerbated by the addition of a GraphQL-format API, which was eventually going to be their main API for querying data and making
configurations — but in the meantime it was rather rudimentary in features and also lived alongside all the other, older, more established APIs.

Here’s an excerpt from my API overview doc:

### Sample section

## Introduction to New Relic APIs

New Relic offers a variety of APIs and SDKs you can use to:
* Send data to New Relic.​
* Retrieve data from New Relic.
* View and configure settings.
  
Looking for API keys? [See API keys](https://docs.newrelic.com/docs/apis/intro-apis/new-relic-api-keys/).

### APIs for data ingest

Our data ingest APIs are some of our [many solutions for reporting data](https://newrelic.com/instant-observability). Our APIs can be used directly, but they're also the underlying ingest route for many of our data-reporting tools. If you're just getting started reporting data to New Relic, we recommend starting at [Install New Relic](https://docs.newrelic.com/docs/new-relic-solutions/new-relic-one/install-configure/install-new-relic).

| API type | Description |
|--------|-------------|
| [Metric API](https://docs.newrelic.com/docs/introduction-new-relic-metric-api) | Send [dimensional metrics](https://docs.newrelic.com/docs/data-apis/understand-data/new-relic-data-types/#dimensional-metrics) to New Relic from any source (including other telemetry monitoring services). |
| [Event API](https://docs.newrelic.com/docs/telemetry-data-platform/ingest-apis/introduction-event-api) | Send custom [event data](https://docs.newrelic.com/docs/data-apis/understand-data/new-relic-data-types/#events-new-relic) to New Relic without the use of an agent or integration. |
| [Log API](https://docs.newrelic.com/docs/enable-new-relic-logs-http-input) | Send [log data](https://docs.newrelic.com/docs/data-apis/understand-data/new-relic-data-types/#log-data) to New Relic. |
| [Trace API](https://docs.newrelic.com/docs/apm/distributed-tracing/trace-api/introduction-new-relic-trace-api) | Send [distributed tracing data](https://docs.newrelic.com/docs/data-apis/understand-data/new-relic-data-types/#trace-data) (`Span` data) to New Relic without the use of an agent or integration. |

---

**READ MORE**: This doc is largely unchanged from when I wrote it in 2019. [Read the rest of the doc here](https://docs.newrelic.com/docs/apis/intro-apis/introduction-new-relic-apis/).

---

## Example 5: Distributed tracing API

One of my earlier large projects at New Relic was being embedded with a product team as they rolled out their distributed tracing feature. This was considered a highly important feature, as distributed tracing was big at that time in the monitoring/observability space. I documented a new UI, new types of data and querying, and new APIs. The docs were a success; one sign of this was that the docs had significantly higher CSAT (customer satisfaction) scores than average.

### Sample section 

## Report traces via the Trace API (New Relic format)

If you want to create your own tracing implementation, you can use our [Trace API](https://docs.newrelic.com/docs/understand-dependencies/distributed-tracing/trace-api/introduction-trace-api). This doc explains how to send traces in our general format, also known as `newrelic` format. (To send Zipkin-format data, see [Zipkin](https://docs.newrelic.com/docs/apm/distributed-tracing/trace-api/report-zipkin-format-traces-trace-api).)

## Get started 

Using our Trace API is as simple as:

* Sending trace data in the expected format (in this case, our `newrelic` format).
* Sending that data to the appropriate [endpoint](https://docs.newrelic.com/docs/understand-dependencies/distributed-tracing/trace-api/trace-api-general-requirements-limits#requirements).

Before using the Trace API, you should decide whether you want to use Infinite Tracing. To learn more about this, see [Intro to Infinite Tracing](https://docs.newrelic.com/docs/understand-dependencies/distributed-tracing/infinite-tracing/introduction-infinite-tracing) and [Sampling considerations](https://docs.newrelic.com/docs/understand-dependencies/distributed-tracing/trace-api/introduction-trace-api#sampling).

To get started using the Trace API, follow one of these paths:

* Want to use [Infinite Tracing](https://docs.newrelic.com/docs/understand-dependencies/distributed-tracing/trace-api/introduction-trace-api#sampling)? Follow the [Set up a trace observer](https://docs.newrelic.com/docs/understand-dependencies/distributed-tracing/infinite-tracing/set-trace-observer#set-up) instructions. That walks you through creating a trace observer and sending a sample payload to the trace observer endpoint.
* Don't want Infinite Tracing? See how to send a [sample payload](#new-relic-quick-start) (below).

## Send sample trace payload (non-Infinite Tracing) 

The following explains how to send a standard (non-[Infinite Tracing](https://docs.newrelic.com/docs/understand-dependencies/distributed-tracing/trace-api/introduction-trace-api#sampling)) payload to the Trace API using our `newrelic` format.

1. Get a <InlinePopover type="licenseKey"/> for the account you want to report data to.
2. Insert that key into the following JSON and then send the JSON to our endpoint. Note: if you have a EU New Relic account, use the [EU endpoint](https://docs.newrelic.com/docs/understand-dependencies/distributed-tracing/trace-api/trace-api-general-requirements-limits#requirements) instead.

   ```bash
   curl -i -H 'Content-Type: application/json' \
       -H 'Api-Key: YOUR_LICENSE_KEY' \
       -H 'Data-Format: newrelic' \
       -H 'Data-Format-Version: 1' \
       -X POST \
       -d '[
               {
                   "common": {
                       "attributes": {
                           "service.name": "Test Service A",
                           "host": "host123.example.com"
                       }
                   },
                   "spans": [
                       {
                           "trace.id": "123456",
                           "id": "ABC",
                           "attributes": {
                               "duration.ms": 12.53,
                               "name": "/home"
                           }
                       },
                       {
                           "trace.id": "123456",
                           "id": "DEF",
                           "attributes": {
                               "error.message": "Invalid credentials",
                               "service.name": "Test Service A",
                               "host": "host456.example.com",
                               "duration.ms": 2.97,
                               "name": "/auth",
                               "parent.id": "ABC"
                           }
                       }
                   ]
               }
           ]' 'https://trace-api.newrelic.com/trace/v1'
   ```

>     If you're sending more than one `POST`, change the `trace.id` to a unique value. Sending the same payload or span `id` multiple times for the same `trace.id` may result in fragmented traces in the UI.

3. If your test returned `HTTP/1.1 202 Accepted`, go to [our UI](https://one.newrelic.com/launcher/distributed-tracing-nerdlets.distributed-tracing?launcher=eyJ0aW1lUmFuZ2UiOnsiYmVnaW5fdGltZSI6bnVsbCwiZW5kX3RpbWUiOm51bGwsImR1cmF0aW9uIjoxODAwMDAwfSwiJGlzRmFsbGJhY2tUaW1lUmFuZ2UiOnRydWV9&pane=eyJuZXJkbGV0SWQiOiJkaXN0cmlidXRlZC10cmFjaW5nLW5lcmRsZXRzLmRpc3RyaWJ1dGVkLXRyYWNpbmctbGF1bmNoZXIiLCJzb3J0SW5kZXgiOjAsInNvcnREaXJlY3Rpb24iOiJERVNDIiwicXVlcnkiOnsib3BlcmF0b3IiOiJBTkQiLCJpbmRleFF1ZXJ5Ijp7ImNvbmRpdGlvblR5cGUiOiJJTkRFWCIsIm9wZXJhdG9yIjoiQU5EIiwiY29uZGl0aW9ucyI6W119LCJzcGFuUXVlcnkiOnsib3BlcmF0b3IiOiJBTkQiLCJjb25kaXRpb25TZXRzIjpbeyJjb25kaXRpb25UeXBlIjoiU1BBTiIsIm9wZXJhdG9yIjoiQU5EIiwiY29uZGl0aW9ucyI6W3siYXR0ciI6InNlcnZpY2UubmFtZSIsIm9wZXJhdG9yIjoiRVEiLCJ2YWx1ZSI6IlRlc3QgU2VydmljZSBBIn1dfV19fX0=) to see a query of your test data using the span attribute `service.name = Test Service A`.

>     Traces may take up to one minute to be processed by both the trace observer and the Trace API.

---

**READ MORE**: This doc is largely unchanged from when I wrote it in 2017. [Read the rest of the doc here](https://docs.newrelic.com/docs/distributed-tracing/trace-api/report-new-relic-format-traces-trace-api).

---

## Example #6: Querying data with NRQL

One project of mine was to improve the New Relic query language (NRQL) docs. NRQL was a SQL-like query language customers could use to query their observability data via the UI or via an API. When I started, the NRQL docs were hard to get started with: they didn’t do a good job explaining at a high level why you’d want to use NRQL, what the major use cases were, and how to quickly get started with it. I created a doc that would make people feel comfortable getting started and that would hopefully provide some value quickly.

In the introductory doc, my goal was to explain: a) common use cases, b) where you could do it, c) an overview of the syntax, and d) the types of data you could query. 

Here’s an excerpt from that doc:  

### Sample section

## What is NRQL?
NRQL is an acronym of New Relic query language. It's a query language similar to ANSI SQL (see the syntax), and you can use it to retrieve detailed New Relic data to get insight into your applications, hosts, and business-important activity. NRQL can help you:

* Create a new chart
* Answer a specific question for the purpose of troubleshooting or business analysis
* Set up NRQL-based alerts (our primary and most powerful type of alert)
* Make API queries of New Relic data (for example, using our NerdGraph API)

You can use NRQL to create simple queries, such as fetching rows of data in a raw tabular form that gives insight on individual events. You can also use NRQL to run powerful calculations on the data before it's presented to you, such as crafting funnels based on how end users interact with your site or application. We use NRQL behind the scenes to generate many of the charts and dashboards in our curated UI experiences:

[IMAGE OF DASHBOARD]
Where can you use NRQL? 
You can use NRQL across the platform to access your data. Those places include:

* The query builder. [screenshot of the query builder] You can run a NRQL query in the platform’s query builder. This NRQL query shows a count of distributed tracing spans faceted by their entity names.
* NRQL-based alerts. [screenshot of NRQL-based alerts UI] You can use NRQL to build NRQL-based alerts, our primary and most powerful alert type. This will help to notify you of issues and help you address them in a timely fashion.

* NerdGraph API. [screenshot of the Nerdgraph API] You can also use NRQL with our NerdGraph API. This gives you more powerful features than querying in the UI (for example, cross-account querying, and asynchronous queries).

---

**READ MORE**: This doc is largely unchanged from when I edited it in 2019. [Read the rest of the doc here](https://docs.newrelic.com/docs/nrql/get-started/introduction-nrql-new-relics-query-language).

---

## Example 7: Go language monitoring agent APIs

New Relic’s core feature is application performance monitoring (APM). This was handled by installable agents available for several coding languages (Go, Ruby, Java, .NET, Python, PHP, Node.js). I worked on all of these docs over the years, with a special focus on Go, .NET, and Python. Work in these areas included documenting installation, configuration, data explanations, common use cases, and code snippets. 

One of my early assignments was writing the Go language agent docs, which was the first language agent they’d added in years (and ended up being their last). Each language agent had their own library of APIs that allowed customers to customize the agent, to get it to work how they wanted it to work. 
Here’s a sample from one of the Go agent APIs: 

## Sample section

## Guide to using the Go agent API

The [New Relic Go agent](https://docs.newrelic.com/docs/agents/go-agent/get-started/introduction-new-relic-go) monitors your Go language applications and microservices to help you identify and solve performance issues. The Go agent API is one of several available [New Relic APIs](https://docs.newrelic.com/docs/apis/getting-started/introduction-new-relic-apis).

> Because Go applications run from a compiled, native binary file, you need to [manually instrument your code](https://docs.newrelic.com/docs/agents/go-agent/get-started/instrument-go-transactions) to monitor transactions for your Go applications by adding New Relic methods to it.

## Monitor transactions 

Before you manually instrument your code to monitor [transactions](https://docs.newrelic.com/docs/apm/transactions/intro-transactions/transactions-new-relic-apm), make sure that you meet the [compatibility and requirements](https://docs.newrelic.com/docs/agents/go-agent/get-started/go-agent-compatibility-requirements) and that you are using the [latest version of the Go agent](https://docs.newrelic.com/docs/release-notes/agent-release-notes/go-release-notes).

| If you want to... | Use this method... |
|------------------|-------------------|
| Start timing a transaction | [`StartTransaction()`](https://docs.newrelic.com/docs/agents/go-agent/get-started/instrument-go-transactions#go-txn) |
| Stop timing a transaction | [`txn.End()`](https://docs.newrelic.com/docs/agents/go-agent/get-started/instrument-go-transactions#go-txn) |
| Prevent a transaction from reporting to New Relic | [`Ignore()`](https://godoc.org/github.com/newrelic/go-agent/v3/newrelic#Transaction.Ignore) |
| Prevent an active transaction from reporting Apdex to New Relic | [`IgnoreApdex()`](https://godoc.org/github.com/newrelic/go-agent/v3/newrelic#Transaction.IgnoreApdex) |
| Use the standard HTTP library package to monitor transactions | [HTTP request wrapping](https://docs.newrelic.com/docs/agents/go-agent/get-started/instrument-go-transactions#http-handler-txns) |

## Time specific methods using segments 

If a transaction is already visible in New Relic, but you do not have enough data about a particular method that was called during that transaction, you can create [segments](https://docs.newrelic.com/docs/agents/go-agent/get-started/instrument-go-segments). For example, if you want to time a method that has complex logic, you can create a segment for each of the methods in the transaction.

To instrument a method within an existing transaction, create segments for the following:

* [Blocks of code](https://docs.newrelic.com/docs/agents/go-agent/get-started/instrument-go-segments#segment-code-block)
* [Functions](https://docs.newrelic.com/docs/agents/go-agent/get-started/instrument-go-segments#segment-function)
* [Datastores](https://docs.newrelic.com/docs/agents/go-agent/get-started/instrument-go-segments#go-datastore-segments)
* [External services](https://docs.newrelic.com/docs/agents/go-agent/get-started/instrument-go-segments#go-external-segments)

If the work is happening in a different goroutine from where the transaction started, you must use the [`NewGoroutine()`](/docs/agents/go-agent/features/tracing-asynchronous-applications) API.

---

**READ MORE**: This doc is largely unchanged from when I wrote it in 2017. [Read the rest of the doc here](https://docs.newrelic.com/docs/apm/agents/go-agent/api-guides/guide-using-go-agent-api).

---

## More samples

If you’d like to see more writing samples from my time at New Relic, let me know. I have many more I could share. 

A note about my time at Amazon: unfortunately, most of my work for the Amazon Ads API department was spent on internal docs for API designers and API consumers, and I can't share this publicly. That's unfortunate, as I was proud of helping a large internal audience build and consume APIs more efficiently. 

You can [find my GitHub commits here](https://github.com/zuluecho9?tab=overview&from=2023-12-01&to=2023-12-31). Those commits are from my final 2.5 years or so at New Relic, ending in late 2023. 

## Content marketing examples

Over the years, I’ve done quite a bit of freelance content marketing work for various tech companies. This work has included blog posts, white papers, case studies, guides, and the like. The goals were generally a) to gather online traffic/leads, and b) to communicate expertise and trustworthiness in the chosen domain.

Examples:

* [Hydrolix log storage](#hydrolix-log-storage)
* [Spire satellite data](#spire-satellite-data)

### Hydrolix log storage

Hydrolix is a streaming data-lake solution designed for log storage and analytics. In 2025, I wrote several blog posts for them aimed at gathering more leads from companies with
high-volume logs. This included a focus on the security-related benefits of advanced log parsing and analytics. This work involved me working side-by-side with marketing team members to arrive at optimal SEO approaches for titles and keywords.

Pieces I wrote for Hydrolix:

* [Unlocking threat-hunting insights from high-volume network logs](https://hydrolix.io/blog/threat-hunting-insights/)
* [Log management: A detailed guide](https://hydrolix.io/blog/log-management-guide/)
* [Best practices for monitoring CDN security](https://hydrolix.io/blog/cdn-security-monitoring-best-practices/)


### Spire satellite data

Spire is a satellite company and a satellite data company. Between 2018 and 2021, I wrote roughly a dozen pieces for them, aimed at demonstrating expertise and thought leadership in several domains, including agriculture applications, maritime management applications, and aviation applications. This work involved a lot of research on my part: learning how satellite data was being used, and might be used, to improve various systems and workflows.

I also helped them overhaul their website and write copy for all major components/sections of their new site (although the site has been overhauled again since I did that work).

Here are a few of the resources I created for Spire:

*​ [White paper: An Ocean of Data: The digital revolution and its ongoing impact on maritime industries](https://spire.com/wp-content/uploads/2020/02/An-Ocean-of-Data-The-digital-Revolution.pdf)
*​ [Case study: TTEK uses Spire to improve their aviation products](https://spire.com/case-study/aviation/powering-the-threat-matrix/)
* [Blog post: As renewable energy grows, so does demand for weather data and analytics](https://spire.com/blog/weather-climate/as-renewable-energy-grows-so-does-demand-for-weather-data-and-analytics)
* [Blog post: Top 5 reasons you should be using specialized agriculture weather forecasts](https://spire.com/blog/weather-climate/top-5-reasons-you-should-be-using-specialized-agriculture-weather-forecasts)


## Coding and scripting experience 

I'm far from a professional coder but I have strong general knowledge of software development and deployment. My best language is Python, but I've documented and written code examples for many languages, application frameworks, and types of APIs (with most of that experience coming from my time at New Relic, due to the full-stack breadth of their offerings). AI/LLM tools have dramatically improved my ability to write scripts/code to solve specific technical challenges. 

As evidence of my skills and comfort with coding, check out a [personal coding project](www.linkedin.com/feed/update/urn:li:activity:7401999440531705856) of mine, which involves video and computer-vision algorithms.  


