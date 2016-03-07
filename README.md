# Description
This project is primarily used for installing development components in a consistent way for future macbook provisions

# Pre-requisites
 - execute bootstrap.sh
 - ensure that you export AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY before running the ansible playbook to correctly setup aws credentials in your user folder.


# Usage

From the root of the project:

ansible-playbook -i hosts playbook.yml

## Optional
If you want to ensure that Homebrew is reinstalled then run with the additional parameters:

ansible-playbook -i hosts playbook.yml --extra-vars "reinstall_homebrew=True" 