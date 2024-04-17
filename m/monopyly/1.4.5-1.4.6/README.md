# Comparing `tmp/monopyly-1.4.5.tar.gz` & `tmp/monopyly-1.4.6.tar.gz`

## Comparing `monopyly-1.4.5.tar` & `monopyly-1.4.6.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 monopyly-1.4.5/README.md -> monopyly/README.md
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/README.md
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/_version.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/auth/actions.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/auth/blueprint.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/auth/routes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/auth/tools.py
--rw-r--r--   0        0        0     9828 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/banking/accounts.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/banking/actions.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/banking/banks.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/banking/blueprint.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/banking/filters.py
--rw-r--r--   0        0        0    10506 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/banking/forms.py
--rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/banking/routes.py
--rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/banking/transactions.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/cli/apps.py
--rwxr-xr-x   0        0        0     3838 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/cli/run.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/common/transactions.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/common/utils.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/common/forms/__init__.py
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/common/forms/_forms.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/common/forms/fields.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/common/forms/utils.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/common/forms/validators.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/config/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/config/default_settings.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/config/settings.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/core/actions.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/core/blueprint.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/core/context_processors.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/core/filters.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/core/internal_transactions.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/core/routes.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/credit/accounts.py
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/credit/actions.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/credit/blueprint.py
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/credit/cards.py
--rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/credit/forms.py
--rw-r--r--   0        0        0    17880 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/credit/routes.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/credit/statements.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/credit/transactions/__init__.py
--rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/credit/transactions/_transactions.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/database/__init__.py
--rw-r--r--   0        0        0    15095 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/database/models.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/database/preloads.sql
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/database/schema.sql
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/database/views.sql
--rw-r--r--   0        0        0    87462 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/jquery-3.7.0.min.js
--rw-r--r--   0        0        0    48860 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/css/style.css
--rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/browserconfig.xml
--rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-114.png
--rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-120.png
--rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-144.png
--rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-150.png
--rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-152.png
--rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-16.png
--rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-160.png
--rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-180.png
--rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-192.png
--rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-310.png
--rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-32.png
--rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-57.png
--rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-60.png
--rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-64.png
--rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-70.png
--rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-72.png
--rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-76.png
--rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon-96.png
--rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon.ico
--rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/favicon/favicon.png
--rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/statement.png
--rw-r--r--   0        0        0   370982 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/about/bank-account-details.png
--rw-r--r--   0        0        0   389739 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/about/bank-account-summaries.png
--rw-r--r--   0        0        0   387290 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/about/bank-accounts.png
--rw-r--r--   0        0        0   373677 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/about/credit-account-details.png
--rw-r--r--   0        0        0   452288 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/about/credit-transactions.png
--rw-r--r--   0        0        0   551891 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/about/homepage-user.png
--rw-r--r--   0        0        0   277799 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/about/homepage.png
--rw-r--r--   0        0        0   434617 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/about/statement-details.png
--rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/cards/chase-card.png
--rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/cards/discover-card.png
--rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/cards/new-card.png
--rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/cards/template-card.png
--rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/arrow-down.png
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/arrow-left.png
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/arrow-up.png
--rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/checkmark.png
--rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/delete-orange-thick.png
--rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/delete-orange.png
--rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/delete-thick.png
--rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/delete.png
--rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/edit.png
--rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/link.png
--rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/minus-thick.png
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/minus.png
--rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/plus-thick.png
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/plus.png
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/refresh.png
--rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/save.png
--rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/sort-asc.png
--rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/sort-desc.png
--rw-r--r--   0        0        0    53387 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/statement-pair.svg
--rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/statement.png
--rw-r--r--   0        0        0    50319 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/statement.svg
--rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/img/icons/x-thick.png
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/add-subtransaction.js
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/add-transfer.js
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/autocomplete-transaction.js
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/bind-tag-actions.js
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/create-balance-chart.js
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/define-filter.js
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/display-new-account-type-inputs.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/display-new-bank-inputs.js
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/display-new-credit-account-inputs.js
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/expand-bank-account.js
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/expand-bank.js
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/expand-transaction.js
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/flip-card.js
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/hide-homepage-block.js
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/infer-card.js
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/infer-statement.js
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/make-payment.js
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/show-linked-transaction.js
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/update-account-statement-parameters.js
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/update-bank-name.js
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/update-card-status.js
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/update-statement-parameters.js
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/update-statements-display.js
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/update-transactions-display.js
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/modules/ajax.js
--rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/modules/autocomplete-input.js
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/modules/expand-box-row.js
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/modules/expand-transaction.js
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/modules/manage-acquisition-form.js
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/modules/manage-overlays.js
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/modules/manage-subforms.js
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/modules/update-database-widget.js
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/static/js/modules/update-display-ajax.js
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credits.html
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/index.html
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/layout.html
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/profile.html
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/story.html
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/auth/login.html
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/auth/register.html
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/account_page.html
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/account_summaries.html
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/account_summaries_page.html
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/account_summary.html
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/accounts_page.html
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/account_form/account_form.html
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/account_form/account_form_page_new.html
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transaction_form/bank_info_form.html
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transaction_form/transfer_form.html
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/banking/transactions_table/transactions.html
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/form_page.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transaction_form/subform.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transaction_form/subtransaction_subform.html
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transactions_table/linked_bank_transaction.html
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transactions_table/linked_credit_transaction.html
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transactions_table/subtransactions.html
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transactions_table/transaction_condensed.html
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transactions_table/transaction_expanded.html
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/common/transactions_table/transactions.html
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/account_page.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/card_submission_page.html
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/cards.html
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/cards_page.html
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/statement_page.html
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/statement_summary.html
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/statements.html
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/statements_page.html
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/tags_page.html
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transaction_submission_page.html
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transactions_page.html
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/card_form/card_form.html
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/card_form/card_form_page_new.html
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/card_graphic/card_back.html
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/card_graphic/card_front.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/tag_tree/subtag_tree.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/tag_tree/tag_tree.html
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.4.5/monopyly/templates/credit/transactions_table/transactions.html
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 monopyly-1.4.5/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.4.5/COPYING
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.4.5/LICENSE
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 monopyly-1.4.5/pyproject.toml
--rw-r--r--   0        0        0    10206 2020-02-02 00:00:00.000000 monopyly-1.4.5/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 monopyly-1.4.6/README.md -> monopyly/README.md
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/README.md
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/_version.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/auth/actions.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/auth/blueprint.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/auth/routes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/auth/tools.py
+-rw-r--r--   0        0        0     9828 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/accounts.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/actions.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/banks.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/blueprint.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/filters.py
+-rw-r--r--   0        0        0    10506 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/forms.py
+-rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/routes.py
+-rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/transactions.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/cli/apps.py
+-rwxr-xr-x   0        0        0     3838 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/cli/run.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/transactions.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/utils.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/__init__.py
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/_forms.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/fields.py
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/utils.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/validators.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/config/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/config/default_settings.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/config/settings.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/actions.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/blueprint.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/context_processors.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/filters.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/internal_transactions.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/routes.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/accounts.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/actions.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/blueprint.py
+-rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/cards.py
+-rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/forms.py
+-rw-r--r--   0        0        0    17794 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/routes.py
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/statements.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/transactions/__init__.py
+-rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/transactions/_transactions.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/__init__.py
+-rw-r--r--   0        0        0    15095 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/models.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/preloads.sql
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/schema.sql
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/views.sql
+-rw-r--r--   0        0        0    87462 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/jquery-3.7.0.min.js
+-rw-r--r--   0        0        0    48930 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/css/style.css
+-rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/browserconfig.xml
+-rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-114.png
+-rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-120.png
+-rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-144.png
+-rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-150.png
+-rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-152.png
+-rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-16.png
+-rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-160.png
+-rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-180.png
+-rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-192.png
+-rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-310.png
+-rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-32.png
+-rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-57.png
+-rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-60.png
+-rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-64.png
+-rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-70.png
+-rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-72.png
+-rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-76.png
+-rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-96.png
+-rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon.ico
+-rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon.png
+-rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/statement.png
+-rw-r--r--   0        0        0   370982 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/bank-account-details.png
+-rw-r--r--   0        0        0   389739 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/bank-account-summaries.png
+-rw-r--r--   0        0        0   387290 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/bank-accounts.png
+-rw-r--r--   0        0        0   373677 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/credit-account-details.png
+-rw-r--r--   0        0        0   452288 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/credit-transactions.png
+-rw-r--r--   0        0        0   551891 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/homepage-user.png
+-rw-r--r--   0        0        0   277799 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/homepage.png
+-rw-r--r--   0        0        0   434617 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/statement-details.png
+-rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/cards/chase-card.png
+-rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/cards/discover-card.png
+-rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/cards/new-card.png
+-rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/cards/template-card.png
+-rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/arrow-down.png
+-rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/arrow-left.png
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/arrow-up.png
+-rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/checkmark.png
+-rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/delete-orange-thick.png
+-rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/delete-orange.png
+-rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/delete-thick.png
+-rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/delete.png
+-rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/edit.png
+-rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/link.png
+-rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/minus-thick.png
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/minus.png
+-rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/plus-thick.png
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/plus.png
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/refresh.png
+-rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/save.png
+-rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/sort-asc.png
+-rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/sort-desc.png
+-rw-r--r--   0        0        0    53387 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/statement-pair.svg
+-rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/statement.png
+-rw-r--r--   0        0        0    50319 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/statement.svg
+-rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/x-thick.png
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/add-subtransaction.js
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/add-transfer.js
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/autocomplete-transaction.js
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/bind-tag-actions.js
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/create-balance-chart.js
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/define-filter.js
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/display-new-account-type-inputs.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/display-new-bank-inputs.js
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/display-new-credit-account-inputs.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/expand-bank-account.js
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/expand-bank.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/expand-transaction.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/flip-card.js
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/hide-homepage-block.js
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/infer-card.js
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/infer-statement.js
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/make-payment.js
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/show-linked-transaction.js
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-account-statement-parameters.js
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-bank-name.js
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-card-status.js
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-statement-parameters.js
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-statements-display.js
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-transactions-display.js
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/ajax.js
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/autocomplete-input.js
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/expand-box-row.js
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/expand-transaction.js
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/manage-acquisition-form.js
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/manage-overlays.js
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/manage-subforms.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/update-database-widget.js
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/update-display-ajax.js
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credits.html
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/index.html
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/layout.html
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/profile.html
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/story.html
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/auth/login.html
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/auth/register.html
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_page.html
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_summaries.html
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_summaries_page.html
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_summary.html
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/accounts_page.html
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_form/account_form.html
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_form/account_form_page_new.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/bank_info_form.html
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transfer_form.html
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transactions_table/transactions.html
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/form_page.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transaction_form/subform.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transaction_form/subtransaction_subform.html
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_bank_transaction.html
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_credit_transaction.html
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/subtransactions.html
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/transaction_condensed.html
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/transaction_expanded.html
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/transactions.html
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/account_page.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_submission_page.html
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/cards.html
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/cards_page.html
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/statement_page.html
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/statement_summary.html
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/statements.html
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/statements_page.html
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/tags_page.html
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_submission_page.html
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_page.html
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_form/card_form.html
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_form/card_form_page_new.html
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_graphic/card_back.html
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_graphic/card_front.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/tag_tree/subtag_tree.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/tag_tree/tag_tree.html
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_table/transactions.html
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 monopyly-1.4.6/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.4.6/COPYING
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.4.6/LICENSE
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 monopyly-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0    10206 2020-02-02 00:00:00.000000 monopyly-1.4.6/PKG-INFO
```

### Comparing `monopyly-1.4.5/monopyly/README.md` & `monopyly-1.4.6/monopyly/README.md`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/__init__.py` & `monopyly-1.4.6/monopyly/__init__.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/auth/routes.py` & `monopyly-1.4.6/monopyly/auth/routes.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/auth/tools.py` & `monopyly-1.4.6/monopyly/auth/tools.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/banking/accounts.py` & `monopyly-1.4.6/monopyly/banking/accounts.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/banking/actions.py` & `monopyly-1.4.6/monopyly/banking/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/banking/banks.py` & `monopyly-1.4.6/monopyly/banking/banks.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/banking/filters.py` & `monopyly-1.4.6/monopyly/banking/filters.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/banking/forms.py` & `monopyly-1.4.6/monopyly/banking/forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/banking/routes.py` & `monopyly-1.4.6/monopyly/banking/routes.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/banking/transactions.py` & `monopyly-1.4.6/monopyly/banking/transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/cli/apps.py` & `monopyly-1.4.6/monopyly/cli/apps.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/cli/run.py` & `monopyly-1.4.6/monopyly/cli/run.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/common/transactions.py` & `monopyly-1.4.6/monopyly/common/transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/common/utils.py` & `monopyly-1.4.6/monopyly/common/utils.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/common/forms/_forms.py` & `monopyly-1.4.6/monopyly/common/forms/_forms.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -30,35 +30,35 @@
     that follows the same naming schema.
     """
 
     def prepopulate(self, entry):
         """
         Generate a duplicate prepopulated form.
 
-        Notes
-        -----
-        WTForms requires that a form be instantiated in order to be
-        able to properly introspect fields. Because of this, this method
-        will only return a duplicate form matching the type of the
-        form instance used to call it. Using the form's process method
-        will not properly handle enumeration of field lists, so it
-        can not be used as a replacement for populating an existing
-        form.
-
         Parameters
         ----------
         entry : database.models.Model
             A database entry from which to pull information for
             prepopulating the form.
 
         Returns
         -------
         form : EntryForm
             A duplicate form, prepopulated with the collected database
             information.
+
+        Notes
+        -----
+        WTForms requires that a form be instantiated in order to be
+        able to properly introspect fields. Because of this, this method
+        will only return a duplicate form matching the type of the
+        form instance used to call it. Using the form's process method
+        will not properly handle enumeration of field lists, so it
+        can not be used as a replacement for populating an existing
+        form.
         """
         data = self.gather_entry_data(entry)
         return self.__class__(data=data)
 
     @abstractmethod
     def gather_entry_data(self, entry):
         raise NotImplementedError(
```

