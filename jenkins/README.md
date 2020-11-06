## Playbooks for installing and configuring Jenkins on a Debian/Ubuntu host

Note that the `configure` playbook installs Jenkins plugins via the `initialAdminPassword`, without trying to bypass the Setup Wizard.  
This will kind of mess up the [InstallState](https://javadoc.jenkins-ci.org/jenkins/install/InstallState.html), but you just have to:

1. Go to **Manage Jenkins** -> **Configure System** and set the **Jenkins URL** (or just click Apply)
2. Create a new user from **Manage Jenkins** -> **Manage Users** -> **Create User**
