# SIP Call Flow Reference

A basic SIP call flow is simple on paper.

Each SIP message answers a different troubleshooting question.

## Messages

INVITE

Was the call initiated?

100 Trying

Did the next system accept processing?

180 Ringing

Did the destination start alerting?

200 OK

Was the call answered?

ACK

Was the dialog confirmed?

RTP

Is audio actually flowing?

BYE

Was the session closed correctly?

200 OK

Was the termination confirmed?

## Production lesson

SIP creates the session.

RTP carries the media.

Never stop troubleshooting after seeing 200 OK.
