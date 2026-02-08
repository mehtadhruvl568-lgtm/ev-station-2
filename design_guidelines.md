# EV Charging Station Planning Platform Design Guidelines

## Design Approach
**Selected Approach:** Reference-Based (Productivity/Data Visualization)
Drawing inspiration from **Linear** for clean data interfaces and **Notion** for organized information hierarchy, combined with mapping platform patterns from industry leaders.

**Key Design Principles:**
- Data-first clarity for traffic analysis
- Professional dashboard aesthetic for B2B users
- Map-centric layout with supporting data panels
- Minimal cognitive load for complex datasets

## Core Design Elements

### A. Color Palette
**Primary Colors:**
- Deep Blue: 215 85% 25% (primary brand, trust, technology)
- Electric Blue: 200 95% 55% (EV theme, interactive elements)

**Supporting Colors:**
- Neutral Gray: 220 15% 95% (backgrounds, cards)
- Success Green: 145 75% 45% (recommended stations)
- Warning Orange: 35 90% 60% (medium priority areas)
- Subtle Purple: 260 25% 65% (accent, data visualization)

**Dark Mode:**
- Background: 220 15% 8%
- Cards: 220 10% 12%
- Text Primary: 220 15% 95%

### B. Typography
**Primary Font:** Inter (Google Fonts)
- Headers: 600 weight, sizes 32px, 24px, 20px
- Body: 400 weight, 16px base
- Data/Labels: 500 weight, 14px

**Monospace:** JetBrains Mono for data values and coordinates

### C. Layout System
**Tailwind Spacing Units:** Consistent use of 4, 6, 8, 12, 16
- Component padding: p-6, p-8
- Section margins: mb-8, mt-12
- Element spacing: gap-4, space-y-6

### D. Component Library

**Navigation:**
- Top navigation bar with logo, main sections, user profile
- Breadcrumb navigation for deep data views
- Floating action button for "Add Data Source"

**Data Display:**
- Map container taking 70% of viewport width
- Side panel (30% width) for controls and analysis
- Metric cards with large numbers and trend indicators
- Data tables with sorting and filtering
- Progress bars for charging station priority scores

**Forms & Controls:**
- Map layer toggles (traffic density, EV adoption, existing stations)
- Date range selectors for historical data
- Search/filter controls for road segments
- Upload interface for traffic data files

**Interactive Elements:**
- Map markers with hover tooltips showing detailed metrics
- Clickable road segments highlighting traffic data
- Expandable panels for detailed station recommendations
- Modal dialogs for adding new data points

**Overlays:**
- Loading states with progress indicators
- Data processing status notifications
- Confirmation dialogs for station recommendations

### E. Layout Specifications

**Dashboard Layout:**
- Header: 64px height with navigation
- Main content: Split view (map 70% | data panel 30%)
- Map controls: Floating overlay on map (top-right)
- Status bar: Bottom 48px for data processing status

**Data Visualization:**
- Heat map overlay for traffic density (red-to-green gradient)
- Pin clusters for existing charging stations (blue icons)
- Recommended locations (green pins with priority numbers)
- Road segment highlighting on hover/selection

### F. Interaction Patterns

**Map Interactions:**
- Click road segments to view detailed traffic data
- Drag to create custom analysis areas
- Zoom controls with data density adaptation
- Pan with lazy-loading for performance

**Data Management:**
- Drag-and-drop file upload for traffic datasets
- Real-time validation of data formats
- Progress tracking for large data processing
- One-click export of recommendations

## Images
No large hero image required. Focus on:
- Clean iconography for map controls (zoom, layers, filter)
- Data visualization charts and graphs within the interface
- Simple loading animations for data processing states
- Minimal branded elements maintaining professional aesthetic

## Key Constraints
- Map must remain primary focus with uncluttered overlay design
- Data density should adapt to zoom levels (no information overload)
- Performance-first approach for large dataset handling
- Accessibility compliance for color-blind users in data visualization