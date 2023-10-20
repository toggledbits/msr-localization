# Change Log

**NOTE: It is recommended that users translating from any base version of the US English file use the `ref_version` key to track the version of that file used to create/update their translation files.** That is, if you set `ref_version` to 21275, you will know in future that you made your translation up-to-date and in parity with US English version 21275, so future new versions can more easily focus on changes since that version. Also, check out the `txtool.js` file in the `tools` subdirectory of your Reactor install directory.

For "New Strings", please refer to the reference file for comments/specifics/recommendations regarding usage.

## 23196

* The "Number formatting" strings `decimal_sep` and `thousands_sep` are deprecated and will be removed from a future file. Localization of numbers is handled by Node/JS-native localization data (always has been).
* The short and long weekday and month names are now only used if provided; if they are not provided (i.e. are not defined at all in the file, which is now recommended), the Node/JS-native localization data will be used for translation. They have been removed from the reference (en-US) file.

New Strings:

    '#action-form-warning'
    '#cond-op-nottrue'
    '#cond-op-notfalse'
    '#opt-current-reaction'
    '#action-desc-stop-current'
    "The global expression {0:q} ({1}) could not be evaluated"
    "An Entity Attribute condition in rule {0:q} ({1}) failed because the referenced entity {2} ({3}) does not have attribute {4}"
    'An "Expression Value" condition in rule {0:q} ({1}) references an expression {2:q} of rule {3:q} ({4}) that no longer exists.'
    'An "Expression Value" condition in rule {0:q} ({1}) references a local expression {2:q} that no longer exists.'
    'An Expression Value condition in rule {0:q} ({1}) references rule {2:q}, which no longer exists.'
    'An "Expression Value" condition in rule {0:q} ({1}) references global expression {2:q}, which no longer exists.'
    'Rule {0:q} ({1}) failed because an Interval condition references a dependent condition that no longer exists.'
    'Rule {0:q} ({1}) failed because it contains a condition of type {2:q}, which is not a recognized condition type'
    'Rule {0:q} ({1}) could not start because of an error; please refer to the log file.'

Modified Strings:
    '#cond-group-disable-tip'

Retired Strings:
    "An Entity Attribute condition in rule {0:q} failed because the referenced entity {1} could not be found": >
    "An Entity Attribute condition in rule {0:q} failed because the referenced entity {1} ({2}) does not have attribute {3}": >
    'An "Expression Value" condition in rule {0:q} references a local expression {1:q} that no longer exists.': >
    'An "Expression Value" condition in rule {0:q} references an expression {1:q} of rule {2:q} that no longer exists.': >
    'An Expression Value condition in rule {0:q} references rule {1:q}, which no longer exists.': >
    'An "Expression Value" condition in rule {0:q} references global expression {1:q}, which no longer exists.': >
    'Rule {0:q} failed because an Interval condition references a dependent condition that no longer exists.': >
    'Rule {0:q} failed because it contains a condition of type {1}, which is not a recognized condition type': >
    'Rule {0:q} could not start because of an error; please refer to the log file.': >

## 22306

New Strings:

    'Stop this reaction/task'
    'Enter comment text'
    'Content hidden'
    '#reactor-update-available': 'A new version of Reactor is available ({0}-{1}). {2}'
    '#reactor-update-message': 'Please upgrade to get the latest bug fixes and features.'

## 22292

* Changed string `#condopt-sustain` to `'#condopt-sustain': 'for {0:"less than "?:lt}{0:"at least "?!:lt}{1} secs` to fix incorrect text for sustained-for option with "less than" operator (specifically, the `<` character was changed to the correct `lt` string in both substitutions).

New Strings:

    'minutes after'
    'minutes before'
    'Wait for completion'
    '#action-desc-run-wait': ' (wait for it to finish)'
    '#action-desc-run-continue': ' (do not wait for it to finish)'

## 22140

* Fixed the new entity discovery message entry ("Discovered new device {0:q} ({1}) on controller {2:q}") value to match the key. The key was the correct/desired string, but along the way it had been updated prior to release and the changes were not applied to the value. They now match.

## 22131

New Strings:

* 'Controller ID: {0}'

## 22124

New Strings:

