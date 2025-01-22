<h1>Analysis Response</h1>

<h2>Description</h2>

<p>Many organizations marginalize the management of the security of their infrastructure in hopes that they will not be the target of cyberattacks. However, cyberattacks happen frequently and tend to become more sophisticated over time. In reality, every organization is a likely target of malicious actors. These attacks result in a range of impacts on an organization and its core business and could significantly interrupt operations.</p>

<p>To be proactive, organizations need to have structures, processes, and plans in place to counter and respond to potential attacks and to deal with the consequences of successful attacks. A suitable security management plan and well-defined security goals that support the overall goals of the organization can ensure a reasonable level of business continuity, even in the case of security incidents.</p>

<p>In any organization, the individuals on the IT staff must work together to support the security goals of the organization. These individuals play significant roles in detecting and preventing security incidents before they occur. In the case of successful attacks, security management professionals are tasked with acting quickly to mitigate the attack’s effects. </p>

In this project, we will refer to the attached “Case Study,” which contains details regarding a security incident at a small non-governmental organization (NGO). In part I of this project, I have analyzed the security incident and provided specific examples and details from the case study to support your risk assessment. In part II, I have created a plan to effectively address the aftermath of the incident and managed the NGO’s ongoing security risks.</p>

<h2>Part I: Incident Analysis and Response</h2>

<h2>Why the Attack Was Successful</h2>

<p>The attack on Azumer Water’s infrastructure was largely successful because of several overlooked security vulnerabilities in the organization’s environment. First, John, the volunteer coordinator, clicked on a suspicious link in a phishing email claiming to offer discounted water pallets. This action immediately exposed the organization to malicious code or external websites that steal data. Because there was no consistent security training, John and other employees were not adequately equipped to recognize phishing attempts or know how to handle suspicious emails. Additionally, Azumer Water relied on an enterprise firewall whose configuration was never completed, which effectively left the network unprotected against potentially harmful traffic.</p>

<p>The organization’s wireless network also used the outdated Wired Equivalent Privacy (WEP) protocol. WEP encryption has been proven weak for many years and is relatively easy for attackers to bypass or crack. Moreover, Azumer Water’s password policy was poorly enforced, leading to employees reusing the same credentials for long periods without mandatory updates. Finally, the lack of thorough data backup processes meant no reliable secondary copy of the volunteer database. Despite some employees occasionally copying the database to USB drives, these practices were unregulated and inconsistent. These gaps combined make it easy for attackers (in this case, potentially the hacktivist group Elecktores) to carry out a damaging security breach.</p>

<h2>How the Confidentiality, Integrity, and Availability Were Compromised</h2>

<p>Using the <b>NIST Special Publication 800-53 Revision 5 (2020)</b> framework as a guide, we can see clear evidence of compromises to Azumer Water’s confidentiality, integrity, and availability.</p>

<p><b>Confidentiality</b> was compromised when unauthorized individuals likely accessed the organization’s systems or misled volunteers into disclosing information. Under NIST 800-53, controls such as AC-2 (Account Management) and AC-3 (Access Enforcement) require strict oversight of user accounts and permissions. However, because Azumer Water did not enforce a strong password policy or employee security training, attackers could exploit these weaknesses and access data that should have remained private.</p>

<p><b>Integrity</b> was compromised when the volunteer database went missing on Monday morning. From the case study, it is clear that attackers either deleted, relocated, or altered the database files. NIST 800-53 advocates for data integrity checks (SI-7) and comprehensive backup and recovery strategies (CP-9). If Azumer Water had possessed rigorous integrity checks and a consistent backup schedule, the suspicious or unauthorized alterations to the database could have been quickly detected and reversed.</p>

<p><b>Availability</b> was significantly impacted because the volunteer database was not accessible, and day-to-day operations were disrupted. Volunteers were confused and upset, as evidenced by the 71 angry emails John received. The combination of lost data and volunteer mistrust highlights how availability issues can directly affect an organization’s ability to fulfill its mission.</p>

<h2>Federal Regulation Violated</h2>

<p>Given that Azumer Water partners with FEMA (a federal agency) and handles personally identifiable information (PII), such as the last four digits of volunteers’ Social Security numbers, the organization must comply with the <b>Federal Information Security Modernization Act (FISMA)</b>. Under FISMA, any federal agency or affiliated organization must implement comprehensive security measures, conduct periodic risk assessments, and establish formal incident response and data protection procedures.</p>

