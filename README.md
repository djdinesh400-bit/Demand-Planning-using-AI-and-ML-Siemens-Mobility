# 🚆 Demand Planning Using AI & Machine Learning

## 📌 Project Overview

**Demand Planning Using AI & Machine Learning** is a Supply Chain Analytics case study focused on exploring how **Artificial Intelligence (AI) and Machine Learning (ML)** can improve demand forecasting and decision-making in project-based rail infrastructure environments.

Using **Siemens Mobility** as the case study context, the project examines the challenges associated with forecasting demand in rail infrastructure, where demand is influenced by **long lead times, government funding cycles, infrastructure investment, project-based orders, and other external factors**.

The analysis compares traditional forecasting approaches with AI/ML-based methods and explores how the integration of **internal ERP data, backlog information, operational signals, and external economic and policy indicators** can improve demand planning.

The project also examines the **Bullwhip Effect**, feature engineering, machine learning techniques, probabilistic forecasting, S&OP integration, governance, and implementation considerations.

The overall objective is not to eliminate uncertainty, but to enable **structured and defensible management of forecast uncertainty** through AI-augmented decision-making.

---

## 🎯 Key Objectives

- Understand demand planning within project-based rail infrastructure.
- Analyze the challenges associated with long-term and uncertain demand.
- Examine the limitations of traditional forecasting methods.
- Understand the **Bullwhip Effect** and the impact of information asymmetry.
- Explore AI and Machine Learning approaches to demand forecasting.
- Compare traditional forecasting with AI/ML-based demand planning.
- Identify internal and external features that can influence rail demand.
- Examine the role of backlog, lead times, production capacity, and historical demand.
- Incorporate external signals such as infrastructure spending, policy changes, macroeconomic indicators, and commodity prices.
- Explore machine learning techniques including **ARIMA, Random Forest, XGBoost, and LSTM**.
- Understand probabilistic forecasting and forecast uncertainty.
- Examine the integration of AI forecasting into **Sales & Operations Planning (S&OP)**.
- Identify governance, explainability, data quality, and change management requirements.
- Evaluate performance metrics relevant to demand planning.
- Demonstrate how AI can augment planners rather than replace human decision-making.

---

## 🔬 Methodology

### 1. Business Context Analysis

The case study begins by examining the demand environment of **Siemens Mobility**, with particular focus on rail infrastructure.

The analysis identifies several structural characteristics:

- Project-based demand
- Long lead times
- Government dependency
- High-value and customized requirements
- Structural uncertainty

Major rail infrastructure components may have lead times of **18–36 months**, while public funding cycles and infrastructure investment programmes can significantly influence demand.

---

### 2. Demand Planning Analysis

The project examines demand planning across the **demand-to-delivery chain**:

```text
Forecast
   ↓
Production Planning
   ↓
Procurement
   ↓
Inventory
   ↓
Delivery
   ↓
Financial Performance
```

Forecast errors can result in:

- Excess inventory
- Higher working capital costs
- Backlog accumulation
- Unmet demand and delivery delays
- Service-level risk
- Supplier instability
- Reactive procurement costs

---

### 3. Bullwhip Effect Analysis

The project examines the **Bullwhip Effect**, where relatively small changes in customer demand can create increasingly larger fluctuations upstream in the supply chain.

The **Beer Game** is used as a conceptual supply chain simulation to demonstrate the effect of information visibility.

Two scenarios are considered:

**Round 1 — No Demand Visibility**

- High backlog accumulation
- Large inventory swings
- Excessive ordering amplification
- Higher total supply chain cost

**Round 2 — Demand Shared**

- Stable backlog levels
- Smoother inventory transitions
- Reduced ordering overreaction
- Lower total supply chain cost

The case study highlights that improved information flow can reduce supply chain instability and provides a rationale for AI-driven demand forecasting.

---

### 4. Traditional Forecasting Analysis

The project evaluates several traditional demand forecasting approaches:

| Method | Approach | Best Suited For |
|---|---|---|
| **ARIMA** | Uses historical demand and lagged error terms | Stable, linear time-series data |
| **Exponential Smoothing** | Weighted average of recent observations | Short-term forecasts with trend/seasonality |
| **Planner Judgment** | Uses planner knowledge and market conditions | Low-data environments and qualitative signals |
| **Safety Stock Buffers** | Inventory buffer based on demand variability | Hedging against forecast uncertainty |

A key limitation identified is that traditional approaches primarily depend on historical demand patterns and assume relative stability over time.

This creates challenges when demand is influenced by structural external factors such as:

- Government budget cycles
- Infrastructure investment programmes
- Macroeconomic conditions
- Policy changes

---

### 5. Machine Learning Techniques

The case study examines four forecasting approaches:

#### ARIMA

Used as a traditional time-series baseline.

- Uses past demand and lagged errors
- Assumes linear time-series relationships
- Suitable for stationary and seasonal data
- Provides a benchmark for ML comparison

#### Random Forest

An ensemble learning approach that combines multiple decision trees.

- Captures nonlinear relationships
- Handles complex structured data
- Robust to noisy data
- Provides interpretable feature importance

#### XGBoost

A gradient boosting approach based on sequential error correction.

- Strong performance on structured/tabular data
- Suitable for ERP and backlog-related features
- High predictive capability
- Widely applicable to business forecasting problems

#### LSTM

A deep learning approach using neural network memory cells.

- Learns long-term sequences
- Captures temporal dependencies
- Suitable for long-range demand patterns
- Requires larger amounts of training data

---

### 6. AI vs. Traditional Forecasting

The project compares traditional forecasting with AI/ML-based approaches across several dimensions:

| Dimension | Traditional Methods | AI / ML Approach |
|---|---|---|
| **Data Inputs** | Historical demand | Historical + external + backlog signals |
| **Relationship Type** | Linear, additive | Nonlinear, interaction effects |
| **Structural Shifts** | Poor detection | Improved through feature engineering |
| **Output** | Point estimate | Probabilistic forecast distribution |
| **Bias Handling** | Manual correction | Data-driven bias reduction |
| **Learning Over Time** | Static parameters | Model retraining using new data |

The analysis positions AI/ML as an **extension** of traditional forecasting rather than a complete replacement.

---

### 7. Feature Engineering

Feature engineering focuses on combining internal operational data with external demand signals.

#### Internal Features

- **Backlog Size** — Volume of undelivered orders
- **Order Frequency** — Rate of new project order arrivals
- **Lead-Time Variability** — Fluctuations in supplier delivery times
- **Production Capacity** — Available manufacturing capacity
- **Historical Demand** — Lagged demand patterns

#### External Features

- **Infrastructure Spending Index** — Government capital expenditure commitments
- **Policy & Regulatory Signals** — Tender announcements and budget cycles
- **Macroeconomic Indicators** — GDP growth and construction indicators
- **Commodity Prices** — Steel and copper price signals
- **Customer Project Milestones** — Contractual delivery windows

The case study emphasizes that model quality depends heavily on feature quality, particularly in project-based rail demand environments.

---

### 8. AI-Enhanced Demand Planning

The project identifies several ways AI can improve demand planning:

- Capture nonlinear relationships between demand drivers.
- Integrate multiple internal and external signals.
- Reduce systematic forecast bias.
- Detect structural shifts in demand.
- Generate probabilistic forecasts.
- Support structured management of forecast uncertainty.

The focus is therefore not solely on achieving perfect forecast accuracy, but on providing decision-makers with better information about **uncertainty and risk**.

---

### 9. S&OP Integration & Governance

The case study proposes integrating AI forecasting into the **Sales & Operations Planning (S&OP)** process.

The proposed decision-support structure consists of:

```text
Data Layer
     ↓
Model Layer
     ↓
Decision Layer
     ↓
S&OP Planning
```

The governance principle is that AI should function as a **decision-support tool rather than an autonomous system**.

Planners retain:

- Forecast ownership
- Decision accountability
- Validation responsibility

Model outputs should also be interpretable and explainable to build planner trust.

---

### 10. Performance Metrics

The case study identifies several performance indicators for evaluating demand planning:

- Forecast Bias
- MAPE (Mean Absolute Percentage Error)
- Service Level %
- Working Capital
- Backlog Reduction

These metrics provide a broader view of forecasting performance by connecting model accuracy with operational and financial outcomes.

---

### 11. Implementation Considerations

The project identifies four major implementation areas:

#### Data Quality & Integration

- ERP data may be incomplete or siloed.
- External data requires curation.
- Data governance requires early investment.

#### Change Management

- Planners may initially distrust model outputs.
- Training and pilot programmes are important.
- Early measurable results can support adoption.

#### Model Interpretability

- Black-box models can reduce planner trust.
- Explainability techniques such as SHAP can be used.
- Transparent model logic supports governance.

#### Governance Structure

- Define ownership of model validation.
- Establish a review cadence within the S&OP cycle.
- Document decision trails for auditability.

---

## 🛠️ Technologies & Analytical Methods