### Comparing `monopyly-1.4.5/monopyly/common/forms/fields.py` & `monopyly-1.4.6/monopyly/common/forms/fields.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/common/forms/utils.py` & `monopyly-1.4.6/monopyly/common/forms/utils.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/common/forms/validators.py` & `monopyly-1.4.6/monopyly/common/forms/validators.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/config/default_settings.py` & `monopyly-1.4.6/monopyly/config/default_settings.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/config/settings.py` & `monopyly-1.4.6/monopyly/config/settings.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/core/actions.py` & `monopyly-1.4.6/monopyly/core/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/core/context_processors.py` & `monopyly-1.4.6/monopyly/core/context_processors.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/core/filters.py` & `monopyly-1.4.6/monopyly/core/filters.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/core/routes.py` & `monopyly-1.4.6/monopyly/core/routes.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/credit/accounts.py` & `monopyly-1.4.6/monopyly/credit/accounts.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/credit/actions.py` & `monopyly-1.4.6/monopyly/credit/actions.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def get_card_statement_grouping(cards):
     """
     Get groupings (by card) of credit card statements.
 
     Parameters
     ----------
-    cards : list of sqlite3.Row
+    cards : list of database.models.CreditCard
         The database card entries for which to get statements.
 
     Returns
     -------
     card_statements : dict
         A mapping between the card entries and a list of all
         corresponding statement entries for that card.
@@ -27,26 +27,53 @@
         card_statements[card] = CreditStatementHandler.get_statements(
             card_ids=(card.id,),
             sort_order="DESC",
         )
     return card_statements
 
 
+def get_statement_and_transactions(statement_id, transaction_sort_order="DESC"):
+    """
+    Given a statement ID, get the corresponding statement and transactions.
+
+    Parameters
+    ----------
+    statement_id : int
+        The ID of the statement to acquire.
+    transaction_sort_order : str
+        The order to sort transactions returned for the statement. The
+        default is 'DESC' for transactions sorted in descending order.
+
+    Returns
+    -------
+    statement : database.models.CreditStatementView
+        The statement with the given ID.
+    transactions : list of database.models.CreditTransactionView
+        All transactions on the statement with the given ID.
+    """
+    statement = CreditStatementHandler.get_entry(statement_id)
+    transactions = CreditTransactionHandler.get_transactions(
+        statement_ids=(statement_id,),
+        sort_order=transaction_sort_order,
+    )
+    return statement, transactions.all()
+
+
 def get_potential_preceding_card(card):
     """
     Get the card that this new card may be intended to replace (if any).
 
     When a new card is added, there is a good chance that it may be
     replacing an existing card. Check to see if there is a good
     candidate card that might be replaced (a single active card with an
     unpaid balance affiliated with the same account as the new card).
 
     Parameters
     ----------
