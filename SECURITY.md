# **Security Release Process** #
The FATE community follows the disclosure and response policies formulated in FATE Security to ensure that we address key issues responsibly.

## Security Response Committee (SRC) ##
The Security Response Committee (SRC) is composed of the security director, relevant technical personnel, and operation personnel. It organizes the response to all security issues, including internal communication and external disclosure, and organizes relevant personnel to complete the process.

## Supported Versions ##
The community maintains the LTS release and the latest 2 major releases. Each major release only maintains the latest minor version.

## Reporting a Vulnerability ##
We thank all community members and users who report vulnerabilities to the FATE open-source community. The FATE SRC will thoroughly investigate all reported vulnerabilities.
### Private Disclosure Process ###
All confirmed or suspected security vulnerabilities shall be reported privately to the FATE SRC to minimize attacks on FATE's current users before remediation. If you wish to notify the SRC of a vulnerability, you may send an email to [FATE-security@groups.io](https://groups.io/g/FATE-security) so that we can respond and eliminate the issue as soon as possible.
Important: To protect the user community, do not post security vulnerabilities on GitHub or other public media.
**Recommended Vulnerability Reporting Format**
Please include the following information in the body of the email, along with a descriptive subject line.
- Basic identity information, such as your name and employer.
- Specific steps for vulnerability recurrence (necessary scripts, screenshots, and compressed packet captures are all helpful).
- Describe the impact of the vulnerability on FATE so that the FATE security team can reproduce the vulnerability.
- Describe how this vulnerability affects FATE's usage and provide an estimate of the attack surface, if any.
- List other projects or dependencies used with FATE to produce the vulnerability.
**Security Vulnerability Response**
After receiving your email, the FATE SRC will contact you within 3 working days and start to investigate the vulnerability, including the results of vulnerability identification and analysis, fixing plan, and any potential workarounds implemented during this period. Any vulnerability information shared with the SRC will remain within the FATE project and will not be disseminated to other projects unless it is necessary to fix the issue.
### When Should I Report a Vulnerability ###
- You think you have found a potential security vulnerability in FATE.
- You suspect that there is a potential vulnerability, but you are not sure if it affects FATE.
- You know or suspect that a vulnerability has been found in another project on which FATE relies (for projects that have their own vulnerability reporting and disclosure procedure, please report vulnerabilities to the project).
### When Should I NOT Report a Vulnerability? ###
- You need help turning FATE components for security.
- You need help applying security-related updates.
- Your problem is unrelated to security.

## Patch, Release, and Disclosure ##
After receiving the vulnerability report, the FATE SRC will respond to the vulnerability as follows:
1. Normally, the SRC will contact you within 3 working days to investigate the vulnerability, confirm whether it is true, and determine its impact and severity;
- If this problem is not a vulnerability, SRC will provide the specific reason for rejection and reply to you;
- If the security vulnerability is confirmed, SRC will reply to you after completing the next step, including the results of vulnerability identification and analysis, patching plan, and any potential workarounds implemented during this period;
2. After confirmation, SRC will formulate the vulnerability fixing method and schedule, develop a mitigation plan, and communicate with the community, including determining the mitigation steps that the affected users can take to protect themselves until the release of a patch;
3. Fix and test the vulnerability and prepare for the release of a patch;
4. A corresponding minor version will be released in all supported versions (namely the latest two major versions and the LTS version of the project) to fix the vulnerability. Once the patched FATE version is released, SRC will follow the public disclosure process.
5. Public disclosure process: SRC will issue a public announcement to the FATE community through GitHub website to guide FATE users to learn about the vulnerability and obtain a patched version. SRC will also announce the mitigation measures that users can take until they can apply patches to their FATE services.

## Mailing list ##
Security issues can be reported to the FATE SRC by sending email to [FATE-security@groups.io](https://groups.io/g/FATE-security). The FATE SRC will discuss security issues and patching methods privately via this email group before disclosure.

## Limitation of Liability ##
The FATE community pays high attention to the vulnerabilities that impair the confidentiality and integrity of user data. The FATE community takes all reported, potential, and suspected vulnerabilities seriously and will investigate them promptly.
The copyright owner of FATE/FederatedAI (the "Work") and each contributor (collectively, the "Licensor") openly grants a license to any individual or legal entity (the "Licensee"), but Licensee's acceptance of the license is also subject to [DISCLAIMER](./DISCLAIMER.md)) and the "Limitation of Liability" clause herein.