* 'Rule History'
* 'Reaction History'
* 'Controller Status'
* 'Click to add a new widget'
* 'About Status Panel Widgets'
* '#status-widget-info-text': 'This is the Status Panel. Each element of the Status Panel is a "widget" that you can customize. Drag a widget to move it. Resize a widget by grabbing the resize handle in its bottom right corner and dragging. Remove a widget by dragging it out of the Status Panel (over the left navigation area). Add a new widget by clicking the "Add Widget" widget (scroll down). You can change this widget to something else by choosing a new type below:'
* 'Choose Widget:'
* 'New Widget'
* '#entity-rename-button-label': 'Rename'
* '#entity-rename-title': 'Rename Entity'
* '#entity-rename-input-label': 'New Name'
* '#entity-rename-advice': 'Renaming an entity only renames it in Reactor, it does not change the name at the hub/source. If the source object supports renaming at the source, you may want to do it there.'
* '#entity-rename-button-cancel': 'Cancel'
* '#entity-rename-button-rename': 'Rename'
* '#entity-delete-button-label': 'Delete'
* '#entity-delete-title': 'Delete Entity'
* '#entity-delete-button-cancel': 'Cancel'
* '#entity-delete-button-delete': 'Delete'
* '#entity-delete-body': 'Deleting an entity removes it from Reactor but does not remove it from the hub/source. If the source object still exists, the entity will be recreated next time the source is inventoried.'
* '#entity-missing-alert': 'The entity is marked missing from the hub'
* '#condrestrict-seq-conds': 'Eligible Conditions'
* '#cond-button-clone': 'Clone condition'
* '#grp-button-clone': 'Clone group'
* '{0} (DEPRECATED)'
* '#reaction-while': 'Repeat While...'
* '#default-group-name': 'Group Constraints'
* '#default-while-name': 'Repeat Conditions'
* 'An Entity Attribute condition in {0:q} ({1}) failed because the referenced entity {2:q} could not be found'
* 'Controller {0} device {1:q} ({2}) no longer exists.'
* 'Discovered new device {0:q} ({1}) on controller {2:q}'

## 21340

New Strings:

* '#reaction-delay-for': 'for'
* '; save response to {0:q} {1} ({2})'
* '; capture output to {0:q} {1} ({2})'
* '; capture output to {0:q} (local)'
* '; capture output to {0:q} (global)'
* '#action-desc-delay-inline': 'Delay for {0} seconds'
* '#action-desc-delay-start': 'Delay for {0} seconds from start of reaction'
* '#action-desc-comment': 'Comment: {0}'
* '#action-desc-perform': 'Perform {0} on {1}{2:" with "?#>0}{2}'
* '#action-desc-setvar-rule': 'Set Variable {0} in {1} to {2}{3:" and re-evaluate"?t}'
* '#action-desc-setvar-global': 'Set Variable {0} to {1}{2:" and re-evaluate"?t}'
* '#action-desc-run-global': 'Run global reaction {0} ({1})'
* '#action-desc-run-rule': 'Run rule {0} ({1}) {2:"Set"?t}{2:"Reset"?f} reaction'
* '#action-desc-stop-global': 'Stop global reaction {0} ({1})'
* '#action-desc-stop-rule': 'Stop rule {0} ({1}) {2:"Set"?t}{2:"Reset"?f} reaction'
* '#action-desc-notify': 'Notify via {0}: {1}'
* '#action-desc-request': 'Request HTTP {0} {1:q}{2:"; wait for completion"?#t}'
* '#action-desc-shell': 'Shell command: {0:q}{1:" (ignore exit code)"?t}'
* '#action-desc-unrecognized': 'Unrecognized action type {0:q}? {1}'

Modified Strings (these modifications are safe for all versions of Reactor current and prior):

* '#sun-desc-after': 'after {1:#D?!=0}{1:" minutes"?!=0}{1:" before"?<0}{1:" after"?>0"} {0:T}'
* '#sun-desc-before': 'before {1:#D?!=0}{1:" minutes"?!=0}{1:" before"?<0}{1:" after"?>0"} {0:T}'

Retired Strings (do not delete from your data, just move them or mark them somehow)

* '; save response to {0:q} ({1})': '; save response to {0:q} ({1})'  # 0=varname, 1=rule [RETIRED]

## 21332

New strings:

* '#cond-op-empty': 'is EMPTY'
* '#cond-op-notempty': 'is not EMPTY'

Modified Strings:

* Please ensure that the string tagged '#sun-desc-nob' is for *NOT between (time) and (time).

## 21305

New strings:

