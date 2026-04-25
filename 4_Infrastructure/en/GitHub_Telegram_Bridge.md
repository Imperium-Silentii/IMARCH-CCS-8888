# GITHUB-TELEGRAM NOTIFICATION BRIDGE

## 1. PURPOSE
To provide immediate transparency. Every time a "Renovation Act" or "Incident Act" is committed to this repository, the system triggers a notification to the official Telegram Channel of the Trust Service.

## 2. DATA FLOW
1. **Trigger:** `git commit` + `git push` to the main branch.
2. **Webhook:** GitHub sends a JSON payload to the bridge server.
3. **Parsing:** The bridge extracts the Act ID and the Hash.
4. **Broadcast:** Message is sent to the authorized Telegram group/channel.

## 3. AUDIT TRAIL
This bridge ensures that no one can "silently" edit the Chronicle. Every change is announced to the community and stakeholders in real-time.
