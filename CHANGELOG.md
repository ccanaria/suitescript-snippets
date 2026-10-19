# Change Log

All notable changes to the "SuiteScript Snippets" extension will be documented in this file.

## [1.1.1] - 2026-10-18

### Added
- Extension icon and Marketplace gallery banner
- Marketplace metadata in `package.json` (`homepage`, `bugs`, `pricing`)

### Changed
- Corrected the advertised snippet count to 50 (32 for SuiteScript 1.0, 18 for SuiteScript 2.1)
- Updated README with the actual Marketplace display name, contact email, and repository links
- Aligned `RELEASE.md` licensing section with the Custom Source-Available License in `LICENSE`
- Excluded `RELEASE.md` and `.github/` from the packaged extension

## [1.1.0] - 2026-01-22

### Added
- Complete SuiteScript 1.0 support with 30+ new snippets
- All major SuiteScript 1.0 script types (RESTlet, Suitelet, User Event, Scheduled, Client, etc.)
- SuiteScript 1.0 User Event individual entry point snippets (beforeLoad, beforeSubmit, afterSubmit)
- Comprehensive SuiteScript 1.0 helper snippets:
  - Search with pagination and simple search
  - Record operations (load, create, transform)
  - Field operations (get/set field values, line items)
  - HTTP requests using nlapiRequestURL
  - Script scheduling and field utilities
  - Logging and error handling
  - Context, user, and role information
  - Client-side dialogs (alert, confirm)
- All SuiteScript 1.0 snippets use `ss10-` prefix for easy identification
- Traditional function syntax for legacy compatibility

### Changed
- Extension name updated to reflect dual version support
- Package name changed from `canariawerx-suitescript-2-1-snippets` to `canariawerx-suitescript-snippets`
- Updated documentation to clearly separate SuiteScript 1.0 and 2.1 snippets

## [1.0.0] - 2026-01-22

### Added
- Initial release
- Complete snippets for all SuiteScript 2.1 script types
- RESTlet with full CRUD operations
- Suitelet with GET/POST handling
- User Event Script with all three entry points
- Map/Reduce Script with all four phases
- Scheduled Script template
- Client Script with all event handlers
- Portlet Script template
- Mass Update Script template
- Workflow Action Script template
- Bundle Installation Script template
- Reusable module template
- Helper snippets for common operations (search, record operations, HTTP requests)
- ECMA 6 syntax throughout
- No N/log module dependencies
- JSDoc annotations for IntelliSense
- @author tag for code attribution
