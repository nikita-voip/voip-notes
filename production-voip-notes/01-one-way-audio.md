# One-Way Audio Is Rarely Just a VoIP Problem

One-way audio is one of the most common problems in VoIP troubleshooting.

The SIP part may look perfect:

- INVITE is sent
- 200 OK is received
- ACK is completed
- the call is established

But the media path still fails.

In production, one-way audio is often caused by:

- NAT issues
- wrong RTP IP in SDP
- firewall rules
- missing routes
- asymmetric traffic
- incorrect SBC or PBX network settings

The key lesson:

SIP tells you that the call exists.  
RTP tells you if people can actually talk.

A successful call is not just a connected call.  
A successful call is when both sides can clearly hear each other.