-    card : sqlite3.Row
+    card : database.models.CreditCard
         The new card being added to the database.
 
     Returns
     -------
     preceding_card : sqlite3.Row
         A card that matches the criteria, which may be being replaced by
         the new card.
```

### Comparing `monopyly-1.4.5/monopyly/credit/cards.py` & `monopyly-1.4.6/monopyly/credit/cards.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/credit/forms.py` & `monopyly-1.4.6/monopyly/credit/forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/credit/routes.py` & `monopyly-1.4.6/monopyly/credit/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ..common.forms.utils import extend_field_list_for_ajax
 from ..common.transactions import get_linked_transaction
 from ..common.utils import dedelimit_float, parse_date, sort_by_frequency
 from .accounts import CreditAccountHandler
 from .actions import (
     get_card_statement_grouping,
     get_potential_preceding_card,
+    get_statement_and_transactions,
     make_payment,
     transfer_credit_card_statement,
 )
 from .blueprint import bp
 from .cards import CreditCardHandler, save_card
 from .forms import CardStatementTransferForm, CreditCardForm, CreditTransactionForm
 from .statements import CreditStatementHandler
@@ -173,19 +174,15 @@
     # Filter selected statements from the database
     return render_template("credit/statements.html", card_statements=card_statements)
 
 
 @bp.route("/statement/<int:statement_id>")
 @login_required
 def load_statement_details(statement_id):
