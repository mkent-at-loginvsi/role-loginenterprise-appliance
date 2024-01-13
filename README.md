# role-loginenterprise-appliance

role-loginenterprise-appliance is an ansible role

This Ansible role installs Login VSI's flagship platform - Login Enterprise - from an existing release (the build of the release file is not part of this role) on existing linux operating systems. The tasks in this role are support remote or local ansible execution, support check mode, are idempotent and have testing built in.

# Installation
This role is only available via github and is not published in ansible-galaxy's site, however the project includes a requirements.yml which allows you to use ansible-galaxy for installation locally:

ansible-galaxy install -r requirements.yml --force
Starting galaxy role install process
- changing role role-loginenterprise-appliance from main to main
- extracting role-loginenterprise-appliance to /Users/<user>/.ansible/roles/role-loginenterprise-appliance
- role-loginenterprise-appliance (main) was installed successfully

You may also download the repo zip extract the and include it into your deployment that way as well.

# OS Support for this role
-Debian 10

# Why a separate installer?
There are occations when customers need support for operating systems, cloud instance types, tooling etc that are not condusive or ameiable to either an appliance based prodcut or a Debian base OS. This installer is designed to provide an option in those scenarios.

# Why ansible?
Deploying Login Enterprise via a configuration manager was used to support larger automation efforts and provide idempotency. Ansible was chosen for those same reasons, automation and idempotency, and in the mainainer's view a clear DSL and metaphor tha does not break down the deeper you go (just an opinion). Ansible provides a robust, feature rich set of capabilties and is easy to read and maintain.

# How do I get help?
Contact the project maintainer for any questions or issues you may have.

# How can I contribute?
As this is a new effort, please contact the project mainainers if you wish to contribute. We are adding some flexibility to the installer to allow for collaboration and contribution, its not quite there just yet.