# The Most Complex Problem Was One Route

During a FreePBX 15 to FreePBX 17 migration, the system appeared to have a telephony problem.

Calls were failing.

At first glance, it looked like:

- SIP trunk issue
- provider issue
- FreePBX configuration problem

The migration itself had completed successfully.

After troubleshooting SIP signaling, routing and PBX configuration, the actual cause turned out to be much simpler.

A static route from the old server was missing on the new one.

One line in the routing table prevented the PBX from reaching the provider network.

After restoring the route, inbound and outbound calling returned to normal.

Lesson learned:

When troubleshooting migrations, compare the entire environment.

Not only the PBX configuration.

Sometimes the most complex outage is caused by the smallest missing configuration.
