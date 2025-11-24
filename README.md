# Autologon

## Introduction

Autologon makes it easy to set up Windows’ built-in automatic sign-in capability. Instead of requiring users to type their username and password during startup, Windows simply uses the credentials configured through Autologon—stored in the Registry in an encrypted format—to automatically log in the selected account.

Using Autologon is uncomplicated: run the BAT file, specify the desired account, and click **Enable**. After that, each time the system starts, Windows will attempt to sign in the configured user at the console using the saved credentials. Be aware that Autologon does not verify whether those credentials are correct or whether the account is permitted to log on locally.

Beyond basic configuration, Autologon is useful in environments where systems must start without user input—such as kiosks, service workstations, automated testing setups, or virtual machines that require unattended startup. Since it leverages native Windows authentication instead of adding extra services, it introduces almost no overhead and doesn’t interfere with existing security mechanisms.

Administrators often rely on Autologon during deployment or imaging processes to streamline initial configuration, run provisioning scripts on first boot, or simplify domain-join steps. Still, it’s important to consider the security aspects: protect physical access to the device and limit admin rights to prevent unauthorized recovery of stored credentials.
