# Privacy notice

**Effective date:** November 20, 2026

This notice applies to the Shearer Technical Remote Support client distributed
from this repository. It describes the project-maintainer's intended handling
of information through the client; it does not replace a customer's own
privacy, security, or acceptable-use policies.

## What the client does

The client is used to establish authorized remote-support sessions. To set up a
session, it communicates with the self-hosted rendezvous and relay service
configured in the public source code. During a session, information selected or
enabled by the people operating the two endpoints can be transmitted to the
remote peer. This can include screen images, keyboard and mouse input, audio,
clipboard content, and files transferred through the client.

## How information is handled

- A remote session is initiated only after a person operating the client uses
  its connection and authorization controls.
- The project does not add advertising or analytics code to the client.
- Support-session data is not intentionally sent to third-party analytics or
  advertising services by this project.
- Local configuration and diagnostic logs may be stored on the device as part
  of normal client operation. Device owners and administrators control access
  to those devices and logs.

## Your choices

Do not accept or continue a remote-support session unless you recognize and
trust the other party. Disable session features you do not want to use, such as
file transfer or clipboard sharing, where those controls are available. You
may uninstall the client using the operating system's normal application
removal process.

## Contact and source code

Questions about this client or this notice can be raised through the
[project's GitHub issue tracker](https://github.com/shearertechnical/shearer-technical-rustdesk/issues).
The full source code and build configuration are available in the
[project repository](https://github.com/shearertechnical/shearer-technical-rustdesk).
