# Security Policy

## Supported versions

Courier is a self-hosted, single-release-line product -- there is no long-term-support branch. Security fixes are made
against the current release line only. Please always run the latest published release (the version is shown in the console
under Settings, About) before reporting an issue, in case it is already fixed.

## Reporting a vulnerability

If you believe you have found a security vulnerability in Courier (the server application, the Courier module for the RSJ
Agent, or the installer), please report it privately rather than opening a public GitHub issue or discussing it publicly.

**Email: security@rsjsoftware.com**

Please include as much of the following as you can:

- A description of the vulnerability and its potential impact.
- Steps to reproduce, or a proof of concept.
- The affected version (Settings, About).
- Any suggested mitigation, if you have one.

### What to expect

- We aim to acknowledge your report within **3 working days**.
- We will keep you informed as we investigate and work on a fix.
- We ask that you give us a reasonable window to develop and release a fix before any public disclosure, and that you avoid
  accessing, modifying, or exfiltrating data beyond what is strictly necessary to demonstrate the issue.
- Good-faith security research conducted under this policy will not result in legal action from us.

### Scope

In scope: the Courier server application, the Courier module that runs on the RSJ Agent, and the Windows installer. A problem
you find in the RSJ Agent itself is also welcome at the same address.

Out of scope: third-party services Courier works with (for example Active Directory and Windows itself) and individual
school infrastructure -- please report those to the relevant vendor.

### Bug bounty

We do not currently operate a paid bug bounty programme. We are genuinely grateful for responsible disclosures and will credit
reporters (with permission) in release notes where appropriate, but we want to be upfront that there is no monetary reward on
offer at this time, so there is no unstated expectation either way.

---

RSJ Software Ltd -- Courier is a self-hosted school messaging product. Notices stay on the school's own server.
