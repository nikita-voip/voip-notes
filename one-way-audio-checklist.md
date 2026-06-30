# One Way Audio Troubleshooting Checklist

## Symptoms

- Caller hears remote side only
- One-way audio after answer
- Audio disappears after transfer

## Step 1. Check RTP Flow

Verify RTP packets in both directions.

Tools:
- sngrep
- tcpdump
- Wireshark

## Step 2. Check NAT

Common issues:

- wrong external address
- symmetric NAT
- missing RTP ports

## Step 3. Inspect SDP

Verify:

- c= address
- media ports
- codec negotiation

## Step 4. Check Firewall

Allow RTP range and SIP signaling.

## Step 5. Verify SBC Behavior

Check media anchoring and RTP proxy settings.
