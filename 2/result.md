# Bug Report: Logout Button Non-Functional in Safari Browser

## Description  
The logout button fails to respond when clicked in Safari browser. This prevents users from properly ending their session, creating potential security concerns.

## Steps to Reproduce  
1. Launch Safari browser (v16.4+)  
2. Log into the application  
3. Attempt to logout via:  
   - Main navigation menu (top-right)  
   - Account settings page  
4. Observe behavior  

## Expected vs Actual Results  
| Expected | Actual |  
|----------|--------|  
| Session terminates | No response |  
| Redirect to login page | Page remains unchanged |  
| Confirmation message | No feedback received |  

## Environment  
**Browser:** Safari 16.4+  
**OS:** macOS Ventura 13.3 / iOS 16.5  
**Device Types:**  
- MacBook Pro (M1/M2)  
- iPhone 14 Pro  
**App Version:** 2.3.1  

## Impact Assessment  
**Severity:** High (P1)  
**Impact:**  
- Security vulnerability (forced session persistence)  
- Violates GDPR/logout compliance requirements  
- Negative user experience  

## Additional Context  
- Issue occurs consistently across Safari versions  
- No JavaScript errors in console  
- Works normally in Chrome/Firefox  
- First reported by QA team on 2023-11-15  

## Attachments  
- [Screen recording](path/to/video.mp4)  
- [Console logs](path/to/logs.txt)  

## Traceability  
Requirement: SEC-204 (Mandatory logout functionality)  
Test Case: TC-4112  