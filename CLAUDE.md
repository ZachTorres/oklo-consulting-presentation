# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an Oklo Technical Services business presentation project for a Business 4900 Data Story assignment. The repository contains:

1. **Web presentation** (`oklo_presentation.html`) - Interactive reveal.js presentation with animations and charts
2. **PowerPoint presentation** (`Oklo_Professional_Presentation.pptx`) - 15-slide deck with Oklo branding
3. **Speaker notes** (`Oklo_Speaker_Notes_10_Minute_Script.docx`) - Timed 10-minute presentation script
4. **Slidedoc** (`Oklo_SLIDEDOC_Final.md`) - Written version for standalone reading

**Data POV (Core Argument):**
"With over 80 new nuclear startups entering the microreactor market, Oklo can transform from a pre-revenue reactor builder into the ecosystem's technical backbone — offering simulation, safety, and regulatory consulting to accelerate others' reactor licensing and earn immediate, scalable revenue."

## Key Files and Their Purposes

### Presentation Files
- `oklo_presentation.html` - Main reveal.js HTML presentation (interactive, web-based)
- `Oklo_Professional_Presentation.pptx` - PowerPoint version with Oklo branding
- `oklo-logo.png` - Oklo brand logo used in presentations

### Documentation
- `Oklo_SLIDEDOC_Final.md` - Comprehensive written version (~16KB, full details)
- `Oklo_Speaker_Notes_10_Minute_Script.docx` - Word-for-word script with timing
- `COMPLETE_GUIDE_FROM_SCRATCH.md` - Comprehensive tutorial for students
- `README.md` - Project overview and live demo link

### Python Generation Scripts
- `create_professional_presentation.py` - Main script to generate PowerPoint from scratch
- `create_speaker_notes_doc.py` - Generates speaker notes Word document
- `analyze_pptx.py` - Analyzes PowerPoint structure
- `modify_presentation.py` - Modifies existing presentations
- `add_all_visuals.py` - Adds visual elements to slides

## Presentation Architecture

