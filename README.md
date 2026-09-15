# Human Digital Baseline v3.0 — Personal Baseline Engine

Major upgrade focused on longitudinal scientific quality rather than adding more unrelated data.

## Personal Baseline Engine
- Robust personal baseline using median/MAD, with SD fallback when MAD is zero.
- Baseline excludes the two most recent observations to reduce circularity.
- Prototype persistent-change signal requires at least 5 prior baseline measurements plus 2 recent measurements.
- A persistent signal is shown only when the last two measurements are on the same side of the prior personal baseline and each is >=1.5 robust SD from it.
- Descriptive slope is calculated per calendar day over up to the latest 8 observations.
- No clinical cutoff, diagnosis or disease probability is produced.

## Metric Explorer
Longitudinal charts and robust statistics for:
- cognitive metrics
- sleep structure and HDB-SQI
- individual neuro-function reports
- vitals
- physical-performance metrics
- all entered blood analytes
- context/confounder variables

Charts show the personal median and interquartile baseline band when enough data exist.

## Multidomain view
The Dashboard detects persistent deviations across domains while keeping:
- objective measurements
- self/caregiver reports
- context/confounders
analytically distinct.

## Data quality
- cognitive sessions store device/browser/screen signature, time band, false starts and protocol metadata
- blood data retain laboratory/method metadata
- vitals and physical-performance forms include protocol/device/setup notes
- Dashboard flags method/device changes that can reduce longitudinal comparability

## Profile & accessibility
- participant ID
- optional birth year / sex at birth / usual height
- preferred device and testing-period metadata
- standardized cognitive-protocol note
- Senior / accessibility mode with larger interface controls
- caregiver reporting remains available in Neuro Function Log

## Backup & privacy
- complete local JSON backup
- optional AES-GCM encrypted backup using a passphrase (PBKDF2-derived key)
- restore backup
- delete all local HDB data
- data remain browser-local in this prototype

## Correlation upgrades
- cognition is aggregated to one observation per day before cross-domain correlation
- Sleep ↔ Cognition and Neuro Function ↔ Cognition include exploratory Pearson r and Fisher-transform 95% confidence intervals
- results are explicitly labeled unstable with fewer than 14 paired days
- association is never presented as causation or diagnosis

## Date handling
Daily logs now use the local calendar date rather than UTC date, improving same-day pairing.

This remains a research prototype, not a medical device or diagnostic system.
