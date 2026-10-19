# Phone Club uptime

Every 10 minutes, GitHub Actions checks:

- the five sites (phoneclub.in, sell, logistics, admin, selladmin)
- the API and its database
- how many days the HTTPS certificates have left

When anything is down, or a certificate has under 14 days left, the run fails and GitHub emails
the repo owner. The results are in the **Actions** tab.

To get those emails: GitHub → Settings → Notifications → **Actions** → tick **Email** (with
"Only notify for failed workflows").
