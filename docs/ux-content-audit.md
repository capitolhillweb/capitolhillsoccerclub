# Capitol Hill Soccer Club — first-pass UX and content audit

Research date: November 10, 2026. Based on publicly accessible pages; some embedded documents, registration systems, and navigation destinations could not be verified. This is a design draft, not an approved content migration.

## Peer-site review

| Club | Observed pattern | Implication |
| --- | --- | --- |
| McGilvra | Immediate season status, registration and coaching notices | Make current-season tasks visible |
| Beacon Hill | Fall program page with dates, fees, and aid tiers | Consolidate registration requirements and financial aid |
| Woodland | FAQ anticipates roster, schedule, and game-day questions | Add a parent FAQ after content confirmation |
| Ballard | Detailed registration dates, pricing, and scholarships | Provide transparent registration information |
| Shorelake | Season overview, boundaries, news, registration | Separate seasonal announcements from evergreen content |
| Rainier Valley | Current-season CTA, schedules, coaches, volunteer roles | Prioritize repeat-visitor shortcuts |
| SC Queen Anne | Programs, get involved, resources, about and registration | Use task-based navigation |
| LVR | Age-based program details and expected game days | Clarify U6–U9 vs U10–U19 pathways |
| Lake City | Minimal registration-led homepage | Ensure basic action is never buried |

Sources:
- https://mcgilvrasoccer.org/
- https://beaconhillsoccerclub.org/programs/fallsoccer
- https://woodlandsoccer.org/
- https://ballardsoccer.org/registration/
- https://shorelake.org/
- https://www.rainiervalleysoccer.org/
- https://qasoccer.org/
- https://www.lvr-soccer.org/
- https://lakecitysoccer.org/

## Current Capitol Hill site

Source: https://capitolhillsoccerclub.org/

### Existing strengths
- Clear recreational mission and SYSA affiliation
- Registration destination through Otto Sport
- Fall practice schedule, MOD games, association games
- Montlake and Garfield field resources
- Coach compliance and training plans
- Jamboree, City Tournament, indoor league and summer notices
- Contact email and mailing address

### UX weaknesses
- Evergreen information, operational resources and time-sensitive announcements appear in one long homepage stream
- No stable parent-oriented information hierarchy
- Coach resources compete with player/parent tasks
- Expired summer announcements remain prominent
- Dates and links have mixed levels of specificity
- Many actions depend on offsite documents or third-party systems

### Proposed navigation
Home / Programs / Schedules & fields / Coaches / Get involved / About, with Register as the primary action.

### Design system decisions
- Blue and green inspired by supplied crest and SYSA 2024 club color reference; not a replacement for formal club brand standards
- DM Sans body and Outfit display, both open-licensed Google Fonts; system font fallbacks
- Semantic HTML, visible keyboard focus, skip link, reduced-motion support, responsive navigation, descriptive link text
- Reusable spacing, type, buttons, cards and semantic color tokens
- Avoid invented fees, dates or claims about scholarships
- Existing club team photography referenced from current Squarespace CDN pending media permissions and asset migration

## Content/link verification before launch
1. **Logo:** supplied PNG is not yet committed as a binary repository asset; the current header uses a provisional symbol. Replace with the actual crest before approval.
2. **Direct links:** some existing links lead to Squarespace documents or pages that could not be resolved in the research environment. Validate and migrate coach training PDFs, game schedules, playfield maps and donation link.
3. **Season dates:** 2026 content is retained as historical/current-site material, not represented as new 2027 announcements.
4. **Registration:** verify Otto Sport landing page and registration availability; do not imply registration is currently open.
5. **Photos:** currently hotlinked from existing club Squarespace; download to the repository with permission before DNS cutover.
6. **CMS:** only the homepage announcement remains in Pages CMS in this first layout draft. Migrate approved section copy and seasonal updates to CMS collections next.
7. **Testing:** verify Astro build, keyboard/mobile menu, contrast, responsive breakpoints and link destinations locally before merging.
8. **No DNS/deployment changes** are included in this branch.
