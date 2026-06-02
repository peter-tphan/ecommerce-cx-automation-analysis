# eCommerce CX Automation Analytics Case Study

A real take home case study focused on eCommerce customer service automation, Week 1 performance diagnosis, customer communication, and implementation readiness.

This repository shows how I approached the case as an end to end analytics project, moving from client discovery to Python based data audit, dashboard storytelling, root cause interpretation, and OMS readiness review.

The original branded take home brief and full OMS reference document are not included in this public repository because they were provided as assessment materials. The relevant task requirements are summarised below so the project can be reviewed without the original documents.

## 🔎 How to Review This Project

For a quick review, open the files in this order:

| Step | File                                       | What to look for                                                                                                 |
| ---- | ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| 1    | `Presentation_Case_Deck.pdf`               | Final case response, client discovery framework, dashboard views, root cause findings, and launch readiness plan |
| 2    | `Python_Analysis_Notebook.html`            | Python workflow, data audit, KPI validation, scatter plot, matrix logic, and chart outputs                       |
| 3    | `Raw_data.xlsx`                            | Original dataset used for Week 1 performance analysis                                                            |
| 4    | `Cleaned_Data.csv`                         | Cleaned dataset prepared for Python analysis                                                                     |
| 5    | `Willy_Wonka_Candy_Factory_Case_Study.pdf` | Supporting API scenario context for the OMS integration section                                                  |

## 🎯 Case Objective

The case asked for a structured response to a new eCommerce automation launch.

The task covered three areas:

| Area   | What the task required                                                                                       |
| ------ | ------------------------------------------------------------------------------------------------------------ |
| Part 1 | Define the top five things to understand about an incoming brand before implementation                       |
| Part 2 | Analyse Week 1 automation performance using customer intent volume, automation rate, and repeat contact data |
| Part 3 | Review whether a custom OMS API was ready for integration and identify possible data or endpoint gaps        |

The case was not only about producing charts. The expected output had to explain what the data meant, how to share concerning findings with the customer, and how to prepare the team for a successful implementation.

## 🧠 My Case Approach

I treated the case as a customer success analytics problem with three connected layers:

| Layer                    | Purpose                                                                                                          |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| Client discovery         | Understand the brand, goals, pain points, success metrics, technical stack, and internal ownership before launch |
| Performance diagnosis    | Use Python to audit Week 1 data, validate KPIs, and identify where automation was helping or failing             |
| Implementation readiness | Review OMS data requirements and translate API gaps into practical launch considerations                         |

## 🏁 Part 1: Client Discovery Framework

For the client discovery section, I created a Formula 1 inspired framework called **The Five Essentials**.

| Framework element   | What it represented                                                                        |
| ------------------- | ------------------------------------------------------------------------------------------ |
| Car Blueprint       | Business model, customer journey, launch goals, and expected outcomes                      |
| Engine Temperature  | Service pain points, current pressure points, customer friction, and urgency               |
| Dashboard           | Success metrics, ROI expectations, reporting needs, and how performance should be measured |
| Powertrain          | Technical stack, OMS setup, integration readiness, and data availability                   |
| Driver and Pit Crew | Internal ownership, escalation routes, team responsibilities, and operating constraints    |

This structure helped turn a broad discovery question into a practical implementation readiness checklist.

The main idea was simple: data gives direction, empathy builds trust, and integration drives performance.

## 🧪 Part 2: Performance Data Investigation

Part 2 focused on Week 1 automation performance.

I used Python to audit the data, validate the logic, and create visual outputs that could explain the situation clearly to a customer success or implementation team.

Key questions included:

1. Which intents carried the most volume?
2. Which flows had low automation coverage?
3. Which flows still created repeat contact after automation?
4. Which areas should be fixed, monitored or replicated?
5. How should the findings be shared with the customer without damaging trust?

### Data work completed

| Step                 | What I did                                                                                                     |
| -------------------- | -------------------------------------------------------------------------------------------------------------- |
| Data review          | Checked the raw dataset structure, column names, field formats, and percentage values                          |
| Data cleaning        | Normalised percentage fields and prepared the dataset for analysis                                             |
| Category filtering   | Removed non actionable records such as total rows or non service categories that could distort the analysis    |
| KPI validation       | Checked automation rate, total volume, automated volume, repeat contact rate, and channel level repeat contact |
| Analysis preparation | Created clean outputs that could support ranked charts, scatter plots, and quadrant views                      |

### Python methods used

| Tool or method | How it was used                                                                                    |
| -------------- | -------------------------------------------------------------------------------------------------- |
| Python         | Main analysis environment for data audit, KPI checks, and visual output generation                 |
| pandas         | Loaded datasets, cleaned columns, converted fields, filtered records, and prepared analysis tables |
| NumPy          | Supported numerical handling and KPI calculations                                                  |
| Matplotlib     | Created ranked charts and visual outputs for the presentation deck                                 |
| Seaborn        | Supported cleaner visual styling and comparison views                                              |
| Excel          | Reviewed raw data and supported pivot or lookup style validation before and after Python analysis  |

