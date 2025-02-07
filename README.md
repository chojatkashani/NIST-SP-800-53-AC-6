# Data Leak Report

## Incident Summary

A sales manager shared access to an internal-only folder containing:  
- Files related to a new, unannounced product  
- Customer analytics and promotional materials  

### The Problem:  
- The sales manager did not revoke access after the meeting.  
- The team was warned to wait for approval before sharing promotional materials.  

### What Happened Next?  
- A sales representative mistakenly shared the internal folder link instead of promotional materials during a video call with a business partner.  
- The business partner posted the link on their company’s social media page, assuming it was promotional content.  

## Control: Least Privilege

### Issues:
- Access to the internal folder was not restricted to only the sales team and manager.  
- The business partner should not have had permission to share confidential information on social media.  

### Review:  
- NIST SP 800-53: AC-6 addresses least privilege and suggests control enhancements to improve data security.  

### Recommendations:  
- Restrict access to sensitive resources based on user role.  
- Regularly audit user privileges.  

### Justification:  
- Limiting access ensures internal files are not shared externally.  
- Routine audits prevent exposure of sensitive information to unauthorized users.  

## Security Plan Snapshot

The NIST Cybersecurity Framework (CSF) organizes security guidelines into four hierarchical levels:  
**Function → Category → Subcategory → Reference(s)**  

| Function  | Category          | Subcategory                         | Reference(s)               |
|-----------|------------------|-----------------------------------|----------------------------|
| Protect   | PR.DS: Data Security | PR.DS-5: Protections against data leaks | NIST SP 800-53: AC-6 |  

In this case, the manufacturer follows **NIST SP 800-53**, which provides guidelines for securing sensitive information.  

## NIST SP 800-53: AC-6 (Least Privilege)

### Control:  
- Users should be given only the minimal access and authorization required to complete tasks.  

### Discussion:  
- Processes, user accounts, and roles should follow the principle of least privilege.  
- Prevents users from operating at a higher privilege level than necessary.  

### Control Enhancements:  
- Restrict access to sensitive resources based on user roles.  
- Automatically revoke access after a defined period.  
- Keep activity logs of provisioned user accounts.  
- Regularly audit user privileges.  

SP 800-53 categorizes least privilege as AC-6 within access controls.  
<img width="709" alt="Screenshot 2025-02-06 at 8 45 39 PM" src="https://github.com/user-attachments/assets/802b3dbf-a172-45dd-b9fd-b9ef37b7fbca" />

## Summary

This data leak incident highlights the risks of unrestricted access and the importance of enforcing least privilege.  
By implementing **NIST SP 800-53 AC-6 controls**, organizations can:  
- Minimize security breaches  
- Restrict unauthorized access  
- Improve compliance with security best practices  

Proactive security measures prevent future incidents and safeguard critical business data.  
