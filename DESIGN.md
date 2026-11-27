# PayTrack — Design Direction

## Audience and purpose
**Audience:** The BSIT finals evaluator and people reviewing a payroll-management interface.

**Primary job:** Present employee records and payroll status in a clear register, with the required login → dashboard → logout flow.

**Headline claim:** “PayTrack starts with an empty employee register.” The interface also makes clear that no pay period is configured and no payroll figures are calculated. It is a classroom prototype, not payroll processing software.

## Visual identity
**Brand color:** Forest green #174A3A, retained from the existing PayTrack identity and used for navigation and primary actions.

**Neutrals:** Page #F3F6F4; surface #FFFFFF; main text #1D2D26; secondary text #52645B; borders #D7E1DA. Text combinations are checked for WCAG AA normal-text contrast (4.5:1). Input borders and keyboard focus indicators use stronger contrast; focus colors differ between light surfaces and the green navigation panels.

## Typography
Tahoma with Arial, sans-serif fallbacks. One familiar sans-serif family keeps the interface readable and the CSS straightforward. Monetary values use tabular numerals when added later.

## Layout and spacing
Spacing scale: 4, 8, 12, 16, 24, 32, 48px, with larger page spacing fluidly adjusted for screen width. Radius scale: 0px for ledger and data surfaces; 4px for form controls and navigation links. Desktop uses a fixed navigation rail and a wide record area; mobile moves navigation above the content. The employee register receives more space than secondary status information.

## Icons
No decorative icons or emoji. Navigation and actions use visible text labels.

## Motion and interaction
No entrance animation, parallax, or decorative motion. Hover and visible keyboard-focus states are provided. Reduced-motion preferences are respected.

## Content rules
Keep the login → dashboard → logout flow. Do not invent employee identities, salary amounts, payroll dates, deduction rates, company details, testimonials, or performance claims. Show honest empty states. The login form only checks that both fields are filled; it does not authenticate accounts. The prototype does not save records, calculate pay, or protect real employee information.
