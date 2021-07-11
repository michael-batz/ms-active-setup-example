# ms-active-setup-example
Small example for Microsoft Active Setup

## setup

* execute scripts/active-setup.reg to install the Active Setup registry entry
* place scripts/test.reg under C:\test.reg

## run the example

After log in of an existing or new user, the command defined in scripts/active-setup.reg will be executed. It will 
import C:\test.reg for the current user in HKEY\_CURRENT\_USER and create a demo registry key in HKCU\Software\ActiveSetup.
This only happens on the first login of the user after the scripts/active-setup.reg key was set.

## background
For background information, have a look at one of the following articles:
* https://helgeklein.com/blog/2010/04/active-setup-explained/
* https://www.itninja.com/blog/view/appdeploy-articles-activesetup