-    statement = CreditStatementHandler.get_entry(statement_id)
-    transactions = CreditTransactionHandler.get_transactions(
-        statement_ids=(statement_id,),
-        sort_order="DESC",
-    )
+    statement, transactions = get_statement_and_transactions(statement_id)
     # Get bank accounts for potential payments
     bank_accounts = BankAccountHandler.get_accounts()
     return render_template(
         "credit/statement_page.html",
         statement=statement,
         statement_transactions=transactions,
         bank_accounts=bank_accounts,
```

### Comparing `monopyly-1.4.5/monopyly/credit/statements.py` & `monopyly-1.4.6/monopyly/credit/statements.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Tools for interacting with the credit statements in the database.
 """
 
 from authanor.database.handler import DatabaseViewHandler
+from dateutil.relativedelta import relativedelta
 
 from ..common.utils import get_next_occurrence_of_day
 from ..database.models import (
     CreditAccount,
     CreditCard,
     CreditStatement,
     CreditStatementView,
@@ -132,25 +133,44 @@
             A flag indicating whether a statement should be created
             if it is not found in the database. The default is `False`;
             a statement will not be created, even if no matching
             statement already exists in the database.
 
         Returns
         -------
-        statement : database.models.CreditStatementView
+        statement : database.models.CreditStatement
             The inferred statement entry for the transaction.
         """
         issue_day = card.account.statement_issue_day
         issue_date = get_next_occurrence_of_day(issue_day, transaction_date)
         statement = cls.find_statement(card.id, issue_date)
         if not statement and creation:
             statement = cls.add_statement(card, issue_date)
         return statement
 
     @classmethod
+    @DatabaseViewHandler.view_query
+    def get_prior_statement(cls, statement):
+        """
+        Given a statement, get the immediately preceding statement.
+
+        Parameters
+        ----------
+        statement : database.models.CreditStatement
+            The statement for which to find the preceding statement.
+
+        Returns
+        -------
+        statement : database.models.CreditStatementView
+            The statement immediately preceding the given statement.
+        """
+        issue_date = statement.issue_date + relativedelta(months=-1)
+        return cls.find_statement(statement.card.id, issue_date=issue_date)
+
+    @classmethod
     def add_statement(cls, card, issue_date, due_date=None):
         """Add a statement to the database."""
         if not due_date:
             due_day = card.account.statement_due_day
             due_date = get_next_occurrence_of_day(due_day, issue_date)
         statement_data = {
             "card_id": card.id,
```

### Comparing `monopyly-1.4.5/monopyly/credit/transactions/_transactions.py` & `monopyly-1.4.6/monopyly/credit/transactions/_transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/database/__init__.py` & `monopyly-1.4.6/monopyly/database/__init__.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/database/models.py` & `monopyly-1.4.6/monopyly/database/models.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/database/schema.sql` & `monopyly-1.4.6/monopyly/database/schema.sql`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/database/views.sql` & `monopyly-1.4.6/monopyly/database/views.sql`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/jquery-3.7.0.min.js` & `monopyly-1.4.6/monopyly/static/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/css/style.css` & `monopyly-1.4.6/monopyly/static/css/style.css`

 * *Files 0% similar despite different names*

```diff
@@ -1660,14 +1660,18 @@
   margin: 20px 0;
   font-size: 72pt;
   font-weight: bold;
   letter-spacing: 1px;
   text-align: center;
 }
 
+.details .summary-box .balance .dollar-sign {
+  margin-right: 5px;
+}
+
 .details .summary-box .projected-balance .amount {
   color: var(--moneytree);
   font-weight: 500;
 }
 
 .details .summary-box .projected-balance .amount.negative {
   color: crimson;
```

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-114.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-114.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-120.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-120.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-144.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-144.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-150.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-150.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-152.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-152.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-16.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-16.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-160.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-160.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-180.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-180.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-192.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-192.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-310.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-310.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-32.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-32.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-57.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-57.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-60.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-60.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-64.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-64.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-70.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-70.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-72.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-72.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-76.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-76.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon-96.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon-96.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon.ico` & `monopyly-1.4.6/monopyly/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/favicon/favicon.png` & `monopyly-1.4.6/monopyly/static/favicon/favicon.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/statement.png` & `monopyly-1.4.6/monopyly/static/img/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/about/bank-account-details.png` & `monopyly-1.4.6/monopyly/static/img/about/bank-account-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/about/bank-account-summaries.png` & `monopyly-1.4.6/monopyly/static/img/about/bank-account-summaries.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/about/bank-accounts.png` & `monopyly-1.4.6/monopyly/static/img/about/bank-accounts.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/about/credit-account-details.png` & `monopyly-1.4.6/monopyly/static/img/about/credit-account-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/about/credit-transactions.png` & `monopyly-1.4.6/monopyly/static/img/about/credit-transactions.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/about/homepage-user.png` & `monopyly-1.4.6/monopyly/static/img/about/homepage-user.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/about/homepage.png` & `monopyly-1.4.6/monopyly/static/img/about/homepage.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/about/statement-details.png` & `monopyly-1.4.6/monopyly/static/img/about/statement-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/cards/chase-card.png` & `monopyly-1.4.6/monopyly/static/img/cards/chase-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/cards/discover-card.png` & `monopyly-1.4.6/monopyly/static/img/cards/discover-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/cards/new-card.png` & `monopyly-1.4.6/monopyly/static/img/cards/new-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/cards/template-card.png` & `monopyly-1.4.6/monopyly/static/img/cards/template-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/arrow-down.png` & `monopyly-1.4.6/monopyly/static/img/icons/arrow-down.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/arrow-left.png` & `monopyly-1.4.6/monopyly/static/img/icons/arrow-left.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/arrow-up.png` & `monopyly-1.4.6/monopyly/static/img/icons/arrow-up.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/checkmark.png` & `monopyly-1.4.6/monopyly/static/img/icons/checkmark.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/delete-orange-thick.png` & `monopyly-1.4.6/monopyly/static/img/icons/delete-orange-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/delete-orange.png` & `monopyly-1.4.6/monopyly/static/img/icons/delete-orange.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/delete-thick.png` & `monopyly-1.4.6/monopyly/static/img/icons/delete-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/delete.png` & `monopyly-1.4.6/monopyly/static/img/icons/delete.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/edit.png` & `monopyly-1.4.6/monopyly/static/img/icons/edit.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/link.png` & `monopyly-1.4.6/monopyly/static/img/icons/link.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/minus-thick.png` & `monopyly-1.4.6/monopyly/static/img/icons/minus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/minus.png` & `monopyly-1.4.6/monopyly/static/img/icons/minus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/plus-thick.png` & `monopyly-1.4.6/monopyly/static/img/icons/plus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/plus.png` & `monopyly-1.4.6/monopyly/static/img/icons/plus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/refresh.png` & `monopyly-1.4.6/monopyly/static/img/icons/refresh.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/save.png` & `monopyly-1.4.6/monopyly/static/img/icons/save.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/sort-asc.png` & `monopyly-1.4.6/monopyly/static/img/icons/sort-asc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/sort-desc.png` & `monopyly-1.4.6/monopyly/static/img/icons/sort-desc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/statement-pair.svg` & `monopyly-1.4.6/monopyly/static/img/icons/statement-pair.svg`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/statement.png` & `monopyly-1.4.6/monopyly/static/img/icons/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/statement.svg` & `monopyly-1.4.6/monopyly/static/img/icons/statement.svg`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/img/icons/x-thick.png` & `monopyly-1.4.6/monopyly/static/img/icons/x-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/add-subtransaction.js` & `monopyly-1.4.6/monopyly/static/js/add-subtransaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/add-transfer.js` & `monopyly-1.4.6/monopyly/static/js/add-transfer.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/autocomplete-transaction.js` & `monopyly-1.4.6/monopyly/static/js/autocomplete-transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/bind-tag-actions.js` & `monopyly-1.4.6/monopyly/static/js/bind-tag-actions.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/create-balance-chart.js` & `monopyly-1.4.6/monopyly/static/js/create-balance-chart.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/define-filter.js` & `monopyly-1.4.6/monopyly/static/js/define-filter.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/display-new-account-type-inputs.js` & `monopyly-1.4.6/monopyly/static/js/display-new-account-type-inputs.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/display-new-credit-account-inputs.js` & `monopyly-1.4.6/monopyly/static/js/display-new-credit-account-inputs.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/expand-bank-account.js` & `monopyly-1.4.6/monopyly/static/js/expand-bank-account.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/expand-bank.js` & `monopyly-1.4.6/monopyly/static/js/expand-bank.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/expand-transaction.js` & `monopyly-1.4.6/monopyly/static/js/expand-transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/flip-card.js` & `monopyly-1.4.6/monopyly/static/js/flip-card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/infer-card.js` & `monopyly-1.4.6/monopyly/static/js/infer-card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/infer-statement.js` & `monopyly-1.4.6/monopyly/static/js/infer-statement.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/make-payment.js` & `monopyly-1.4.6/monopyly/static/js/make-payment.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/show-linked-transaction.js` & `monopyly-1.4.6/monopyly/static/js/show-linked-transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/update-account-statement-parameters.js` & `monopyly-1.4.6/monopyly/static/js/update-account-statement-parameters.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/update-bank-name.js` & `monopyly-1.4.6/monopyly/static/js/update-bank-name.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/update-card-status.js` & `monopyly-1.4.6/monopyly/static/js/update-card-status.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/update-statement-parameters.js` & `monopyly-1.4.6/monopyly/static/js/update-statement-parameters.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/update-statements-display.js` & `monopyly-1.4.6/monopyly/static/js/update-statements-display.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/update-transactions-display.js` & `monopyly-1.4.6/monopyly/static/js/update-transactions-display.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/modules/ajax.js` & `monopyly-1.4.6/monopyly/static/js/modules/ajax.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/modules/autocomplete-input.js` & `monopyly-1.4.6/monopyly/static/js/modules/autocomplete-input.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/modules/expand-box-row.js` & `monopyly-1.4.6/monopyly/static/js/modules/expand-box-row.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/modules/expand-transaction.js` & `monopyly-1.4.6/monopyly/static/js/modules/expand-transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/modules/manage-acquisition-form.js` & `monopyly-1.4.6/monopyly/static/js/modules/manage-acquisition-form.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/modules/manage-overlays.js` & `monopyly-1.4.6/monopyly/static/js/modules/manage-overlays.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/modules/manage-subforms.js` & `monopyly-1.4.6/monopyly/static/js/modules/manage-subforms.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/modules/update-database-widget.js` & `monopyly-1.4.6/monopyly/static/js/modules/update-database-widget.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/static/js/modules/update-display-ajax.js` & `monopyly-1.4.6/monopyly/static/js/modules/update-display-ajax.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/index.html` & `monopyly-1.4.6/monopyly/templates/index.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/layout.html` & `monopyly-1.4.6/monopyly/templates/layout.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/profile.html` & `monopyly-1.4.6/monopyly/templates/profile.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/story.html` & `monopyly-1.4.6/monopyly/templates/story.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/account_page.html` & `monopyly-1.4.6/monopyly/templates/banking/account_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/account_summaries.html` & `monopyly-1.4.6/monopyly/templates/banking/account_summaries.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/account_summaries_page.html` & `monopyly-1.4.6/monopyly/templates/banking/account_summaries_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/account_summary.html` & `monopyly-1.4.6/monopyly/templates/banking/account_summary.html`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   </div>
 
   <div class="title">
     {{ account.account_type.type_common_name.upper() }}
   </div>
 
   <div class="balance">
-    <div>$</div>
+    <div class="dollar-sign">$</div>
     <div>{{ account.balance|currency }}</div>
   </div>
 
   {% if account.balance != account.projected_balance %}
     <div class="projected-balance subtitle">
       <span>Projected balance: </span>
       <span class="amount{{ ' negative' if account.projected_balance < 0 }}">
```

### Comparing `monopyly-1.4.5/monopyly/templates/banking/accounts_page.html` & `monopyly-1.4.6/monopyly/templates/banking/accounts_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/account_form/account_form.html` & `monopyly-1.4.6/monopyly/templates/banking/account_form/account_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/account_form/account_form_page_new.html` & `monopyly-1.4.6/monopyly/templates/banking/account_form/account_form_page_new.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/transaction_form/bank_info_form.html` & `monopyly-1.4.6/monopyly/templates/banking/transaction_form/bank_info_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/transaction_form/transaction_form.html` & `monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<form id="bank-transaction" class="transaction" action="{{ submission_url }}" method="POST" autocomplete="off">
+<form id="bank-transaction" class="transaction" action="{{ submission_url }}" method="post" autocomplete="off">
 
   {{ form.hidden_tag() }}
 
   {% with subform = form.account_info, id_prefix = 'transaction' %}
     {% include 'banking/transaction_form/bank_info_form.html' %}
   {% endwith %}
```

### Comparing `monopyly-1.4.5/monopyly/templates/banking/transaction_form/transaction_form_page.html` & `monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/transactions_table/expanded_row_content.html` & `monopyly-1.4.6/monopyly/templates/banking/transactions_table/expanded_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/banking/transactions_table/transaction_field_titles.html` & `monopyly-1.4.6/monopyly/templates/banking/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/common/transaction_form/subtransaction_subform.html` & `monopyly-1.4.6/monopyly/templates/common/transaction_form/subtransaction_subform.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/common/transactions_table/linked_bank_transaction.html` & `monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_bank_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/common/transactions_table/linked_credit_transaction.html` & `monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_credit_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/common/transactions_table/linked_transaction_overlay.html` & `monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_transaction_overlay.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/common/transactions_table/transaction_expanded.html` & `monopyly-1.4.6/monopyly/templates/common/transactions_table/transaction_expanded.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/common/transactions_table/transactions.html` & `monopyly-1.4.6/monopyly/templates/common/transactions_table/transactions.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/account_page.html` & `monopyly-1.4.6/monopyly/templates/credit/account_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/cards.html` & `monopyly-1.4.6/monopyly/templates/credit/cards.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/statement_page.html` & `monopyly-1.4.6/monopyly/templates/credit/statement_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/statement_summary.html` & `monopyly-1.4.6/monopyly/templates/credit/statement_summary.html`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   </div>
 
   <div id="issue-date" class="title">
     {{ statement.issue_date.strftime('%B %Y') }}
   </div>
 
   <div class="balance">
-    <div>$</div>
+    <div class="dollar-sign">$</div>
     <div>{{ statement.balance|currency }}</div>
   </div>
 
   <div id="payment">
 
     <div id="due">
       <div>DUE</div>
@@ -43,16 +43,16 @@
 
       <form id="pay" action="" method="post">
 
         <div class="form-inputs">
 
           <div class="form-line">
             <div class="dollar-sign">$</div>
-            <input id="pay-amount" type="text" name="pay_amount" value="{{ statement.balance|currency }}" maxlength="8"/>
-            <input id="pay-date" type="text" name="pay_date" value="{{ date_today }}" maxlength="10"/>
+            <input id="pay-amount" type="text" name="pay_amount" value="{{ statement.balance|currency }}" maxlength="8" />
+            <input id="pay-date" type="text" name="pay_date" value="{{ date_today }}" maxlength="10" />
           </div>
 
           <div class="form-line">
             <select id="pay-bank-account" form="pay">
               <optgroup>
                 <option value="0">Select a bank</option>
                 {% for account in bank_accounts %}
```

### Comparing `monopyly-1.4.5/monopyly/templates/credit/statements.html` & `monopyly-1.4.6/monopyly/templates/credit/statements.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/statements_page.html` & `monopyly-1.4.6/monopyly/templates/credit/statements_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/tags_page.html` & `monopyly-1.4.6/monopyly/templates/credit/tags_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/transaction_submission_page.html` & `monopyly-1.4.6/monopyly/templates/credit/transaction_submission_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/transactions_page.html` & `monopyly-1.4.6/monopyly/templates/credit/transactions_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/card_form/card_form.html` & `monopyly-1.4.6/monopyly/templates/credit/card_form/card_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/card_form/card_form_page_new.html` & `monopyly-1.4.6/monopyly/templates/credit/card_form/card_form_page_new.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/card_form/transfer_statement_inquiry.html` & `monopyly-1.4.6/monopyly/templates/credit/card_form/transfer_statement_inquiry.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/card_graphic/card_back.html` & `monopyly-1.4.6/monopyly/templates/credit/card_graphic/card_back.html`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   <div class="digits obscure">▐▐▐▐</div>
   <div class="digits">{{ card.last_four_digits }}</div>
 </div>
 
 <div class="options">
 
   <label class="toggle-switch-gadget" for="card-{{ card.id }}-status">
-    <input id="card-{{ card.id }}-status" data-card-id="{{ card.id }}" type="checkbox" {{ 'checked' if card.active else '' }}/>
+    <input id="card-{{ card.id }}-status" data-card-id="{{ card.id }}" type="checkbox"{{ ' checked' if card.active else '' }} />
 
     <div class="option">
       <div class="text">
         Active
       </div>
       <div class="slider">
         <div class="switch"></div>
```

### Comparing `monopyly-1.4.5/monopyly/templates/credit/card_graphic/card_front.html` & `monopyly-1.4.6/monopyly/templates/credit/card_graphic/card_front.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/tag_tree/subtag_tree.html` & `monopyly-1.4.6/monopyly/templates/credit/tag_tree/subtag_tree.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/transaction_form/transaction_form.html` & `monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/transaction_form/transaction_form_page.html` & `monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/transactions_table/condensed_row_content.html` & `monopyly-1.4.6/monopyly/templates/credit/transactions_table/condensed_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/transactions_table/expanded_row_content.html` & `monopyly-1.4.6/monopyly/templates/credit/transactions_table/expanded_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/monopyly/templates/credit/transactions_table/transaction_field_titles.html` & `monopyly-1.4.6/monopyly/templates/credit/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/.gitignore` & `monopyly-1.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/COPYING` & `monopyly-1.4.6/COPYING`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.5/pyproject.toml` & `monopyly-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
   { name = 'Mitch Negus', email = 'mitchnegus57@gmail.com' },
 ]
 description = 'A homemade personal finance manager.'
 license = { text = 'GNU GPLv3' }
 requires-python = '>=3.10,<3.11'
 dependencies = [
   'authanor==1.1.0',
-  'Flask==3.0.2',
+  'Flask==3.0.3',
   'Flask-WTF==1.2.1',
   'fuisce==1.0.2',
-  'gunicorn==21.2.0',
+  'gunicorn==22.0.0',
   'Markdown==3.6',
   'python-dateutil==2.9.0',
   'rich==13.7.1',
   'SQLAlchemy==2.0.29',
 ]
 keywords = [
   'Finance',
```

### Comparing `monopyly-1.4.5/PKG-INFO` & `monopyly-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monopyly
-Version: 1.4.5
+Version: 1.4.6
 Summary: A homemade personal finance manager.
 Project-URL: Download, https://pypi.org/project/monopyly
 Project-URL: Homepage, http://monopyly.com
 Project-URL: Repository, https://github.com/mitchnegus/monopyly
 Project-URL: Changelog, https://github.com/mitchnegus/monopyly/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Requires-Python: <3.11,>=3.10
 Requires-Dist: authanor==1.1.0
 Requires-Dist: flask-wtf==1.2.1
-Requires-Dist: flask==3.0.2
+Requires-Dist: flask==3.0.3
 Requires-Dist: fuisce==1.0.2
-Requires-Dist: gunicorn==21.2.0
+Requires-Dist: gunicorn==22.0.0
 Requires-Dist: markdown==3.6
 Requires-Dist: python-dateutil==2.9.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: sqlalchemy==2.0.29
 Description-Content-Type: text/markdown
 
 <div id="header">
```

