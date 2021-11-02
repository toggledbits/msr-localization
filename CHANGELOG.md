# Change Log

**NOTE: It is recommended that users translating from any base version of the US English file use the `ref_version` key to track the version of that file used to create/update their translation files.** That is, if you set `ref_version` to 21275, you will know in future that you made your translation up-to-date and in parity with US English version 21275, so future new versions can more easily focus on changes since that version. Also, check out the `txtool.js` file in the `tools` subdirectory of your Reactor install directory.

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
