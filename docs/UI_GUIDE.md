# UI Guide — Make the report look unique and self-made

Goal: apply a cohesive modern design, tweak layout and controls, and add original visual elements so the report looks original.

1) Import theme
- In Power BI Desktop: View > Themes > Browse for themes > import theme/powerbi-theme.json

2) Title & Header
- Replace the existing title with a simple two-line header:
  - Small subtitle (left): "Blinkit — Sales & Inventory"
  - Large title (center): "Operational Performance Dashboard"
- Use Inter or Montserrat (install font and set in Theme JSON). Use bold for title.

3) Top KPI strip
- Create 4 compact KPI cards (Total Sales, Avg Order Value, #Items, Avg Rating)
- Use Card or KPI visual. Add small descriptive secondary text.
- Use a subtle background rectangle with corner radius to group these KPIs.

4) Color & Accent
- Use the theme dataColors for charts (avoid default rainbow). Keep 2–3 core accent colors:
  - Primary: #0F4C5C (deep teal)
  - Accent: #FFD166 (sun)
  - Secondary: #118AB2 (blue)
- Use these consistently (bar fills, line colors, KPI icons).

5) Visual replacements
- Replace default stacked bar with 100% stacked or small multiples where appropriate.
- Replace table visuals with a Card + small table combo for better scanability.
- Use Chiclet Slicer or Synoptic Panel for store tier/region filters (install from AppSource).

6) Navigation & Layout
- Add a left-side slim navigation pane with small icons (Home, Sales, Inventory, Customers, About).
- Each nav item is a bookmark button toggling between pages.
- Create one “About” page that includes a short project summary, authorship, license, and a screenshot.

7) Tooltips and Drillthrough
- Add a compact tooltip page for product-level insights (mini line + KPIs) and enable it for product visuals.
- Implement a drillthrough page for Outlet details.

8) Fonts & Icons
- Use Inter or Montserrat for headings and Roboto for body.
- Add icon images for KPI cards (flatten them and ensure they are consistent color).
- Use subtle shadows under KPI cards (rectangle with soft shadow image or shape to simulate depth).

9) Visual polish
- Use whitespace: increase spacing, use separators (thin line) between sections.
- Replace default color legends with in-visual labels where possible.
- Add animation: use Play Axis (where helpful) for establishment growth trend.

10) Re-export
- After changes, export a new dashboard image (File > Export to PNG) and replace Blinkit-Dashboard.png.
- Export a PDF with the updated title page.

11) Export queries and model metadata
- Use External Tools (Tabular Editor or Power BI Helper) to export:
  - Power Query M queries into queries/ (one .m or .txt file per query)
  - DAX measures list into docs/dax_measures.md
  - Model metadata into docs/model_metadata.json

12) Version & Plagiarism
- Run the plagiarism/text similarity checks over extracted text/queries and document findings in docs/PLAGIARISM_REPORT_TEMPLATE.md

Short design tips to ensure originality
- Re-name calculated measures and cards with your own naming conventions.
- Reword titles & insights, add an “Insights” textbox describing what you changed/analyzed.
- Create original visual compositions (e.g., KPI strip + map + small multiples) rather than copying the original layout exactly.