# RTP Troubleshooting Flow

One of the biggest mistakes in VoIP troubleshooting is starting with random packet captures.

A better approach is to ask the right questions in the right order.

## Troubleshooting sequence

1. Is RTP leaving your endpoint?
2. Is RTP arriving at the remote side?
3. Does the SDP contain correct media IP and ports?
4. Are both endpoints using compatible codecs?
5. Is RTP flowing in both directions?

## Common causes

- NAT
- Firewall
- Wrong SDP
- Codec mismatch
- Incorrect RTP routing
- Asymmetric routing

## Production lesson

SIP establishes the session.

RTP carries the conversation.

A successful SIP call without working RTP is still a failed call.