<p>Azumer Water violated FISMA in this case by not properly safeguarding volunteer data and failing to maintain adequate security controls. The organization did not enforce strong password standards, did not complete firewall configurations, nor did it have a consistent backup plan. For instance, the CEO knew the network was vulnerable but ignored Pruhart Tech’s recommendation for a vulnerability assessment. Furthermore, storing PII on a single machine without routine backups or encryption represents a failure to protect sensitive volunteer records in a manner consistent with FISMA guidelines.</p>

<h2>Immediate Steps to Mitigate Impact</h2>

<p>To reduce the harm caused by this incident, Azumer Water should take several immediate steps. First, they should <b>isolate the affected systems</b>. Specifically, any computers or servers suspected to be compromised—especially the machine where the volunteer database was kept—must be taken offline. This helps to prevent attackers from moving laterally across the network or inflicting further damage.</p>

<p>Second, the organization should <b>reset all passwords</b> and enforce a more rigorous password policy. Since some employees have been using the same credentials for years, this step will limit any compromised accounts from remaining a backdoor for attackers. Next, Azumer Water should <b>work with Pruhart Tech to configure and patch the firewall</b>. Since the firewall setup was initially deferred, completing it is essential to protect the network from unauthorized incoming and outgoing traffic.</p>

<p>Additionally, <b>notifying volunteers and relevant stakeholders is critical</b>. Azumer Water should clarify that any recent donation requests via suspicious emails are fraudulent, thus preventing further confusion and potential financial loss for volunteers. A short-term communication plan should be established to reassure volunteers and ensure their concerns are addressed. This approach both mitigates harm and begins to restore trust.</p>

<h2>Benefits of Having an Incident Response Plan</h2>

<p>An incident response plan is a structured and pre-documented process that details what steps to take during a security breach. If Azumer Water had such a plan, they could have contained the incident more quickly and with less confusion. Employees would know exactly which systems to disconnect, which logs to review, and how to communicate with volunteers and officials. The plan would establish clear roles so John or any other staff member could quickly inform the designated incident response leader.</p>

<p>Moreover, having an incident response plan in place helps reduce downtime by providing instructions on preserving evidence, conducting forensic analysis, and restoring normal operations. In this scenario, the missing volunteer database could have been recovered or restored from backups if the plan mandated frequent, regulated backups and emergency recovery procedures. Azumer Water would have also been better prepared to maintain trust with volunteers and FEMA by following a documented plan. Thus, an incident response plan directly supports the organization’s commitment to protecting the confidentiality, integrity, and availability of information.</p>

<h2>Part II: Risk Assessment and Management</h2>

<h2>Two Processes to Increase Information Assurance and Ensure Compliance</h2>

<p>Two key processes can be adopted immediately to boost Azumer Water’s information assurance levels and help comply with FISMA:</p>

1. **Regular Security Assessments and Audits:** This involves scheduling periodic vulnerability scans, penetration tests, and compliance audits. Azumer Water can identify weaknesses in its servers, wireless network, and open-source software through these assessments. The organization will continuously align with FISMA’s risk management requirements by systematically checking for vulnerabilities and addressing them.
2. **Implementing Formalized Backup and Recovery Procedures:** Establishing routine, automated backups that are stored securely off-site is essential. These backups should be encrypted, and periodic restore tests should be performed to verify their integrity. This helps preserve the volunteer database and other critical data in the event of accidental deletion or cyberattacks. By doing so, Azumer Water meets the FISMA requirement for continuity of operations and data protection, reducing the severity and impact of any future data incidents.

<h2>Recommended Technical Solutions</h2>

<p>Azumer Water should consider implementing several technical solutions to counter the remaining effects of this attack and to prevent similar incidents:</p>