### Reveal.js Presentation Structure
The HTML presentation uses:
- **Reveal.js 5.0.4** - Core presentation framework
- **Chart.js 4.4.1** - For data visualizations
- **Custom CSS** - Oklo branding (teal #48C9B0, navy #003366, black background)

15 slides covering:
1. Title slide
2. Data POV statement
3. Executive summary (3 stat boxes)
4. Problem identification (bar chart)
5. Why Oklo (4 advantage boxes)
6. Service lines (3 columns)
7. Financial projections (stacked area chart)
8. Market analysis (funnel)
9. Implementation timeline (4 phases)
10. Strategic benefits (hub & spoke)
11. Risk matrix (2x2)
12. Recommendations
13. Conclusion
14. Q&A
15. Sources

### PowerPoint Generation
The `create_professional_presentation.py` script uses `python-pptx` library to:
- Create 15 slides programmatically
- Apply Oklo brand colors (navy #003366, green #00A651)
- Generate 2 data charts (bar chart on slide 4, stacked area chart on slide 7)
- Add visual diagrams (boxes, circles, timelines, matrix)
- Ensure consistent formatting and spacing

**Color Scheme:**
```python
OKLO_NAVY = RGBColor(0, 51, 102)
OKLO_GREEN = RGBColor(0, 166, 81)
OKLO_LIGHT_BLUE = RGBColor(240, 248, 255)
OKLO_DARK_GRAY = RGBColor(51, 51, 51)
OKLO_ORANGE = RGBColor(255, 102, 0)
```

## Common Development Tasks

### Modifying the PowerPoint Presentation

To regenerate the PowerPoint from scratch:
```bash
python create_professional_presentation.py
```

Output: `Oklo_Professional_Presentation.pptx` (60KB, 15 slides)

### Modifying the Reveal.js Presentation

Edit `oklo_presentation.html` directly. Key sections:
- **Styles**: Lines 17-500+ (CSS for branding, layouts, animations)
- **Slides**: Inside `<div class="slides">` (each `<section>` is a slide)
- **Charts**: JavaScript at bottom using Chart.js

### Regenerating Speaker Notes

```bash
python create_speaker_notes_doc.py
```

Output: `Oklo_Speaker_Notes_10_Minute_Script.docx`

### Testing Presentations

**Reveal.js (HTML):**
- Open `oklo_presentation.html` in browser
- Press `S` for speaker notes
- Press `ESC` for slide overview
- Press `F11` for fullscreen

**PowerPoint:**
- Open in Microsoft PowerPoint
- Use Presenter View for notes

## Data and Content Structure

### Market Data
- 80+ SMR designs in development
- 90+ advanced reactor technologies globally
- 600+ nuclear startups/scaleups analyzed
- Top funded: TerraPower ($1.4B), X-energy ($1B), Kairos ($629M), Newcleo ($677M)

### Financial Projections
Year-by-year revenue targets:
- 2026: $2.6-4.5M (8-15 clients)
- 2027: $11.9-18M (20-30 clients)
- 2028: $34.5-47.3M (40-55 clients)
- 2029: $70-104M (65-95 clients)
- 2030: $115-165M (95-130 clients)

### Service Lines
1. **Licensing & Regulatory**: $50-80M/yr target
2. **Safety & Simulation**: $30-50M/yr target
3. **Fuel Cycle Management**: $15-25M/yr target

## Deployment and Sharing

### GitHub Pages Deployment
The presentation is live at: https://zachtorres.github.io/oklo-consulting-presentation/oklo_presentation.html

To update:
1. Edit `oklo_presentation.html`
2. Commit to main branch
3. GitHub Pages auto-deploys in 1-2 minutes

### Alternative Deployment (Netlify Drop)
- Go to https://app.netlify.com/drop
- Drag `oklo_presentation.html` and `oklo-logo.png`
- Get instant URL

See `CONVERSION_GUIDE.md` for other sharing options (PDF, PowerPoint, Google Slides).

## Important Constraints

### Oklo Branding Requirements
- Primary accent: Teal (#48C9B0) for reveal.js, Green (#00A651) for PowerPoint
- Background: Pure black for reveal.js, Navy for PowerPoint title slides
- Typography: Segoe UI family, bold headings
- Logo: Always include `oklo-logo.png` in top-right corner

### Presentation Timing
- Total duration: 10 minutes
- 15 slides = ~40 seconds per slide average
- Key slides (data POV, financials, conclusion) get more time
- Q&A: Additional 5 minutes after presentation

### Academic Context
- Course: Business 4900
- Project: Data Story Project
- Due: October 28, 2025
- Requirements: Slide deck + Slidedoc + 3-page reflection paper
- AI usage: Must be documented in reflection paper

## Python Script Architecture

All Python scripts use `python-pptx` library for PowerPoint generation:

**Core pattern:**
```python
from pptx import Presentation
from pptx.util import Inches, Pt
from pptx.enum.text import PP_ALIGN
from pptx.dml.color import RGBColor

prs = Presentation()
prs.slide_width = Inches(10)
prs.slide_height = Inches(7.5)

# Add slides with layouts
slide = prs.slides.add_slide(prs.slide_layouts[6])  # Blank layout

# Save
prs.save('output.pptx')
```

**Chart generation:**
```python
from pptx.chart.data import CategoryChartData
from pptx.enum.chart import XL_CHART_TYPE

chart_data = CategoryChartData()
chart_data.categories = ['2026', '2027', '2028']
chart_data.add_series('Revenue', (10, 20, 40))

chart_shape = slide.shapes.add_chart(
    XL_CHART_TYPE.AREA_STACKED, x, y, cx, cy, chart_data
)
```

## Content Sources

All data sourced from publicly available information:
- StartUs Insights (2025) - Nuclear startups data
- NRC filings - Oklo regulatory history
- TechCrunch, CNBC - Funding data
- Utility Dive - NuScale approval timeline
- Oklo Inc. website - Company information

See slide 15 (Sources) and `Oklo_SLIDEDOC_Final.md` for complete bibliography.

## Working Directory Structure

```
oklo-consulting-presentation-main/
├── oklo_presentation.html          # Main reveal.js presentation
├── oklo-logo.png                   # Brand logo
├── Oklo_Professional_Presentation.pptx  # PowerPoint version
├── Oklo_Speaker_Notes_10_Minute_Script.docx
├── Oklo_SLIDEDOC_Final.md         # Written version
├── create_professional_presentation.py  # Main generator
├── create_speaker_notes_doc.py
├── analyze_pptx.py
├── README.md
├── COMPLETE_GUIDE_FROM_SCRATCH.md
├── CONVERSION_GUIDE.md
└── [various other documentation files]
```

## Editing Guidelines

### When modifying slides:
1. **Maintain consistency**: All 15 slides should follow same color scheme
2. **Preserve data**: Financial projections and market data are research-backed
3. **Keep branding**: Oklo logo and colors must remain
4. **Timing awareness**: Each slide ~40 seconds when presenting

### When adding new features:
1. Test in both reveal.js and PowerPoint versions
2. Ensure animations work in modern browsers (Chrome, Firefox)
3. Verify charts render correctly
4. Update speaker notes if content changes

### When fixing issues:
1. Check both HTML and PPTX versions
2. Verify file paths for images (relative paths)
3. Test deployment on GitHub Pages
4. Confirm compatibility with PowerPoint 2007+
