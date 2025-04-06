# AI Project Initialization Request: Interactive Design Patterns & SOLID Principles Showcase

**Project Goal:** Create a visually engaging and interactive educational repository demonstrating common Software Design Patterns and the SOLID principles. Each concept will be presented in its **own self-contained HTML file**, incorporating HTML structure, CSS styling, and JavaScript logic/demonstration, mirroring the interactive presentation style seen in repositories like `ozidan13/algorithms`. The focus is on **visual learning and interaction**.

**Target Audience:** Developers (students, juniors, mid-level) seeking an interactive way to learn, review, or understand Design Patterns and SOLID principles through practical, visual examples directly in their browser.

**Core Technologies:**

*   **Languages:** HTML5, CSS3, JavaScript (Use modern ES6+ features, classes, modules where appropriate but keep it understandable).
*   **Presentation:** Focus on clear explanations, well-formatted code snippets (using `<pre><code>`), and interactive elements within each HTML page. Visualizations should involve direct DOM manipulation (updating text, changing styles, adding/removing elements), simple visual representations (e.g., using styled `div`s), or clear logging to an on-page console/output area.
*   **Libraries:** **Strictly Vanilla JS** for the core pattern/principle implementations and interactions. Avoid external frameworks (React, Vue, etc.) to maintain simplicity and self-containment. *Optional Consideration for Later:* A lightweight syntax highlighter like Prism.js could be added, but implement the initial structure without it.
*   **Code Style:** Clean, well-formatted, and commented HTML, CSS, and JavaScript. Use semantic HTML where possible. Ensure consistent styling across pages.

**Desired Repository Structure:**

├── .gitignore
├── LICENSE
├── README.md # Main project overview and navigation
├── assets/ # Optional: For potential shared resources later
│ ├── css/ # (e.g., global_styles.css)
│ └── js/ # (e.g., syntax_highlighter.js)
│
├── solid/ # SOLID Principles Section
│ ├── 01_single_responsibility/
│ │ ├── README.md # Text-only explanation
│ │ └── index.html # Interactive HTML presentation
│ ├── 02_open_closed/
│ │ ├── README.md
│ │ └── index.html
│ ├── 03_liskov_substitution/
│ │ ├── README.md
│ │ └── index.html
│ ├── 04_interface_segregation/
│ │ ├── README.md
│ │ └── index.html
│ └── 05_dependency_inversion/
│ ├── README.md
│ └── index.html
│
└── design_patterns/ # Design Patterns Section
├── creational/
│ ├── factory_method/
│ │ ├── README.md
│ │ └── index.html
│ ├── abstract_factory/
│ │ ├── README.md
│ │ └── index.html
│ ├── builder/
│ │ ├── README.md
│ │ └── index.html
│ ├── prototype/
│ │ ├── README.md
│ │ └── index.html
│ └── singleton/
│ ├── README.md
│ └── index.html
│
├── structural/
│ ├── adapter/
│ │ ├── README.md
│ │ └── index.html
│ ├── bridge/
│ │ ├── README.md
│ │ └── index.html
│ ├── composite/
│ │ ├── README.md
│ │ └── index.html
│ ├── decorator/
│ │ ├── README.md
│ │ └── index.html
│ ├── facade/
│ │ ├── README.md
│ │ └── index.html
│ ├── flyweight/
│ │ ├── README.md
│ │ └── index.html
│ └── proxy/
│ ├── README.md
│ └── index.html
│
└── behavioral/
├── chain_of_responsibility/
│ ├── README.md
│ └── index.html
├── command/
│ ├── README.md
│ └── index.html
├── iterator/
│ ├── README.md
│ └── index.html
├── mediator/
│ ├── README.md
│ └── index.html
├── memento/
│ ├── README.md
│ └── index.html
├── observer/
│ ├── README.md
│ └── index.html
├── state/
│ ├── README.md
│ └── index.html
├── strategy/
│ ├── README.md
│ └── index.html
├── template_method/
│ ├── README.md
│ └── index.html
└── visitor/
├── README.md
└── index.html