* '#alert-time-last': 'Last {0}'
* 'HTTP Auth Type:'
* 'Username:'
* 'Password:'
* '#reaction-subst-failed-eval': 'Reaction {0:q} ({1}) step {2} substitution failed because the expression {3:q} could not be evaluated'

Disused strings (do not remove -- see [docs](https://reactor.toggledbits.com/docs/Localization/#practices-and-guidelines-for-translators) for recommended handling):

* 'Reaction {0:q} ({1}) step {2} variable substitution failed because the expression {3:q} could not be compiled'
* "Reaction {0:q} ({1}) step {2} HTTP request can't set JSON response to variable {3}"
* "Reaction {0:q} ({1}) step {2} HTTP request couldn't retrieve/parse server's JSON response"
* "Reaction {0:q} ({1}) step {2} HTTP request couldn't retrieve server's response"
* "Reaction {0:q} ({1}) step {2} HTTP request can't set error/null response to variable {3}"
* "Reaction {0:q} ({1}) step {2} HTTP request can't set error/null response to variable {3:q}"

## 21286

New strings:

* '#rule-update-rate': 'Rule {0:q} is being throttled because its update rate exceeds {1} updates per minute. Check for logic errors that may be causing an evaluation loop, or devices that are "flapping".'
* '#rule-change-rate': 'Rule {0:q} is being throttled because it has changed state more than {1} times in the last minute. Check for a "flapping" device or a loop in your logic.'

## 21284

New strings:

* 'Link to documentation for topic'  # tooltip for help icon/docs link

## 21281

New strings:

* '#ep-col-entity': 'Entity'
* '#ep-col-id': 'ID'
* '#cond-desc-between': '{0} and {1}'  # condition description, between/not operands
* '#cond-desc-changes': 'from {0} to {1}'  # condition description, changes terminal operands
* '(any)'  # condition description, changes terminal operand default

Changes:

* '{0} -- {1} as of {2}': The previous use of `{1:T}` should be changed to simply `{1}`, as the code now handles the boolean value itself and passes the translated value into this string (so no need to put it back through the translator as 1:T does).

## 21277

New strings:

* '#group-status-no-data': '(no data)'
* 'Rule ID: {0}'
* 'Perform {0}'
* '{0} -- {1} as of {2}'
* 'Current value: not set'
* 'Current value: ({0}) {1}'
* 'yyyy'
* 'imported triggers'
* 'imported constraints'
* '#cond-group-op-not': 'NOT'
* '#cond-group-op-and': 'AND'
* '#cond-group-op-or': 'OR'
* '#cond-group-op-xor': 'XOR'
* '#cond-group-op-nul': 'NUL'
* '#cond-group-state-disabled': 'DISABLED'
* '({0}) {1}'
* "Add your rule's triggers here"
* 'Add your actions here.'
* '#data-type-string': 'string'
* '#data-type-number': 'number'
* '#data-type-boolean': 'boolean'
* '#data-type-object': 'object'
* '#data-type-array': 'array'
* '#data-type-array-len': 'array:{0}'
* '#data-type-undefined': 'undefined'
* '#data-type-null': 'null'
* 'null'
* '{0}? (missing)'

Removed:

* 'Current value: {0}'
* '(not set)'
* '#cond-button-not'
* '#cond-button-and'
* '#cond-button-or'
* '#cond-button-xor'
* '#cond-button-nul'

## 21275

New:

* 'Local (browser) time'
* 'Host time'
* 'Suppress alerts on HTTP errors'
* '#http-req-subst-notice': 'Note: this action allows in-line substitutions in all text fields using \<tt>${{expr}}\</tt> syntax.'

Modified strings/key changes:

* The misspelled word `expxression` has been corrected to `expression` throughout (key must be fixed in two strings).
* The string "Rule {0:q}  does not exist" had double-space before "does", now corrected to a single space (key must be fixed).

## 21269

New:

* 'There are no set rules at this moment'
* '#rule-control-copy': 'Copy/Move Rule'
* 'Wait until request completes'
* '#deprecated-action-use': '(deprecated; use {0:q})'  # 0=replacement action
* '#deprecated-action': '(deprecated with no replacement)'
* '; save response to {0:q} ({1})'  # 0=varname, 1=rule
* '; save response to {0:q} (local)'  # 0=varname
* '; save response to {0:q} (global)' # 0=varname
* 'Auto-evaluate on dependency changes'  # tooltip

## 21257

* First version checked in.