| Technology / Method | Purpose |
|---|---|
| 🤖 Artificial Intelligence | Demand planning and decision-support |
| 🧠 Machine Learning | Demand forecasting and pattern detection |
| 📈 ARIMA | Time-series forecasting baseline |
| 🌲 Random Forest | Nonlinear structured-data modelling |
| 🚀 XGBoost | Gradient boosting and tabular forecasting |
| 🧠 LSTM | Deep learning for temporal patterns |
| 🔧 Feature Engineering | Integration of internal and external demand signals |
| 📊 Probabilistic Forecasting | Forecast uncertainty and risk assessment |
| 🔄 S&OP | Operational planning and governance |
| 🔍 SHAP / Explainability | Model interpretation and planner trust |

---

## 🔄 Project Workflow

```text
Rail Infrastructure Business Context
                ↓
       Demand Planning Analysis
                ↓
        Forecast Error Analysis
                ↓
         Bullwhip Effect
                ↓
     Traditional Forecasting
                ↓
       AI / ML Approaches
                ↓
        Feature Engineering
                ↓
 Internal + External Signal Integration
                ↓
      Probabilistic Forecasting
                ↓
       Performance Metrics
                ↓
          S&OP Integration
                ↓
     Governance & Explainability
                ↓
       Strategic Decision Support
```

---

## 📂 Repository Contents

| File | Description |
|---|---|
| `Demand Planning using AI & ML_Case Study Siemens_Mobility(1).pdf` | Complete Siemens Mobility demand planning case study |
| `README.md` | Project documentation |

> **Note:** The repository contents listed above reflect the material provided for this project. Additional notebooks, datasets, source code, or presentation files can be added to this section if they are included in the GitHub repository.

---

## 🔎 Key Analytical Themes

The project explores demand planning through the following themes:

- 🚆 Rail infrastructure demand
- 📦 Supply chain analytics
- 📈 Demand forecasting
- 🤖 Artificial Intelligence
- 🧠 Machine Learning
- 🔄 Bullwhip Effect
- 📊 Traditional forecasting
- 🌲 Random Forest
- 🚀 XGBoost
- 🧠 LSTM
- 📉 ARIMA
- 🔧 Feature engineering
- 🏭 ERP and operational data
- 🌍 External economic signals
- 🏛️ Government infrastructure investment
- 📋 Policy and regulatory signals
- 💰 Working capital
- 🔄 Backlog management
- 📐 Probabilistic forecasting
- 🎯 Forecast bias
- 📊 MAPE
- 🤝 Sales & Operations Planning (S&OP)
- 🔍 Explainable AI
- 🛡️ AI governance
- 👥 Planner decision support
- ⚠️ Forecast uncertainty management

---

## ⚠️ Limitations

This project is primarily a **case study and conceptual analysis** of AI-enabled demand planning.

The provided material discusses machine learning techniques, features, forecasting approaches, performance metrics, and implementation considerations, but it does **not** document a completed model-training experiment with a specific dataset and reported model performance.

Therefore:

- The project should not be interpreted as a validated production forecasting system.
- No specific model accuracy results are presented.
- No direct comparison of ARIMA, Random Forest, XGBoost, and LSTM using a common dataset is reported.
- The identified features represent potential demand signals rather than demonstrated causal drivers.
- External data sources would require appropriate data quality checks and governance before implementation.
- Forecasting performance depends on the quality, availability, and timeliness of the underlying data.
- AI/ML models should be treated as decision-support tools rather than autonomous decision-makers.

The case study emphasizes that uncertainty cannot be completely eliminated in project-based rail supply chains; instead, it should be managed in a structured and defensible manner.

---

## 🏁 Conclusion

This project demonstrates how **Artificial Intelligence and Machine Learning** can augment demand planning in complex, project-based rail supply chains.

The analysis progresses from understanding the business context and limitations of traditional forecasting to exploring AI/ML techniques, feature engineering, probabilistic forecasting, performance measurement, S&OP integration, and governance.

A central finding of the case study is that AI can expand demand planning beyond historical demand by combining **internal operational signals** with **external economic, infrastructure, and policy information**.

The project also emphasizes that successful AI adoption requires more than model development. Data quality, explainability, planner trust, governance, and integration into existing S&OP processes are critical for turning analytical outputs into actionable business decisions.

The strategic perspective can be summarized as:

```text
Business Context → Demand Signals → Feature Engineering → AI/ML Forecasting → Uncertainty Management → S&OP Decision Support → Governed Business Action
```

Ultimately, the objective is **not to replace planners with AI**, but to **augment planner decision-making** with better information, broader signals, and structured management of uncertainty.
