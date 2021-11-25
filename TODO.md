Tasks:

[ ] Configure authentication credentials in .zshrc: COMPOSER_AUTH, GITHUB_TOKEN, BLACKFIRE_*, APIGEE_EDGE_* 
[ ] Add VS Codium (with plugins?)?
[ ] Add hardening to the defult SSH config, eg.: https://galaxy.ansible.com/geerlingguy/security

Other:

[ ] If this gets picked up by others, make this more configurable because others might customize my default set up and skip tools that they do not need
[ ] ^ related to this, decide if it worth using roles (without publishing them, are they useful?) or rather switch to smaller, scoped tasks and include them in the playbook. There are issues with roles: https://github.com/ansible/ansible/issues/62847 and cross role dependencies only work if 3rd party roles are stored in `roles` folder.
