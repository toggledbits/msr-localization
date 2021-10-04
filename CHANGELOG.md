# Change Log

**NOTE: It is recommended that users translating from any base version of the US English file use the `ref_version` key to track the version of that file used to create/update their translation files.** That is, if you set `ref_version` to 21275, you will know in future that you made your translation up-to-date and in parity with US English version 21275, so future new versions can more easily focus on changes since that version. Also, check out the `txtool.js` file in the `tools` subdirectory of your Reactor install directory.

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
