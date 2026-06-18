# Advanced Second Entry

Advanced Second Entry is a TradingView Pine Script v6 indicator from Price Action Tools built for discretionary price-action traders who want clean second-entry structure on the chart.

It highlights alternating legs, reset conditions, and second-entry opportunities with 2EL and 2ES labels. Optional HL/LH confirmation markers and projection visuals help keep the setup readable without turning the chart into noise.

## Features

- Alternating up and down leg tracking
- Reset-on-equal-high/low logic
- Second-entry labeling with `2EL` and `2ES`
- Optional `HL` and `LH` confirmation markers
- Optional projection lines for entry, stop, and target
- Configurable break offset, label spacing, and signal filters
- Clean overlay display designed for live trading and review

## What this Pine version does

- Ported from the NinjaTrader 8 Advanced Second Entry indicator logic
- Built natively for TradingView Pine Script v6
- Keeps the core second-entry workflow and chart readability
- Uses TradingView-friendly visuals and inputs

## Notes on TradingView

- Pine is bar-based, so it does not reproduce NT8 intrabar/tick execution exactly
- NT8 licensing and platform-specific UI were intentionally omitted
- Drawing-object behavior can differ slightly from NT8 on live bars

## Price Action Tools

- Website: https://priceactiontools.com
- Product page: https://priceactiontools.com/product/advanced-second-entry-indicator/

## Usage

1. Add the script to a price chart.
2. Adjust the Behavior and Appearance inputs to match your workflow.
3. Use `Only Show Second Entries` if you want a cleaner chart focused on `2EL` and `2ES`.
4. Turn on `Show HL / LH Markers` if you want additional confirmation context.

## Notes

- This script is intended for discretionary trading workflows.
- For best results, compare the output against representative market sessions and tune offsets as needed.
