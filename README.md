# BarLinePlotScatter — Plotly Express Charts

Three small, independent scripts that each read a CSV and open an interactive
[Plotly Express](https://plotly.com/python/plotly-express/) chart in your browser.

## Scripts

| Script | Chart | Reads | Axes / encoding |
| --- | --- | --- | --- |
| `barPlotTable.py` | Bar chart | `data.csv` | x=`Country`, y=`InternetUsers` |
| `plot.py` | Line chart | `line_chart.csv` | x=`Year`, y=`Per capita income`, color=`Country` |
| `scatterPlot.py` | Scatter chart | `data.csv` | x=`Population`, y=`Per capita`, color=`Country`, size=`Percentage` |

The CSV data files (`data.csv`, `line_chart.csv`) are included in the repo.

## Requirements

```
pip install pandas plotly
```

## How to run

Run any of the scripts individually:

```
python barPlotTable.py
python plot.py
python scatterPlot.py
```

## Expected output

Each script calls `fig.show()`, which opens the interactive chart in your default
web browser (or renders inline if run inside a notebook). Nothing is written to
disk. Hover over the chart for tooltips; use the toolbar to zoom, pan, and export
a PNG.
