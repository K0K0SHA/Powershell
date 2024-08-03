I recommend pasting these one-liners into your terminal or your code instead of running them on their own. You can always change them into scripts by changing the .txt extension to a .ps1 extension.

TODO CATALOG:
[X] Get Execution Policy
Get-ExecutionPolicy
[ ] Set Execution Policy to allow remote signed scripts for the duration of the session
 Set-ExecutionPolicy RemoteSigned -Scope Process
[X] Change permission for an SSH private key to work properly, equivalent to 0600 on Linux
icacls "E:\bandit\overthewire_bandit_solutions-main\bandit17.privatekey" /inheritance:r /grant "your_username_that_you_get_from_whoami:R"