1. **Proper Firewall Configuration and Real-Time Monitoring:** Since a firewall solution is already purchased but not configured, it is essential to complete its setup and enable intrusion detection and prevention systems (IDPS). Regular network traffic monitoring for anomalies or signs of intrusion will act as an early warning system if attackers try to breach the network again.
2.	**Secure Wireless Network and VPN:** Replacing the WEP protocol with WPA2 or WPA3 encryption ensures a much more secure wireless environment. Employees who work outside the main office or remotely should also connect via a Virtual Private Network (VPN). This protects data in transit and helps restrict unauthorized access to Azumer Water’s internal systems.
3.	**Multi-Factor Authentication (MFA):** Implementing MFA for all critical systems, such as email and the volunteer database, adds a second layer of protection. It is much harder for attackers to compromise user accounts when they require a password and a code from a phone app or a physical security token.
4.	**Endpoint Protection and Timely Patching:** The organization should ensure that all devices, from office desktops to personal mobile devices, have updated antivirus or anti-malware software. Applying patches and security updates for operating systems and applications as soon as vendors release them will help close existing security gaps.

<h2>Organizational Structure for IT and Security Management</h2>

<p>Given that Azumer Water is a small NGO, it is crucial to have a clear, though not overly complex, organizational structure that delineates roles in IT and security. At the top, Maria Rodriguez, the <b>Chief Executive Officer (CEO)</b>, is responsible for strategic decisions and resource allocation. The CEO should have a dedicated <b>Information Security Officer (ISO)</b>. This new position would oversee all aspects of cybersecurity strategy, including developing policies, managing risk assessments, and coordinating incident response.</p>

<p>Since Azumer Water currently contracts out its IT services to Pruhart Tech, it is recommended that the ISO work closely with Pruhart Tech daily. This collaboration will ensure firewalls and servers are adequately maintained. Meanwhile, the <b>Volunteer Coordinator (John Smith)</b> should remain responsible for volunteer data and communications but always under the guidance of the ISO to ensure that policies and best practices are followed. By clearly separating these roles, everyone knows their responsibilities, and any security issues can be quickly escalated.</p>

<p>This structure provides for quick decision-making during a crisis. The ISO can rapidly instruct Pruhart Tech to isolate systems or run forensic analysis while reporting back to the CEO, and the volunteer coordinator can manage external communication with volunteers under proper supervision.</p>

<h2>Risk Management Approach</h2>

<p>Azumer Water faces two primary risks from the case study: <b>phishing attacks</b> and <b>database loss or tampering</b>. First, phishing attacks present a <b>high likelihood</b> of occurrence because cybercriminals frequently rely on deceptive emails, and the case study demonstrates that John already clicked on a suspicious link while volunteers received fraudulent donation requests. Although these attacks can be partially mitigated through training and technical controls such as spam filtering and multi-factor authentication, their <b>severity</b> is considered <b>medium.</b> Any successful phishing email can lead to unauthorized access or further system breaches. Should an attacker gain a foothold, the <b>operational impact</b> can display as employee hesitancy to open emails, slowing the organization’s disaster response. The <b>reputational implications</b> occur if volunteers perceive Azumer Water as careless with communications, damaging the trust needed for adequate relief efforts. Furthermore, a successful phishing-based data breach involving volunteer information raises a <b>compliance impact</b> under federal guidelines like the Federal Information Security Modernization Act (FISMA), which mandates strict safeguarding of sensitive data.</p>

<p>In contrast, the risk of database loss or tampering carries a <b>medium likelihood</b> but <b>high severity</b>, given that the volunteer database is critical for coordinating deliveries of clean drinking water. While direct access to the database may require more specific tactics than generic phishing, the disappearance of the volunteer database in the case study confirms that such an attack is feasible. Because this system underpins Azumer Water’s mission, any compromise has a significant <b>operational impact</b>, stopping the scheduling and dispatching of volunteers and effectively suspending relief efforts. The <b>reputational implications</b> stem from volunteers losing confidence in the organization’s capacity to protect their records, potentially deterring future volunteer engagement. Lastly, suppose the database is not correctly secured and backed up. In that case, the <b>compliance impact</b> is significant—FISMA requires robust data protection measures and incident response procedures, both lacking before the incident. Azumer Water must combine proactive strategies, such as routine security awareness training and regular vulnerability assessments, with reactive measures, such as a clear incident response plan and frequent, secured backups to manage these risks.</p>

<h2>References</h2>

- National Institute of Standards and Technology. (2020). Security and Privacy Controls for Information Systems and Organizations (NIST Special Publication 800-53, Revision 5). https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final
- International Organization for Standardization. (2022). ISO/IEC 27002:2022 - Information Security Controls. https://www.iso.org/standard/75652.html
