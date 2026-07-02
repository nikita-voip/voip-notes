# Green LEDs Don't Mean Everything Works

One of the most misleading situations in telephony is seeing healthy E1 indicators while calls still fail.

Typical symptoms:

- E1 interface is up
- No alarms
- Synchronization is present
- LEDs are green

Everything appears healthy.

Yet traffic does not pass.

In production environments, physical layer status only confirms that the circuit exists.

It does not guarantee correct signaling, routing or service operation.

Whenever an E1 problem is reported, I verify:

- Layer 1
- Layer 2
- Signaling status
- Routing
- Call processing

Green LEDs are useful.

But they are only the beginning of troubleshooting.
