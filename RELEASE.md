# Release v1.1.0 - SuiteScript 1.0 Support

**Date:** January 22, 2026  
**Author:** Clemen Canaria  
**Organization:** CanariaWerx

## 📦 Installation

Download the VSIX file below and install it in VS Code:

1. Download `canariawerx-suitescript-snippets-1.1.0.vsix`
2. Open VS Code
3. Go to Extensions (`Ctrl+Shift+X` or `Cmd+Shift+X`)
4. Click the "..." menu → **Install from VSIX...**
5. Select the downloaded file

## ✨ Features

A comprehensive collection of VS Code snippets for NetSuite SuiteScript development, now supporting both SuiteScript 1.0 and 2.1!

## 🆕 What's New in v1.1.0

- ✨ **Complete SuiteScript 1.0 Support** - 30+ new snippets for legacy script development
- ✨ **All Major Script Types** - RESTlet, Suitelet, User Event, Scheduled, Client, and more
- ✨ **Comprehensive Helpers** - Search, record operations, field operations, HTTP requests
- ✨ **Easy Identification** - All SuiteScript 1.0 snippets use `ss10-` prefix
- ✨ **Backward Compatible** - All existing SuiteScript 2.1 (`ss21-`) snippets remain unchanged

### SuiteScript 2.1 Script Types (ECMA 6 Syntax)

- **RESTlet** (`ss21-restlet`) - Complete RESTlet with GET, POST, PUT, DELETE handlers
- **Suitelet** (`ss21-suitelet`) - Suitelet with GET and POST request handling
- **User Event** (`ss21-userevent`) - User Event Script with beforeLoad, beforeSubmit, afterSubmit
- **Map/Reduce** (`ss21-mapreduce`) - Map/Reduce script with all four phases
- **Scheduled Script** (`ss21-scheduled`) - Scheduled Script template
- **Client Script** (`ss21-client`) - Client Script with all event handlers
- **Portlet** (`ss21-portlet`) - Portlet Script template
- **Mass Update** (`ss21-massupdate`) - Mass Update Script template
- **Workflow Action** (`ss21-workflowaction`) - Workflow Action Script template
- **Bundle Installation** (`ss21-bundleinstall`) - Bundle Installation Script template
- **Module** (`ss21-module`) - Reusable module template

### SuiteScript 2.1 Helper Snippets

- **Search** (`ss21-search`) - Create and execute a search
- **Record Load** (`ss21-record-load`) - Load a record
- **Record Create** (`ss21-record-create`) - Create a new record
- **HTTP Request** (`ss21-http-request`) - Make an HTTP request
- **Try-Catch** (`ss21-try-catch`) - Try-catch block with error handling
- **Console Log** (`ss21-console-log`) - Console log message
- **Console Error** (`ss21-console-error`) - Console error message

### SuiteScript 1.0 Script Types (Legacy Syntax)

- **RESTlet** (`ss10-restlet`) - RESTlet with GET, POST, PUT, DELETE handlers
- **Suitelet** (`ss10-suitelet`) - Suitelet with GET and POST handling
- **User Event - Before Load** (`ss10-userevent-beforeload`) - Before Load event handler
- **User Event - Before Submit** (`ss10-userevent-beforesubmit`) - Before Submit event handler
- **User Event - After Submit** (`ss10-userevent-aftersubmit`) - After Submit event handler
- **User Event - Full** (`ss10-userevent`) - Complete User Event with all handlers
- **Scheduled Script** (`ss10-scheduled`) - Scheduled Script template
- **Client Script** (`ss10-client`) - Client Script with all event handlers
- **Portlet** (`ss10-portlet`) - Portlet Script template
- **Mass Update** (`ss10-massupdate`) - Mass Update Script template
- **Workflow Action** (`ss10-workflowaction`) - Workflow Action Script template
- **Bundle Installation** (`ss10-bundleinstall`) - Bundle Installation Script template

### SuiteScript 1.0 Helper Snippets

- **Search** (`ss10-search`) - Create and execute a search with pagination
- **Search - Simple** (`ss10-search-simple`) - Simple search without pagination
- **Record Load** (`ss10-record-load`) - Load a record
- **Record Create** (`ss10-record-create`) - Create a new record
- **Get/Set Field** (`ss10-getfield`, `ss10-setfield`) - Field operations
- **Get/Set Line Item** (`ss10-getlineitem`, `ss10-setlineitem`) - Sublist operations
- **HTTP Request** (`ss10-http-request`) - Make an HTTP request
- **Schedule Script** (`ss10-schedule-script`) - Schedule a script
- **Submit/Lookup Field** (`ss10-submit-field`, `ss10-lookup-field`) - Field utilities
- **Transform Record** (`ss10-transform-record`) - Transform records
- **Log Execution** (`ss10-log`) - Logging
- **Context/User/Role** (`ss10-get-context`, `ss10-get-user`, `ss10-get-role`) - Context info
- **Client Dialogs** (`ss10-alert`, `ss10-confirm`) - Client-side dialogs
- **Try-Catch** (`ss10-try-catch`) - Error handling

## 🎯 Highlights

- ✅ **Dual Version Support** - Both SuiteScript 1.0 and 2.1
- ✅ **50 Total Snippets** - Comprehensive coverage of all script types
- ✅ **Modern Syntax** - ECMA 6 for SuiteScript 2.1 (arrow functions, const/let)
- ✅ **Legacy Support** - Traditional function syntax for SuiteScript 1.0
- ✅ **JSDoc Annotations** - Better IntelliSense and documentation
- ✅ **Tab Stops** - Quick navigation through placeholders
- ✅ **Error Handling** - Proper try-catch patterns included
- ✅ **Attribution** - @author tag for code ownership

## 📋 Requirements

- Visual Studio Code 1.80.0 or higher
- JavaScript language support

## 📝 License

This project is licensed under a **Custom Source-Available License**.

This means:
- ✅ You can fork this repository and modify it
- ✅ You can use it in your own projects (personal or commercial)
- ✅ You can use the code in your own work
- ❌ You cannot create standalone copies or redistributions
- ❌ You cannot republish this as your own work
- ⚠️ All forks must maintain attribution to the original author
- ⚠️ Public forks must link back to the original repository

See the [LICENSE](LICENSE) file for full details.

## 📧 Contact

**Clemen Canaria** - [CanariaWerx](https://github.com/ccanaria/suitescript-snippets)  
📧 clemen [at] canariawerx [dot] com

---

## 📋 Full Changelog

### v1.1.0 (January 22, 2026)
- ✨ Added complete SuiteScript 1.0 support with 30+ snippets
- ✨ All major script types for SuiteScript 1.0
- ✨ Comprehensive helper snippets for common operations
- ✨ Consistent naming convention with `ss10-` prefix
- 📝 Updated documentation and examples

### v1.0.0 (January 22, 2026)
- 🎉 Initial release
- ✨ Complete SuiteScript 2.1 support
- ✨ All major script types with ECMA 6 syntax
- ✨ Helper snippets for common operations
