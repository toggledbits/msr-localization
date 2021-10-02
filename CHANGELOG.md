# Change Log

**NOTE: It is recommended that users translating from any base version of the US English file use the `ref_version` key to track the version of that file used to create/update their translation files.** That is, if you set `ref_version` to 21275, you will know in future that you made your translation up-to-date and in parity with US English version 21275, so future new versions can more easily focus on changes since that version. Also, check out the `txtool.js` file in the `tools` subdirectory of your Reactor install directory.

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
