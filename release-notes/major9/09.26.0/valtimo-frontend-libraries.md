# Frontend libraries 5.15.0 (RC)

## New Features

The following features were added:

* **Override default case list tabs**

  A new (optional) environment property, `visibleDossierListTabs` is introduced to change the visibility of the default tabs in the `valtimo-dossier-list` component.

  The new property is an array that includes the tabs that need to be visible on the page. The collection can consist of the following values: `DossierListTab.MINE`, `DossierListTab.OPEN`, and `DossierListTab.ALL`.

  Only cases assigned to the current user are displayed when the option 'my cases' are selected. When selecting the 'unassigned cases'  tab, only the cases with no assignee set are shown.

  With this new property, you can either hide specific tabs that are visible by default or change their default order.


* **Case definition setting enables an option to set an assignee to a case on case management**

  Added a new setting on the case management page to indicate that a case type can have an assignee.

  More information on this case setting can be found [here](/using-valtimo/document/assigning-a-user.md#how-to-configure-cases-to-be-assignable).

* **Number of open cases now shown in menu**

  The number of open/unassigned cases is now shown in the Valtimo menu. When the number of open cases changes, the
  number in the menu is automatically updated without reloading the page.

  ![Open case count](img/open-case-count.png)

* **New tab 'list columns' on case management page**

  Added a new separate tab on case management page to configure case list columns.

## Bugfixes

The following bugs were fixed:

* **Total number of cases found in case list**

  In the badge on the case list the total number of items on the page was shown instead of the actual number of cases found based on the search criteria.

## Breaking changes

No breaking changes.

## Deprecations

No new deprecations.

## Known issues

No new known issues.
