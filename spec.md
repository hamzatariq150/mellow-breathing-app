\# Technical Specification: Mellow



\## Tech Stack

\- \*\*Frontend:\*\* Vanilla HTML5, CSS3, JavaScript (ES6). No build steps or frameworks to ensure instant load times and easy deployment.

\- \*\*Hosting:\*\* GitHub Pages / Vercel (Static hosting).



\## UI/UX Design System (Neumorphism)

\- \*\*Background:\*\* `#e0e5ec` (Soft cool gray).

\- \*\*Extruded Elements (Buttons/Cards):\*\* Dual box-shadows combining a dark bottom-right shadow (`rgba(163, 177, 198, 0.6)`) and a light top-left shadow (`rgba(255, 255, 255, 0.8)`).

\- \*\*Inset Elements (Pressed states/Inputs):\*\* Inverted dual box-shadows to create a "pushed in" physical effect.

\- \*\*Typography:\*\* System UI font stack, soft dark gray text (`#4a5568`), no harsh pure blacks.



\## Component Architecture

1\. \*\*Container:\*\* Centered card with extruded neumorphic shadows.

2\. \*\*Breathing Orb:\*\* A central circle that scales up (inhale), holds, and scales down (exhale) using CSS transitions.

3\. \*\*Control Button:\*\* A large, tactile button that switches to an `inset` shadow state when active.

4\. \*\*State Text:\*\* Dynamic text updating to "Inhale", "Hold", "Exhale".



\## State Management

\- Simple JS state machine: `IDLE` -> `INHALE` (4s) -> `HOLD` (4s) -> `EXHALE` (4s) -> loop or `IDLE`.

