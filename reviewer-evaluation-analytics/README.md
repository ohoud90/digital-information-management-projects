# Reviewer Evaluation Analytics – Power BI

## Overview | نبذة

This case study documents two interactive Power BI reporting views developed for reviewer-evaluation analysis. The portfolio version uses a synthetic model representing **32 training facilities across 13 administrative regions** and discloses no real facility, reviewer, or organizational data.

توثق دراسة الحالة واجهتين تفاعليتين في Power BI لتحليل تقييم المراجعين. تستخدم نسخة المحفظة نموذجًا اصطناعيًا يمثل **32 منشأة تدريبية موزعة على 13 منطقة إدارية**، من دون الإفصاح عن بيانات منشآت أو مراجعين أو جهات حقيقية.

## Analytical Workflow | سير التحليل

1. Import and profile source tables.
2. Clean labels, dates, and category fields in Power Query.
3. Build one-to-many relationships.
4. Create DAX measures for counts, averages, completion, and variance.
5. Design KPI cards, maps, comparisons, and hierarchical filters.
6. Validate Power BI totals against Excel PivotTables.
7. Review privacy, filter context, and publication readiness.

## Example Measures | أمثلة المقاييس

```DAX
Total Evaluations = COUNTROWS(Evaluations)

Average Rating = AVERAGE(Evaluations[Rating])

Completion Rate =
DIVIDE(
    CALCULATE(COUNTROWS(Evaluations), Evaluations[Status] = "Completed"),
    COUNTROWS(Evaluations),
    0
)

Remaining Evaluations = [Target Evaluations] - [Total Evaluations]
```

## Dashboard Components | مكونات اللوحة

- KPI cards for total evaluations, facilities, reviewers, and completion.
- Regional and geographic distribution.
- Trend and comparison visuals.
- Hierarchical slicers for region, facility, role, and period.
- Detail tables for controlled investigation.
- Excel PivotTable reconciliation.

## Outcome | النتيجة

A validated management-reporting workflow that converts detailed evaluation records into clear indicators, geographic views, comparisons, and decision-support insights.

## Public Assets | الملفات العامة

- `sample-data/evaluation_sample.csv`: synthetic demonstration records.
- Screenshots and a `.pbix` demonstration model will be added only after full privacy review.