### Dashboard and visual analysis

The final deck translated the Python outputs into a business friendly dashboard structure.

It included:

1. KPI summary cards
2. Ranked volume charts
3. Automation rate analysis
4. Repeat contact analysis by channel
5. Overall repeat contact volume
6. Scatter plot style comparison of automation rate and repeat contact rate
7. Intent opportunity matrix
8. Recontact opportunity matrix
9. Quadrant views to separate high volume, low automation, high repeat contact, and stronger performing flows
10. Priority areas for customer success follow up

## 📊 Key Insight Logic

A high automation rate does not automatically mean a service flow is performing well.

The analysis compared automation rate with total volume and repeat contact behaviour to check whether automation was actually reducing customer effort.

This helped separate:

| Group               | Meaning                                                                                            |
| ------------------- | -------------------------------------------------------------------------------------------------- |
| Working flows       | High volume or useful automation with low repeat contact                                           |
| Watchlist flows     | Flows that needed closer tracking before making major changes                                      |
| Fix first flows     | High volume or high repeat contact flows that needed clearer scripts, routing, or escalation logic |
| Replicable patterns | Stronger flows that could provide useful design patterns for other journeys                        |

The core analyst judgement was to avoid relying on a single surface level KPI. The analysis looked for cases where a flow appeared efficient but still created avoidable customer follow up.

## 🔗 Part 3: OMS Integration Readiness

Part 3 reviewed whether the custom OMS information was sufficient for a smooth implementation.

The focus was not just to list missing fields. I reviewed how the available API information would support customer conversations, order lookups, cancellation handling, fulfilment updates, and tracking responses.

### OMS areas reviewed

| OMS area                 | Why it mattered                                                                                  |
| ------------------------ | ------------------------------------------------------------------------------------------------ |
| Account lookup           | Needed to identify the caller and connect them to the correct customer record                    |
| Order lookup             | Needed to retrieve the correct order and avoid wrong customer handling                           |
| Order and payment status | Needed to explain whether an order was paid, pending, cancelled, or still in progress            |
| Cancellation reasons     | Needed to understand why an order was cancelled and how to respond accurately                    |
| Fulfilment status        | Needed to answer delivery, shipping, and order progress questions                                |
| Tracking information     | Needed to support Where Is My Order style conversations                                          |
| Item level data          | Needed to confirm which product, variant, quantity, or order item the customer was calling about |
| Error handling           | Needed to manage invalid API keys, missing records, and failed lookup scenarios                  |

### Integration review output

The case response included:

1. A gap review of the customer API documentation against expected OMS requirements
2. A practical view of which fields or endpoints would affect customer experience
3. A timeline approach for acknowledging the customer quickly while allowing enough time for detailed gap analysis
4. A launch readiness view connecting technical gaps to customer success and implementation planning

## 📁 Repository Files

| File                                       | Description                                                                                                                                 |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------- |
| `Presentation_Case_Deck.pdf`               | Final case deck covering client discovery, performance analysis, dashboard views, root cause findings, and implementation readiness         |
| `Python_Analysis_Notebook.html`            | Exported Python notebook showing the data audit, KPI validation, filtering logic, scatter plot logic, quadrant analysis, and visual outputs |
| `Raw_data.xlsx`                            | Original Week 1 performance dataset used for the case analysis                                                                              |
| `Cleaned_Data.csv`                         | Cleaned dataset prepared for Python analysis                                                                                                |
| `Willy_Wonka_Candy_Factory_Case_Study.pdf` | Supporting API scenario context for the OMS integration section                                                                             |

## ✅ What This Project Demonstrates

This project demonstrates my ability to:

1. Structure an ambiguous business case into clear workstreams
2. Use Python to audit, clean, validate, and analyse performance data
3. Work with messy percentage fields and reporting logic before drawing conclusions
4. Create dashboard ready outputs using KPI cards, ranked charts, scatter plots, and quadrant views
5. Identify root causes behind repeat customer contact
6. Translate analytics into a clear executive case deck
7. Connect customer success, data analytics, and implementation readiness
8. Communicate findings in a way that is useful for technical and non technical stakeholders

## 🔗 Relevance to Data Analyst Roles

Although the case focuses on eCommerce customer service automation, the analytical logic is transferable to data analyst roles involving payment, checkout, fraud, chargeback, order journey, or operational performance analysis.

The same approach can be applied when teams need to:

1. Validate reporting logic before using a dashboard
2. Investigate unexpected movements in performance metrics
3. Compare multiple KPIs instead of relying on a single headline number
4. Detect hidden friction behind surface level performance
5. Build dashboard views that support decision making
6. Explain root causes to business stakeholders
7. Turn ad hoc analysis into structured reporting outputs

## 🔐 Public Repository Notes

This is a public portfolio version.

The repository does not include the original branded take home brief or the full OMS reference document because those were provided as assessment materials.

The relevant task requirements and integration considerations have been summarised in this README and reflected in the final case deck. The uploaded files are intended to show the analysis workflow, the final presentation output, and the supporting scenario context.
