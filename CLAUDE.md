# CSE-6040: Computing for Data Analytics

Georgia Tech OMSA course. An introduction to programming techniques relevant to data analysis and machine learning, building a complete data analysis pipeline from scratch: collection, preprocessing, storage, analysis, and visualization.

## Course Focus

Three major modules covering 15 topics:

1. **Module 0 — Fundamentals**: Python basics, dictionaries, probability/calculus/linear algebra review, floating-point arithmetic
2. **Module 1 — Data Representation & Transformation**: String processing and regex, web scraping, Pandas data tidying, visualization (Seaborn, Bokeh), SQL and relational data
3. **Module 2 — Analysis**: NumPy/SciPy, graph algorithms (PageRank), linear/logistic regression, k-means clustering, PCA/SVD

The emphasis is on formalizing high-level analysis questions into mathematical/computational problems, then translating those into working code. Program correctness and efficiency (Big-O) are recurring themes.

## Tech Stack

- **Python** (primary language): NumPy, Pandas, SciPy, Seaborn, Bokeh
- **SQL**: SQLite, relational databases, queries and joins
- **Jupyter Notebooks**: primary development environment
- **Libraries**: regex, BeautifulSoup, json, csv, sqlite3
- **Platform**: Vocareum (autograded lab notebook submissions)

## Workflow: Code First, Then Study

The default workflow is **machine writes, human understands**:

1. **`/complete` — Claude writes full working code** with inline comments explaining key decisions.
2. **Add to the study guide website** at `flashcards/index.html`. For each completed assignment, add:
   - **Study Guide section**: A new topic card with key concepts, decision rationale, formulas (using KaTeX `\( \)` delimiters), and "when to use" guidance.
   - **Flashcards**: New cards tagged to the assignment, each with a front (question/concept), back (answer/explanation), ELI5 description, and key points. Include a mix of:
     - Concept cards ("What is..." / "When would you use...")
     - Decision cards ("Why did we choose X over Y?")
     - "What if" cards ("What would happen if we changed...")
   - **Quiz questions**: 1–2 exam-style multiple-choice questions that test conceptual understanding and code reasoning.
   - Format all additions to match the existing HTML structure, styling, and JavaScript patterns in the file.
3. After completing the code and study materials, use `/quiz` or the built-in quiz tab to test understanding interactively.

### Other modes still available
- **`/homework` — Socratic mode.** Guide through questions and hints, no complete solutions.
- **`/quiz` — Quiz mode.** Test knowledge on specific topics.
- **`/concept`, `/explain-code`, `/optimize`** — Socratic deep-dives on specific areas.

## Homework Context

- All homework is done in **Jupyter Notebooks** running on a remote platform (Vocareum). When the user pastes a code block or exercise, assume it comes from a notebook cell.
- Any undefined variables, imports, references to databases, data files, or other resources in pasted code were defined in earlier cells or exist on the remote notebook environment. **Do not search for them locally, do not flag them as missing, and do not ask the user to provide them.** Infer their types/values from context and write code accordingly.
- The local repo does not contain the notebooks, datasets, or databases — only the user's study materials. All homework execution happens remotely.

## Guidelines for Claude

- When writing Python, follow PEP 8 style and use idiomatic Python (list comprehensions, generators, etc.).
- Connect code back to the data analysis pipeline: collection, preprocessing, storage, analysis, visualization.
- For numerical methods (linear algebra, optimization), explain the math alongside the code.
- When helping with SQL, explain query logic step-by-step.
- Emphasize correctness and efficiency — Big-O reasoning, testing edge cases.
- Help develop intuition for algorithm choices (why this data structure, why this approach).
- Remind about reproducibility: documenting choices, explaining reasoning.