**Detailed File Content Requirements:**

1.  **`.gitignore`**:
    *   Generate a standard `.gitignore` for web development (include `node_modules/`, `.env`, common OS files like `.DS_Store`, `Thumbs.db`, build artifacts, etc.).

2.  **`LICENSE`**:
    *   Use the **MIT License**. Create the `LICENSE` file with the standard text, including placeholders for `<YEAR>` and `<COPYRIGHT HOLDER>` or filling them in.

3.  **`README.md` (Root)**:
    *   **Title:** "Interactive Design Patterns and SOLID Principles Showcase"
    *   **Introduction:** Explain the repo's purpose (interactive learning via HTML/CSS/JS demos). Mention it's inspired by visual algorithm repositories.
    *   **How to Use:** Instruct users to clone the repo and open the individual `index.html` files within each pattern/principle folder directly in their web browser.
    *   **Structure Overview:** Briefly explain the `solid/` and `design_patterns/` directory structure.
    *   **SOLID Principles Navigation:** List the 5 principles. Each list item should link *directly* to the corresponding `index.html` file (e.g., `[Single Responsibility Principle](./solid/01_single_responsibility/index.html)`).
    *   **Design Patterns Navigation:** List the patterns, grouped by category (Creational, Structural, Behavioral). Each pattern name should link *directly* to its corresponding `index.html` file (e.g., `[Factory Method](./design_patterns/creational/factory_method/index.html)`).
    *   **(Optional) Contributing:** Link to `CONTRIBUTING.md` if created later.
    *   **License:** State the license (MIT License).

4.  **`<concept_folder>/README.md` (Example: `solid/01_single_responsibility/README.md`)**:
    *   **Purpose:** Serve as a quick, text-only reference readable on GitHub.
    *   **Content:**
        *   Title: Full name of the principle/pattern.
        *   Brief Definition/Intent.
        *   Problem it solves.
        *   Solution/Structure overview.
        *   (For Patterns) Key participants/classes.
        *   (For SOLID) Core idea/rule.
        *   Link: A prominent link to the interactive `index.html` demo within the same folder (e.g., `[View Interactive Demo](./index.html)`).

5.  **`<concept_folder>/index.html` (THE CORE FILE - Example: `design_patterns/singleton/index.html`)**:
    *   **Structure:** A single, self-contained HTML file.
    *   **`<head>`:**
        *   `<title>`: Name of the Principle/Pattern.
        *   `<style>` tag: Contains all necessary CSS for this specific demo. Aim for a clean, readable layout (e.g., using Flexbox or Grid). Style headings, paragraphs, code blocks (`pre`, `code`), buttons, input/output areas consistently. Define a basic, common visual theme to be used across all `index.html` pages (e.g., similar fonts, color palette).
    *   **`<body>`:**
        *   **Header:** `<h1>` with the Principle/Pattern name.
        *   **Explanation Section:** Clear textual description (definition, problem, solution, benefits, drawbacks, use cases). Can reuse content from the sibling `README.md`.
        *   **Code Display Section(s):**
            *   Use `<pre><code class="language-javascript">...</code></pre>` to display relevant JavaScript code snippets (the pattern implementation itself, usage examples, bad vs. good examples for SOLID).
            *   *Initial CSS:* Include basic CSS rules in the `<style>` tag for padding, background color, and font-family (monospace) for `pre` and `code` tags to ensure readability.
        *   **Interactive Demo Section:** This is crucial for Design Patterns.
            *   **Controls:** Use HTML elements like `<button>`, `<input>`, `<select>` to allow user interaction. Label them clearly.
            *   **Visualization/Output Area:** Use `<div>`s, `<textarea>`, or a dedicated log area to display results, state changes, or visual feedback from the JavaScript execution.
            *   *(Example Interaction for Singleton):* A button "Get Instance". An output div. Clicking the button calls the JS Singleton logic and updates the div to show that the same instance ID is returned each time.
            *   *(Example Interaction for Factory):* A dropdown to select product type, a button "Create Product". Output area shows details of the created product.
            *   *(Example Interaction for Observer):* Buttons to change subject state, an area showing observer notifications.
        *   **SOLID Principles `index.html`:** Focus will be more on side-by-side comparison.
            *   Display "Bad Example" code snippet + explanation of violation.
            *   Display "Good Example" code snippet + explanation of adherence.
            *   Interactivity might be minimal, perhaps a button to trigger a hypothetical scenario demonstrating the fragility of the bad example vs. the robustness of the good one.
    *   **`<script>` tag (usually before `</body>` close):**
        *   Contains all necessary **Vanilla JavaScript** for the demo.
        *   Implement the actual design pattern or SOLID example logic (using classes, functions, objects).
        *   Include DOM manipulation logic: Select HTML elements (controls, output areas), add event listeners (e.g., for button clicks), update the DOM to show results/visualizations.
        *   Ensure JS is well-commented, explaining the pattern implementation and the interaction logic.
        *   Use IIFEs or simple scoping mechanisms if needed to avoid polluting the global namespace, but prioritize clarity.

