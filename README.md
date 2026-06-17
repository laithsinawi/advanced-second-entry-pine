# Advanced Second Entry Pine Port

This workspace contains a native TradingView Pine Script v5 port of the NinjaTrader 8 `AdvancedSecondEntry` indicator:

- Source of truth: `/Users/laithsinawi/Projects/NT8/Indicators/AdvancedSecondEntry/AdvancedSecondEntry.cs`
- Pine script: [`pine/AdvancedSecondEntry.pine`](/Users/laithsinawi/Projects/TradingView/AdvancedSecondEntryPine/pine/AdvancedSecondEntry.pine)

## What was ported

- Alternating up/down leg tracking.
- Reset detection for long and short counts.
- Second-entry staging and 2EL / 2ES labeling.
- Optional HL / LH confirmation markers.
- Optional projection lines for entry, stop, and target.
- User inputs for the main behavior and styling controls.
- Text-only signal labels by default, with an option to hide stage-1 labels and show only 2EL / 2ES.

## What is different from NT8

- TradingView Pine is bar-based here, so the NT8 intrabar/tick execution model is not reproduced exactly.
- NT8-specific licensing, purchase UI, and add-on integration were intentionally omitted.
- Pine cannot mirror NT8 drawing-object lifecycles perfectly, so some live-bar reposition behavior may differ.
- The “Strict Signal Bars” filter is preserved conceptually, but live-bar timing can still differ slightly from NT8 because Pine does not expose the same tick-by-tick event stream.
- TradingView's script author shown in the Indicators dialog comes from the publishing account, not from Pine source comments.

## Notes

- The script is overlayed on price bars.
- The code prefers readability and modularity over forcing a brittle one-to-one translation of NT8 implementation details.
- If labels look stale after updating the script, remove the old indicator from the chart and add the updated version again.
- If you want a tighter visual match, the next step is usually to compare this port against a few representative charts and tune the offset and marker settings.
