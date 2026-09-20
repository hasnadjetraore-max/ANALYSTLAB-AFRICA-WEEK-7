# 🏥 HealthConnect — Financial Due Diligence & Predictability Roadmap

## 📌 Executive Overview
This project delivers a rigorous **Financial Due Diligence** and **Data Integrity Audit** for the *HealthConnect* clinical appointment management system. 

By auditing historical appointment data and optimizing a 5-page interactive Power BI dashboard, this study quantifies the direct revenue loss caused by patient absenteeism (No-Show) and establishes an actionable investment roadmap to recover lost revenue prior to machine learning integration.

---

## 💡 Key Financial Findings & Business Impact

* **Global No-Show Rate:** **48.46%** (3,877 unhonored appointments out of 8,000).
* **Direct Revenue Loss:** **73M FCFA** in lost billing opportunities.
* **Direct Idle Resource Cost:** **36M FCFA** in unutilized clinical time slots.
* **Recoverable Revenue Target:** **11M FCFA** under a conservative **15% reduction** scenario in patient absenteeism.

---

## 🔍 Top 5 Validated Risk Drivers (Features)

1. **`previous_no_shows` (Historical Recidivism):** The single strongest behavioral predictor. No-Show rate approaches **100%** for patients with $\ge 3$ past absences.
2. **`booking_lead_days` (Booking Lead Time):** Sharp decline in commitment as lead time increases:
   * `0–3 days`: **24.84%** No-Show
   * `>14 days`: **54.36%** No-Show *(Key policy threshold)*
3. **`distance_to_clinic_km` (Geographic Friction):** Peak absenteeism observed at **51.91%** for patients residing **>15 km** from the clinic.
4. **`reminder_channel` (Engagement Channel):** Identifies passive channels vs. interactive channels (WhatsApp) suitable for automated recall triggers.
5. **`age_group` (Demographic Control):** Used to adjust communication channels by demographic behavior.


In accordance with technical audit standards, data model integrity was verified through systematic testing:

```text
[TEST] -> [FINDING] -> [ACTION] -> [RETEST] -> [VALIDATED IMPROVEMENT]
