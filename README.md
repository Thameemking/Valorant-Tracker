# Valorant Pro Tracker

A data analytics tool for Valorant players that uses machine learning to provide performance insights.

## Overview

Valorant Pro Tracker analyzes your match data to identify your unique playstyle, track rank progression, and highlight your strengths with different agents. Using K-means clustering, it categorizes players into four playstyles: Aggressive Duelist, Strategic Leader, Support Specialist, or Flex Playmaker.

## Features

- AI-powered playstyle classification
- Interactive rank progression timeline
- Agent performance visualization
- Combat analytics (KDA, headshot %, ADR)
- Custom HTML performance reports

## Setup

```
pip install -q dask[complete] plotly==5.13.0 dask-ml
python tracker.py
```

Enter your Valorant ID when prompted, and a performance report will be generated as an HTML file.

## Technical Details

The tracker processes 200 matches of performance data, applies feature engineering to create advanced metrics, and uses machine learning to identify patterns in your gameplay. Visualizations are created with Plotly and presented in a custom HTML dashboard.
