# GitHub Webhook Setup (Jenkins CI Trigger)

- [GitHub Webhook Setup (Jenkins CI Trigger)](#github-webhook-setup-jenkins-ci-trigger)
  - [Purpose](#purpose)
  - [Steps](#steps)
    - [Webhook Configuration](#webhook-configuration)
  - [Result](#result)
  - [Screenshots](#screenshots)

## Purpose
The webhook notifies Jenkins when code is pushed to GitHub, triggering Job 1 automatically.

---

## Steps

1. Go to the GitHub repository  
2. Navigate to **Settings → Webhooks**
3. Click **Add webhook**

### Webhook Configuration

- **Payload URL:**
http://<jenkins-ip>:8080/github-webhook/


- **Content type:** `application/json` (default)
- **Secret:** not required
- **Active:** ✅ checked

4. Click **Add webhook**

---

## Result
- Any push to the repository sends a notification to Jenkins
- Jenkins triggers Job 1 automatically
- CI pipeline starts without manual intervention

---

## Screenshots
Include:
- GitHub webhook configuration
- Successful webhook delivery (green tick)
