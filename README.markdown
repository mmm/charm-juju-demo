
# juju demo

Use this charm to deploy juju local containers onto other providers.
I.e., an LXC container running in either an openstack or ec2 instance.

There's not much to it... just deploy, then log in.

    $ juju bootstrap
    $ charm get mysql charms/oneiric/mysql
    $ juju deploy --repository ~/charms local:mysql mydb


For charm schools, spread it out and create / hand out passwords
for the 'ubuntu' user on each instance.
That should be a config option.

Maybe pre-cache charms and dependent packages?

