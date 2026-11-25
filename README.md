# PortGuard — IEEE 802.1X Interactive Lab

An offline-friendly educational web simulator for Data Communication, topic 32. Built with plain HTML, CSS and JavaScript, without dependencies or external APIs.

## Run
Open `index.html` in a browser. No installation, server or credentials needed.

## Classroom demo (about 75 seconds)
1. Test normal data before authentication: BLOCKED.
2. Select Authorized student, then Auto play. Watch EAPOL and RADIUS exchanges. Test normal data: PERMITTED.
3. Select Unknown device, then Auto play. Test normal data: BLOCKED.
4. Ask whether 802.1X itself encrypts ordinary data. Answer: no.

Presentation mode hides the extra quiz and references for a focused projector view. Next message steps through the protocol manually.

## Publish via GitHub Pages
Create a repository named `portguard-8021x`, upload `index.html`, `.nojekyll` and this README at the repository root, then Settings > Pages > Deploy from a branch > main / (root) > Save. Use the exact link displayed by GitHub Pages after a successful deployment. The site is static and stores no personal information.

## Scope
All messages and outcomes are simulated. Intermediate EAP method exchanges are omitted; EAPOL-Start is optional in real deployments. The program is not a real RADIUS server, packet capture, encryption tool or production security control. Actual authentication depends on the configured EAP method, authorization policy and network environment.

## References
- William Stallings, *Network Security Essentials: Applications and Standards*, 6th ed., section 5.3.
- [Cisco IEEE 802.1X documentation](https://www.cisco.com/c/en/us/td/docs/ios-xml/ios/sec_usr_8021x/configuration/xe-3e/sec-usr-8021x-xe-3e-book/config-ieee-802x-pba.html)

AI assistance: ChatGPT (OpenAI), for drafting and implementation.
