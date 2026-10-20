# Courier

**Free, self-hosted, one-way messaging for schools.**

Courier lets a school's IT team or office write a short notice, choose who should see it, check exactly how it will look,
send it, and then see how far it got. The notice appears on the Windows computers you choose, through the RSJ Agent. It runs
on a Windows Server in your school, and nothing about your notices leaves your network.

**Website:** [courier.rsjsoftware.com](https://courier.rsjsoftware.com)

Courier is free. There is no licence key, no paid edition and no limit on the number of computers.

---

## What it does

- **Write, preview, send.** A title, a message and an expiry time. The preview shows the notice as the computer will show it,
  who it reaches in words, when it closes, and a warning for anything that might go wrong first (a computer that is off, a
  computer without the Courier module, a person no computer has reported signed in yet).
- **Computers or people.** Send to the computers you tick, or to people by username or by Active Directory group.
- **Honest delivery reports.** Each copy of a notice is Waiting, Received, Displayed, Acknowledged, Expired or Failed.
  Displayed is never "read", and Expired is never "acknowledged". Results can be downloaded as a CSV file.
- **A notice closes when it expires.** After that it is not handed out again and open copies are closed.
- **History you control.** Every notice is kept for the period the school chooses, then deleted.
- **Local accounts.** Administrators and senders, each with their own sign-in. Courier's accounts do not sign in to any other
  product.
- **Templates, your school's name and logo.** Reuse wording you send often. The name and logo show in the console and in the
  preview.
- **Built on the RSJ Agent.** The same agent that other RSJ products use shows the notice on each computer. Courier adds a
  small module to it; it does not replace or change anything else the agent does.

## Where it is today

Courier is new. Please read this before relying on it.

- **Seen working on real computers (a lab server and PC, October 2026):** a notice sent to a computer and to a person, shown on screen and acknowledged, each step recorded in the console; a notice that waits while nobody is signed in, and one that expires while the computer is off; Active Directory groups read from a real domain; the server and the computer restarting; upgrading, uninstalling and reinstalling with the data kept.
- **Not yet proven on real machines:** one person signed in on two computers, signing out and another person signing in, a locked or signed-out screen, and automatic updates.
- **Known issue:** a notice waiting for someone to sign in may not appear when they do. Send it again. It's being fixed in the RSJ Agent.
- **The school name and logo are not shown on the computers' notice window yet**, only in the console and the preview.
- **Not for emergencies.** Courier makes no promise that a notice reaches or interrupts anyone in time. Do not rely on it for
  a lockdown, a fire alarm or anything where a missed message is dangerous.

It has only been tried on a small lab so far, so start with a few computers and tell us how it goes.

## Why self-hosted

- **Your messages stay on your network.** There is no cloud service holding your notices, your staff list or your history.
- **Nothing reported.** Courier sends nothing about you to RSJ Software. The only time it contacts the internet is to check for
  and download updates, and only when you ask it to or turn automatic updates on.
- **Reads, never writes, your directory.** If you let Courier look up Active Directory groups, it uses an account that can
  only read, and it changes nothing in the directory.

---

## Getting started

1. **Download** `CourierSetup.exe` from the [Releases](../../releases) page. It includes everything it needs; there is no
   Python or other software to install first.
2. **Install** it on a Windows Server that stays on, then choose **Open Console** from the Start menu on that server and create
   the first administrator account.
3. **Put the RSJ Agent on your computers**, enrol each one with Courier, and enable the Courier module for them from the
   console. The wiki's [Getting Started](../../wiki/Getting-Started) page walks through every step, including your first notice.

The [wiki](../../wiki) also covers [Sending a notice](../../wiki/Sending-a-Notice), [Audiences](../../wiki/Audiences) and
[Troubleshooting](../../wiki/Troubleshooting).

## Support

- **Questions and ideas:** RSJ Software's shared [Discussions](https://github.com/orgs/rsjsoftwareltd/discussions),
  opening soon.
- **Bugs:** [Issues](../../issues) on this repository.

There is no helpdesk with opening hours. Courier is built to be installed and run by a school's own IT.

---

## About

Courier is built by **RSJ Software** -- a school IT professional who built it for the school IT community.

- Website: [rsjsoftware.com](https://rsjsoftware.com)
- Reporting a security issue: see [SECURITY.md](SECURITY.md)

## Licence

Copyright RSJ Software Ltd. All rights reserved.

This repository is provided for transparency, release distribution and community support. No licence is granted for reuse,
modification or redistribution of the source code.
