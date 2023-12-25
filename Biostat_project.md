Mortality predictors in hematological patients, admitted to intensive
care unit: a single-centre observational study
================
Sergei Vladimirov
2023-12-25

# Abstract

Purpose: Previous research showed conflicting results about mortality
predictors in critically ill patients with hematological malignancies
(HM). The primary aim of this study was to determine mortality in
critically ill patients with HM in intensive care unit (ICU) and to
reveal risk factors predicting the outcome.

Methods and materials: All patients with HM admitted to ICU at our
hospital during 1 year were enrolled. Clinical data upon ICU admission
was collected and then outcomes were estimated.

Results: ICU mortality was 52% among 98 HM patients. According to
multivariate analysis, male sex (OR 2.75, CI: 1.15–6.88, p = 0.026),
high SOFA score (OR 1.30, CI: 1.07–1.62, p = 0.012) and high Charlson
Comorbidity Index (OR 1.30, CI: 1.06–1.64, p = 0.016) were associated
with the outcome.

Conclusion: We found three independent predictors for ICU mortality.
Further research is needed to validate current findings and reveal new
mortality predictors in critically ill HM patients.

# Introduction

Patients with hematologic malignancies (HMs) have an increased risk of
death compared to other oncology patients in settings of intensive care
unit (ICU). According to previous research1, the predictive value of
different admission factors is constantly changing, and several studies
on this topic have conflicting results. Our research question is
addressed to identifying factors in the condition of hematological
patients that can predict a poor ICU outcome. The primary aim of this
study was to determine ICU mortality and risk factors predicting the
outcome of critically ill patients with HMs. We hypothesized that there
are some significant factors in the condition of HM patients at the
moment of ICU admission that are associated with mortality.

# Methods

Our research is an observational, single-center study. We
retrospectively evaluated baseline characteristics of adult HM patients
non-electively admitted to the medical ICU of our hospital from July 1,
2022 to June 30,2023. All the HM diagnoses were based on the
pathological examination results or medical records. All data were
obtained from a local ICU electronic database. Cases with a critical
amount of missing data, as well as those who died or transferred to the
floor within 24 hours were excluded from the study.

<table>
<thead>
<tr>
<th style="text-align:left;">
variable
</th>
<th style="text-align:left;">
definition
</th>
<th style="text-align:left;">
type
</th>
<th style="text-align:left;">
status
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
id
</td>
<td style="text-align:left;">
anonymized identical number of patient
</td>
<td style="text-align:left;">
numerical
</td>
<td style="text-align:left;">
independent
</td>
</tr>
<tr>
<td style="text-align:left;">
gender
</td>
<td style="text-align:left;">
gender of patient
</td>
<td style="text-align:left;">
categorical, binary
</td>
<td style="text-align:left;">
independent
</td>
</tr>
<tr>
<td style="text-align:left;">
age
</td>
<td style="text-align:left;">
age of patient
</td>
<td style="text-align:left;">
numerical, years
</td>
<td style="text-align:left;">
independent
</td>
</tr>
<tr>
<td style="text-align:left;">
cci
</td>
<td style="text-align:left;">
Charlson Comorbidity Index - most widely used scoring system for
comorbidities
</td>
<td style="text-align:left;">
numerical, points
</td>
<td style="text-align:left;">
independent
</td>
</tr>
<tr>
<td style="text-align:left;">
diagnosis
</td>
<td style="text-align:left;">
type of hematological malignancy
</td>
<td style="text-align:left;">
categorical
</td>
<td style="text-align:left;">
independent
</td>
</tr>
<tr>
<td style="text-align:left;">
disease_status
</td>
<td style="text-align:left;">
status of HM progression
</td>
<td style="text-align:left;">
categorical: p (progression) - relapsed or refractory disease, n - newly
diagnosed
</td>
<td style="text-align:left;">
independent
</td>
</tr>
<tr>
<td style="text-align:left;">
days_bfr_icu
</td>
<td style="text-align:left;">
number of days in hospital before admission to ICU
</td>
<td style="text-align:left;">
numerical, days
</td>
<td style="text-align:left;">
independent
</td>
</tr>
<tr>
<td style="text-align:left;">
sofa
</td>
<td style="text-align:left;">
sequential organ failure assessment score (SOFA score), is used to
determine the extent of organ function or rate of failure
</td>
<td style="text-align:left;">
numerical, points
</td>
<td style="text-align:left;">
independent
</td>
</tr>
<tr>
<td style="text-align:left;">
neutropenia
</td>
<td style="text-align:left;">
absolute neutrophil count \< 1000 per mm3
</td>
<td style="text-align:left;">
categorical, binary (1 = yes, 0 = no)
</td>
<td style="text-align:left;">
independent
</td>
</tr>
<tr>
<td style="text-align:left;">
is_deceased
</td>
<td style="text-align:left;">
outcome (1 is death, 0 is survival)
</td>
<td style="text-align:left;">
categorical, binary (1 is death, 0 is survival)
</td>
<td style="text-align:left;">
dependent
</td>
</tr>
</tbody>
</table>

Upon ICU admission, we included baseline patients’ information on
demographic data, diagnosis, extent of organ dysfunction, comorbidity
burden, presence of neutropenia, disease status and number of days in
hospital prior to ICU referral. Based on above-mentioned information,
independent variables were created, and the outcome of ICU
hospitalization was set as a dependent variable (Table 1). This study
was carried out according to the principles of the Declaration of
Helsinki. Approval was granted by the local ethics committee (date:
03.08.2023 / no: 1236). Since we performed a retrospective analysis of
routinely collected de-identified data, informed consents from the
patients were not required. The trial was registered. All statistical
analyses were performed using R version 4.2.1 (R Core Team, 2022).
Сontinuous variables were described as mean (standard deviation), median
(25–75 percentiles) and range. We performed a univariate analysis first
to calculate the odds ratio (OR) of mortality, and statistically
significant factors were then used in a multivariate logistic regression
model to determine outcome prediction. Receiver operating curve (ROC)
was done for the final model. In this research, all the tests were
two-sided, and p \< 0.05 was considered as statistically significant.
