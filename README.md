# Human Digital Baseline v0.6

Adds an optional sleep-cognition analysis visible only inside Sleep History.

Design principle:
- Cognitive measurements remain independent of sleep.
- Sleep never changes cognitive scores or their interpretation.
- Cognitive sessions are stored longitudinally in a separate local dataset.
- The Sleep interface pairs same-day cognitive sessions with the sleep entry for that morning.
- Sleep duration is expressed as deviation from the person's rolling sleep baseline.
- Exploratory within-person Pearson correlations are displayed for reaction time, RT variability, tapping, Go/No-Go accuracy, Go RT and working memory.
- Requires repeated paired observations; early estimates are explicitly labelled exploratory.
- Correlation is not interpreted as causation or diagnosis.

All data remain local to the browser in this prototype.
