# LaTeX Project Rules and Guidelines

Please follow these rules and guidelines when modifying the LaTeX codebase for the Internship Report.

## 1. Syntax & Compilation Safety
- **Escape Special Characters**: Always escape LaTeX special characters such as `_`, `&`, `%`, `$`, `#`, `{`, and `}` unless they are part of command names (e.g. use `\_` for underscores in text, `\&` for ampersands, etc.).
- **Closing Environments**: Always ensure that every `\begin{environment}` has a corresponding `\end{environment}`.
- **Braces Matching**: Ensure that all curly braces `{}` and square brackets `[]` are matched properly to avoid compilation errors.

## 2. Document Structure & Aesthetics
- **Consistent Structure**: Keep pages separated using `\newpage` or logical breaks.
- **Margins & Borders**: Maintain the defined 1-inch margins and the page border set up in the preamble using `eso-pic` and `tikz`.
- **Spacing**: Use `\vspace` and `\hspace` consistently to match existing layouts. Prefer logical spacing packages where applicable.
- **Font & Styling**: Do not mix hardcoded fonts/styles arbitrarily. Use document-wide styles or clean definitions in the preamble.
- **Clear Headings**: Use `\chapter`, `\section`, and `\subsection` in a clean hierarchy.

## 3. Lists, Tables, and Figures
- **Table Formatting**: Use proper alignment descriptors (e.g. `l`, `c`, `r`, `p{width}`) and standard borders. Ensure tables do not overflow margins.
- **Caption & Labels**: Every table or figure must have a `\caption` and a `\label` for cross-referencing if they are placed inside float environments.
- **Image Paths**: Keep figures in the `./images/` directory.

## 4. Coding & Cleanliness Rules
- **Formatting**: Keep the code readable. Use consistent indentation (2 or 4 spaces).
- **Comments**: Keep LaTeX comments (`%`) informative and clean. Do not delete existing comments unless they are outdated or requested to be removed.
- **No Placeholders**: Write the actual text and contents instead of leaving placeholders (like `todo` or empty lines) unless explicitly asked to do so.
- **Minimal Preambles**: Keep package imports grouped and documented in the preamble. Do not load duplicate packages.