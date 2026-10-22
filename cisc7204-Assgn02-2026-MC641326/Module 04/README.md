# Module 04 - Creating Dashboards with Plotly and Dash

## Labs

- **Lab01** - Plotly basics: scatter, line, bar, bubble, histogram, pie, sunburst
- **Lab02** - Dash basics: HTML and core components
- **Lab03** - Adding interactivity: user input and callbacks
- **Lab04** - Flight delay time statistics dashboard

## What this module covers

Moving from static figures to interactive, browser-based dashboards. Plotly produces
charts with hover tooltips, zoom and pan; Dash adds a web application layer on top, where
the layout is built from HTML and core components and interactivity is driven by callback
functions that take user input and return updated figures.

## Key techniques

- `plotly.graph_objects` and `plotly.express` for interactive charts
- `dash.Dash`, `dcc.Graph`, `dcc.Dropdown`, `dcc.Slider`, `html.Div`
- `@app.callback` with `Input` and `Output`
- Running the app inside the Theia IDE and viewing it in the browser

## Files

| File | Lab |
|---|---|
| `CISC7204 Assgn02 Module 04 - Lab01 MC641326 QU YING.ipynb` | Lab01 |
| `CISC7204 Assgn02 Module 04 - Lab02 MC641326 QU YING.zip` | Lab02 |
| `CISC7204 Assgn02 Module 04 - Lab03 MC641326 QU YING.zip` | Lab03 |
| `CISC7204 Assgn02 Module 04 - Lab04 MC641326 QU YING.zip` | Lab04 |

Lab02, Lab03 and Lab04 are zipped Theia project spaces. Unzip and run the application
entry point (typically `python app.py` or `python application.py`) after installing
`dash` and `plotly`; the app is then served at `http://127.0.0.1:8050`.

Evidence of the work, with screenshots of the code and executed output, is posted in
the CISC7204 Personal Forum of Module 04 in Assignment 02.
