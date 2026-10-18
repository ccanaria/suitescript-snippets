# SuiteScript Code Snippets

**Author:** Clemen Canaria  
**Email:** clemen [at] canariawerx [dot] com  
**Organization:** CanariaWerx

A comprehensive collection of VS Code snippets for NetSuite SuiteScript development, supporting both SuiteScript 1.0 and SuiteScript 2.1.

## Features

This extension provides code snippets for all major SuiteScript script types and common patterns, supporting both SuiteScript 1.0 and 2.1.

### SuiteScript 2.1 (ECMA 6 Syntax)

#### Script Types
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

#### Helper Snippets
- **Search** (`ss21-search`) - Create and execute a search
- **Record Load** (`ss21-record-load`) - Load a record
- **Record Create** (`ss21-record-create`) - Create a new record
- **HTTP Request** (`ss21-http-request`) - Make an HTTP request
- **Try-Catch** (`ss21-try-catch`) - Try-catch block with error handling
- **Console Log** (`ss21-console-log`) - Console log message
- **Console Error** (`ss21-console-error`) - Console error message

### SuiteScript 1.0 (Legacy Syntax)

#### Script Types
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

#### Helper Snippets
- **Search** (`ss10-search`) - Create and execute a search with pagination
- **Search - Simple** (`ss10-search-simple`) - Simple search without pagination
- **Record Load** (`ss10-record-load`) - Load a record
- **Record Create** (`ss10-record-create`) - Create a new record
- **Get Field Value** (`ss10-getfield`) - Get field value
- **Set Field Value** (`ss10-setfield`) - Set field value
- **Get Line Item Value** (`ss10-getlineitem`) - Get sublist line item value
- **Set Line Item Value** (`ss10-setlineitem`) - Set sublist line item value
- **HTTP Request** (`ss10-http-request`) - Make an HTTP request
- **Schedule Script** (`ss10-schedule-script`) - Schedule a script to run
- **Submit Field** (`ss10-submit-field`) - Submit a single field value
- **Lookup Field** (`ss10-lookup-field`) - Lookup field without loading record
- **Transform Record** (`ss10-transform-record`) - Transform one record to another
- **Log Execution** (`ss10-log`) - Log execution message
- **Try-Catch** (`ss10-try-catch`) - Try-catch block with error handling
- **Get Context** (`ss10-get-context`) - Get execution context
- **Get User** (`ss10-get-user`) - Get current user ID
- **Get Role** (`ss10-get-role`) - Get current role ID
- **Alert** (`ss10-alert`) - Show alert dialog (client-side)
- **Confirm** (`ss10-confirm`) - Show confirmation dialog (client-side)

## Usage

1. Open a JavaScript file in VS Code
2. Start typing the snippet prefix:
   - For SuiteScript 2.1: `ss21-` (e.g., `ss21-restlet`)
   - For SuiteScript 1.0: `ss10-` (e.g., `ss10-restlet`)
3. Press `Tab` or `Enter` to insert the snippet
4. Use `Tab` to navigate through placeholders

## Examples

### SuiteScript 2.1
Type `ss21-restlet` and press Tab to insert:

```javascript
/**
 * @NApiVersion 2.1
 * @NScriptType Restlet
 * @author Your Name
 */
define([], () => {
    
    /**
     * GET request handler
     * @param {Object} requestParams - Request parameters
     * @returns {Object} Response object
     */
    const get = (requestParams) => {
        try {
            
            return { success: true, data: {} };
        } catch (e) {
            return { success: false, error: e.message };
        }
    };
    
    // ... more handlers
    
    return { get, post, put, delete: doDelete };
});
```

### SuiteScript 1.0
Type `ss10-restlet` and press Tab to insert:

```javascript
/**
 * RESTlet Name
 * @author Your Name
 */

/**
 * GET request handler
 * @param {Object} datain - Request parameters
 * @returns {Object} Response object
 */
function get(datain) {
    try {
        
        return { success: true, data: {} };
    } catch (e) {
        return { success: false, error: e.toString() };
    }
}

// ... more handlers
```

## Key Features

- ✅ **Dual Version Support** - Both SuiteScript 1.0 and 2.1
- ✅ **Modern Syntax** - ECMA 6 for SuiteScript 2.1 (arrow functions, const/let, destructuring)
- ✅ **Legacy Support** - Traditional function syntax for SuiteScript 1.0
- ✅ **JSDoc Annotations** - Better IntelliSense and code documentation
- ✅ **Tab Stops** - Quick navigation through placeholders
- ✅ **Error Handling** - Proper try-catch patterns included
- ✅ **Attribution** - @author tag for code ownership

