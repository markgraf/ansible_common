# ansible_common

One playbook to run everything.

This will require careful setup of your inventory and roles, though.
For each hostgroup a host is in, this playbook will run a role named like the group against the host --if the role exists.

This is useful if you have groups and meta-roles like "database", "webserver" and the like
which change their behaviour depending on variables from group_vars and host_vars.

This could be done with a role as well, putting the common_unconditional_roles into the dependencies.
