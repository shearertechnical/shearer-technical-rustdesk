# Code signing policy

## Project

Shearer Technical Remote Support is an open-source, self-hosted remote-support
client based on RustDesk. The authoritative source, release history, and build
workflow are maintained in the
[shearertechnical/shearer-technical-rustdesk](https://github.com/shearertechnical/shearer-technical-rustdesk)
repository.

The project is licensed under the GNU Affero General Public License v3.0. The
project does not use commercial dual licensing or include a proprietary client
component maintained by this project.

## Signing status

The project is seeking SignPath Foundation code signing. Until an application
is approved and a release expressly identifies a signature, no release should
be represented as signed by SignPath Foundation.

For releases signed through the Foundation, the release page will state:

> Free code signing provided by [SignPath.io](https://about.signpath.io/),
> certificate by [SignPath Foundation](https://signpath.org/).

## Roles

- **Committer and reviewer:** the repository administrator,
  [@bleachbezel](https://github.com/bleachbezel), maintains the project and
  reviews changes before they are released.
- **Approver:** the repository administrator manually approves each signing request
  after confirming the release commit, artifact name, version, and checksum.

Contributions from anyone without repository write access must be reviewed
before merge. All project members must use multi-factor authentication for
GitHub and SignPath access.

## Release and signing process

1. A release is created from a public commit in this repository.
2. GitHub Actions builds the Windows artifact using
   [the documented workflow](../.github/workflows/shearer-windows.yml).
3. The approver verifies the artifact version, source commit, and SHA-256
   checksum before approving a signing request.
4. The signed executable, its SHA-256 checksum, source commit, and license are
   published together in the GitHub Release.
5. A signing request is manually approved for every release; no unattended
   signing approval is used.

## Security and privacy

Only artifacts produced from this repository's public source and build scripts
may be signed. Project releases must retain the product name and version
defined by the build. The client is for authorized remote-support sessions;
unauthorized access, surveillance, or privacy violations are prohibited.

See the [Privacy notice](PRIVACY.md) for information about networked remote
support sessions.