## Requirements

- Visual Studio Code 1.80.0 or higher
- JavaScript language support

## Installation

### Method 1: From VS Code Marketplace (Recommended)
1. Open VS Code
2. Go to Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X` on Mac)
3. Search for "CanariaWerx SuiteScript Snippets"
4. Click **Install**
5. Reload VS Code if prompted

### Method 2: From VSIX File
1. Download the `.vsix` file from the releases page
2. Open VS Code
3. Go to Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X` on Mac)
4. Click the "..." menu (three dots) at the top of the Extensions view
5. Select **Install from VSIX...**
6. Navigate to and select the downloaded `.vsix` file
7. Reload VS Code if prompted

### Method 3: From Source (For Development)
1. Clone this repository:
   ```bash
   git clone https://github.com/ccanaria/suitescript-snippets.git
   cd suitescript-snippets
   ```
2. Copy the folder to your VS Code extensions directory:
   - **Windows**: `%USERPROFILE%\.vscode\extensions\suitescript-snippets`
   - **macOS/Linux**: `~/.vscode/extensions/suitescript-snippets`
3. Restart VS Code

## How to Use

### Basic Usage
1. **Open or create** a JavaScript file (`.js`) in VS Code
2. **Type** the snippet prefix (e.g., `ss21-restlet`)
3. **Select** the snippet from the IntelliSense dropdown that appears
4. **Press** `Tab` or `Enter` to insert the snippet
5. **Navigate** through placeholder fields using `Tab`
6. **Fill in** the placeholders with your specific values

### Triggering IntelliSense
If the snippet dropdown doesn't appear automatically:
- Press `Ctrl+Space` (Windows/Linux) or `Cmd+Space` (Mac) to manually trigger IntelliSense
- Start typing the snippet prefix more completely

### Available Snippet Prefixes

**SuiteScript 2.1** - All snippets start with `ss21-`:
- `ss21-restlet`, `ss21-suitelet`, `ss21-userevent`, `ss21-mapreduce`
- `ss21-scheduled`, `ss21-client`, `ss21-portlet`, `ss21-massupdate`
- `ss21-workflowaction`, `ss21-bundleinstall`, `ss21-module`
- `ss21-search`, `ss21-record-load`, `ss21-record-create`
- `ss21-http-request`, `ss21-try-catch`
- `ss21-console-log`, `ss21-console-error`

**SuiteScript 1.0** - All snippets start with `ss10-`:
- `ss10-restlet`, `ss10-suitelet`, `ss10-userevent`
- `ss10-userevent-beforeload`, `ss10-userevent-beforesubmit`, `ss10-userevent-aftersubmit`
- `ss10-scheduled`, `ss10-client`, `ss10-portlet`, `ss10-massupdate`
- `ss10-workflowaction`, `ss10-bundleinstall`
- `ss10-search`, `ss10-search-simple`, `ss10-record-load`, `ss10-record-create`
- `ss10-getfield`, `ss10-setfield`, `ss10-getlineitem`, `ss10-setlineitem`
- `ss10-http-request`, `ss10-schedule-script`, `ss10-submit-field`
- `ss10-lookup-field`, `ss10-transform-record`, `ss10-log`, `ss10-try-catch`
- `ss10-get-context`, `ss10-get-user`, `ss10-get-role`
- `ss10-alert`, `ss10-confirm`

### Tips for Maximum Productivity
- **Enable Tab Completion**: Ensure tab completion is enabled in VS Code settings
  - Go to `File > Preferences > Settings` (or `Code > Preferences > Settings` on Mac)
  - Search for "tab completion"
  - Set `editor.tabCompletion` to `on` or `onlySnippets`
- **View All Snippets**: 
  - Type `ss21-` and press `Ctrl+Space` for SuiteScript 2.1 snippets
  - Type `ss10-` and press `Ctrl+Space` for SuiteScript 1.0 snippets
- **Customize Snippets**: You can modify snippets in VS Code by going to `File > Preferences > Configure User Snippets > javascript.json`
- **Use Multi-Cursor**: Use `Alt+Click` (Windows/Linux) or `Option+Click` (Mac) to edit multiple placeholders simultaneously

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

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

## Author

**Clemen Canaria** - [CanariaWerx](https://github.com/ccanaria/suitescript-snippets)  
📧 clemen [at] canariawerx [dot] com

## Release Notes

### 1.1.0

Added complete SuiteScript 1.0 support with 30+ snippets for legacy script development.

### 1.0.0

Initial release with support for all major SuiteScript 2.1 script types and common patterns.
