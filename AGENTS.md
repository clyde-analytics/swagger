# Agent Instructions

Do not recreate or update generated `.txt` instance files when changing R scripts.
The project owner will regenerate paste-ready `.txt` outputs manually through
`utils_run.R` using the `prepare_code_for_api(...)` workflow.

## Script Organization

When writing or substantially editing scripts, organize the file into clear numbered sections. Existing well-structured project files may be used as examples, but do not copy poor structure from a messy file just because it exists.

The examples below show the intended style, not required section counts or names. Use only the sections that fit the task.

For R scripts, use section headers such as `# 0. Settings####`, `# 1. Source Dependencies####`, `# 2. Helper Functions####`, `# 3. Main Processing####`, `# 4. Validation / Error Handling####`, and `# 5. Output / Run####`. For longer R scripts, use separator lines when helpful:

```r
#_______________________________________________________________________________
```

For PHP entrypoint/wrapper scripts, keep setup, request method/body validation, authorization, request headers, routing/scoring-engine calls, and response handling separated where applicable.

For other script types, keep the file organized by clear sections with short comments explaining each section's purpose. Prefer practical, readable structure over dense unsectioned code.

## Project Documentation

If a `docs/` folder exists, use it selectively as a routing/context aid before broad repo exploration. Do not read the entire folder by default.

Read the smallest relevant doc when the task is broad, architectural, unfamiliar, ambiguous, or clearly matches a doc filename. Prefer targeted source search when the task points to a specific file, function, error, or small code change.

Treat docs as guidance, not authoritative truth, unless the user says otherwise. Verify current behavior in source code.

Ignore documentation-tool metadata folders such as `.obsidian/`, `.vscode/`, or generated site/build folders unless the task is specifically about documentation tooling.
