# Edmonton Transit Access

This project turns the Edmonton Transit Service (ETS) GTFS schedule feed and OpenStreetMap into precomputed accessibility results, and visualized by neighbourhood in a Streamlit application.

## Motivation

Which Edmonton neighbourhoods have the worst transit access relative to their population, and how does that change with time and day?

## Quick Start

```bash
python -m venv .venv && source .venv/bin/activate
pip install -e ".[dev]"
pytest
```

## Project Structure

```bash
pipeline/         download, validate and build processed data
data/raw/         downloaded inputs
data/processed/   small outputs the app reads
app/              Streamlit app
tests/            pytest tests
```

## Usage

## AI Assistance

This project was built with help from Claude Code (Claude Opus 5.5) for drafting system architecture, writing tests, debugging, and auditing code quality. Commits that include AI-written code carry a `Co-Authored-By: Claude` trailer.

## Data & Licenses

The code is released under the [MIT License](LICENSE), which does not cover the data found in `data/`, that are derived from the sources below and remain under their original licenses.

- Contains information licensed under the
  [City of Edmonton Open Data Terms of Use](https://data.edmonton.ca/stories/s/City-of-Edmonton-Open-Data-Terms-of-Use/msh8-if28/).
- Map data © [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors (ODbL).

## Contributing
