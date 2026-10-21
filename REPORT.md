# Research Progress Update — 2026-10-21

*Ongoing systematic research. All figures are relative. Past results are not advice.*

---

## Summary

Research cycles 33–39 completed since the last update. The current best configuration remains unchanged from the prior cycle. Structural validation confirmed no modifications to the core system are warranted at this time.

## Key Findings

- **Core structure confirmed stable.** Removing any individual component from the combined system degrades performance in at least one evaluation period. All components contribute positively.
- **Event-day filter validated.** A calendar-based exclusion rule (introduced last cycle) holds in both evaluation windows, reducing peak drawdown by approximately 30% relative to the unfiltered baseline while preserving the efficiency ratio.
- **Sizing variant tested.** A reduced-size variant for one component improves the efficiency ratio and reduces drawdown in both periods. Currently flagged for live-data confirmation; not yet adopted.
- **Calendar sub-filters reviewed.** Month-end and day-of-month slices showed inconsistent results between periods and were rejected. No calendar sub-filtering added.
- **After-event behaviour noted.** Trades following a prior unfavourable outcome exhibit stronger statistical properties than the overall average in both periods. No action taken (sizing changes require additional validation).
- **Equity-based filter tested.** A 20-period equity slope filter improved results in the in-sample period only; out-of-sample improvement not observed. Rejected.
- **Alternative variant (v2.3 ADX relaxation):** A relaxed filter variant adds approximately 15–20% more qualifying setups with improved efficiency in-sample. Requires retest in the primary engine before any adoption decision.

## Audit Chain Results

- **Win branch isolation:** Core component isolation confirmed; no single component fully explains the combined edge.
- **Filter tightness audit:** Current filter settings are at or near optimal; widening any primary filter increases trade count but reduces efficiency.
- **Regime-start test:** No robust regime-entry advantage identified; effect was inconsistent across periods.
- **GDP/Fed correlation test:** Macro calendar alignment tested; no consistent edge attributable to scheduled economic releases (beyond the existing event-day exclusion).
- **Broker comparison:** Data consistency check between two data sources completed. Results directionally consistent; minor discrepancies attributable to data source differences, not strategy behaviour.

## Status

System A (best configuration): research-stage, not deployed.  
Next step: retest of relaxed variant in primary engine; await parallel MT4 validation results.

---

*2026-10-21 · Relative metrics only · Not financial advice*
