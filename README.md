# Human Digital Baseline v3.1

Adds a second, separate **Adaptive Go/No-Go** task while preserving the original fixed Go/No-Go as the longitudinal reference.

## Adaptive task
- 24 trials
- approximately 75% GO / 25% NOGO generated trial-by-trial
- begins at 1400 ms pacing and 850 ms response/stimulus window
- after 3 consecutive correct trials: pace shortens by 100 ms and response window by 50 ms
- after an error: pace lengthens by 180 ms and response window by 90 ms
- bounds: pacing 500–1800 ms; response window 300–1000 ms
- random ±15% inter-trial timing jitter
- stores trial-level difficulty, accuracy and reaction time
- session endpoints include accuracy, median GO RT, final pacing and minimum pacing reached

The fixed Go/No-Go is unchanged and remains analytically separate. The adaptive endpoint is experimental and is not a clinical measure.

Adaptive metrics are added to the Personal Baseline Engine, Metric Explorer, Sleep ↔ Cognition and Neuro Function ↔ Cognition analyses.
