###  Improve Serial Number Rendering Logic
### DATE
- 13/01/2026
This update refactors the item serial number rendering logic to improve
readability, print/PDF stability, and data normalization.

#### Key Changes
- Refactored serial number handling to normalize separators (`,` and new lines)
- Converted serial rendering from `<br>`-based layout to row-based chunk rendering
- Added safe chunk size to prevent page-break issues in PDF/print
- Improved table structure by introducing `<tbody>`
- Added CSS to visually group serial rows into a single logical block
- Removed debug-only conditional logic (`if False`)

#### Benefits
- Prevents serial numbers from being cut across pages
- Improves readability for long serial lists
- Produces cleaner and more professional PDF/print output
- Easier to maintain and extend in the future
