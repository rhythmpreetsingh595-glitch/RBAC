# Healthcare Access Control System Design Guidelines

## Design Approach
**System-Based Approach (Design System)**: Given the enterprise healthcare context requiring trust, compliance, and usability, I recommend **Carbon Design System** for its data-heavy, enterprise focus with medical industry precedent.

## Core Design Elements

### A. Color Palette
**Primary Colors:**
- Light Mode: Deep medical blue (210 65% 25%) for trust and professionalism
- Dark Mode: Softer blue-gray (210 35% 85%) for reduced eye strain during long shifts
- Critical alerts: Medical red (0 75% 45%) for emergency access situations
- Success states: Clinical green (145 60% 35%) for approved actions
- Warning states: Amber (35 85% 50%) for elevated risk scenarios

### B. Typography
- **Primary**: IBM Plex Sans (Carbon's system font) via Google Fonts
- **Monospace**: IBM Plex Mono for audit logs and technical data
- **Hierarchy**: Large headers (2xl) for dashboard sections, medium (lg) for data tables, small (sm) for metadata

### C. Layout System
**Tailwind Spacing Primitives**: Focus on 4, 6, 8, and 12 units
- Container padding: p-6 for main content areas
- Component spacing: gap-4 between related elements, gap-8 between sections
- Form elements: mb-4 for field spacing, p-4 for input padding
- Card layouts: p-6 interior, m-4 exterior spacing

### D. Component Library

**Navigation:**
- Sidebar navigation with role-based menu items
- Breadcrumb navigation for complex data hierarchies
- Quick action toolbar for emergency access functions

**Data Display:**
- Data tables with sortable columns for audit logs
- Patient cards with access status indicators
- Risk assessment dashboards with real-time scoring
- Permission matrix views for role management

**Forms & Controls:**
- Multi-step forms for complex permission requests
- Toggle switches for policy activation/deactivation
- Date/time pickers for temporary access windows
- Biometric authentication prompts

**Feedback & Status:**
- Toast notifications for access decisions
- Status badges for user roles and permissions
- Progress indicators for approval workflows
- Alert banners for security incidents

**Security Elements:**
- Device fingerprint displays
- Session timeout warnings
- Access attempt histories
- Compliance status indicators

### E. Accessibility & Dark Mode
Maintain consistent dark mode across all components, especially critical for healthcare environments with 24/7 operations. Ensure form inputs, data tables, and modal dialogs follow the same dark theme patterns for reduced eye strain during night shifts.

## Key Design Principles

1. **Trust Through Transparency**: Clear visual hierarchy showing who has access to what and why
2. **Security-First Interface**: Visual cues for risk levels, device security, and access anomalies
3. **Compliance by Design**: Built-in audit trails and compliance reporting interfaces
4. **Context Awareness**: Visual indicators for location, time-based access, and emergency states
5. **Scalability**: Modular components that work across different hospital sizes and specialties

## Healthcare-Specific Considerations
- High contrast ratios for medical professionals wearing glasses/protective equipment
- Large touch targets for gloved hands and mobile device usage
- Clear emergency access pathways with distinct visual treatment
- Minimal cognitive load during high-stress medical situations