**Initial Implementation Task (Create these first):**

1.  **Generate Structure:** Create the complete directory structure as specified above, including placeholder `assets` folders.
2.  **Generate Base Files:** Create `.gitignore` and `LICENSE` (MIT).
3.  **Generate Root README:** Create the root `README.md` with title, intro, usage, structure overview, and placeholder lists linking to the *future* `index.html` files for all principles/patterns.
4.  **Implement SOLID - Single Responsibility Principle:**
    *   Create `solid/01_single_responsibility/README.md` (text explanation).
    *   Create `solid/01_single_responsibility/index.html`:
        *   Include basic HTML structure, title, heading.
        *   Embed simple CSS for layout and code block styling.
        *   Display JS code snippets for a "Bad Example" (violating SRP) and a "Good Example" (adhering to SRP) within `<pre><code>` tags.
        *   Add clear textual explanations below each code snippet detailing *why* it's bad/good regarding SRP.
        *   No complex JS interaction needed here, focus on clear presentation.
5.  **Implement Design Pattern - Singleton:**
    *   Create `design_patterns/creational/singleton/README.md` (text explanation).
    *   Create `design_patterns/creational/singleton/index.html`:
        *   Include HTML structure, title, heading, explanation section.
        *   Embed CSS for layout, code block, button, and output area styling.
        *   Display the JS Singleton implementation code in `<pre><code>`.
        *   Add an Interactive Demo section:
            *   A `<button id="getInstanceBtn">Get Singleton Instance</button>`.
            *   A `<div id="output">Instance Info: (click button)</div>`.
        *   Embed JavaScript (`<script>` tag):
            *   Implement the Singleton pattern in JS (e.g., using a class or closure).
            *   Add an event listener to `#getInstanceBtn`.
            *   On click, get the singleton instance (which should have some unique property set on first creation, like `instance.id = Math.random()`).
            *   Update the `#output` div's text content to show a message like `Instance ID: [the unique ID] (Got same instance again!)`.
6.  **Create Placeholder READMEs:** For all *other* principle and pattern folders, create just the `README.md` file containing the title and a link to the `./index.html` (which won't exist yet). This sets up the structure for future work.

**Final Instructions for AI:**

*   Ensure all generated HTML files are self-contained and render correctly when opened directly in a modern browser.
*   Prioritize clarity, readability, and simple, effective interactivity/visualization in the generated code and explanations.
*   Adhere strictly to using **Vanilla JavaScript (ES6+)**.
*   Implement the initial SRP and Singleton examples exactly as described in step 4 and 5 of the "Initial Implementation Task".
*   Generate all specified files and the complete directory structure.

Thank you! Please proceed with generating the project based on these instructions.