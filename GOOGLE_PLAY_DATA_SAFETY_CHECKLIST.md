# Google Play Data Safety Checklist
**App:** Benny’s Mathanomical Adventure  
**Last Reviewed:** February 22, 2026

Use this checklist when filling Play Console data safety and Families declarations.

## 1. Preconditions (Must Stay True)
- App works offline
- No account/login system
- No third-party analytics SDK
- No ad SDK
- No user data sent to developer servers
- No child-directed behavioral advertising

If any of the above changes, update:
- App code
- Privacy Policy
- Play Console Data Safety form
- Families Policy declarations

## 2. Data Collection and Sharing (Play Console)
Expected answers based on current app design:

- **Does your app collect or share any of the required user data types?** No
- **Is all data processed ephemerally?** Not applicable if no collection
- **Can users request data deletion?** No collected server-side personal data; local data can be deleted by uninstall/clear storage

## 3. Data Types Audit
Confirm each remains true before each release:

- Personal info (name, email, user IDs): Not collected
- Financial info (card/bank): Not collected by developer; handled by Google Play billing
- Health/fitness: Not collected
- Messages: Not collected
- Photos/videos: Not collected
- Audio files/recordings: Not collected
- Files and docs: Not collected
- Calendar: Not collected
- Contacts: Not collected
- App activity: Not collected by developer analytics
- Web browsing: Not collected
- App info/performance diagnostics sent to developer: Not collected (unless crash SDK added)
- Device or other IDs: Not collected by developer
- Location (approx/precise): Not collected

## 4. Security Practices
- Data in transit: Not applicable for no data transmission by developer
- Local-only progress storage confirmed
- Release build checked for unexpected network calls

## 5. Families Policy Alignment
- Target audience and content declarations match app audience
- No ad SDKs serving child-targeted behavioral ads
- No social features requiring personal data sharing
- Store listing, privacy policy, and in-app behavior are consistent

## 6. Billing and Purchases
- App is a paid app on Google Play (one-time purchase)
- Payment details handled by Google Play
- Privacy Policy states developer does not store full payment card details

## 7. Release Gate (Do Not Ship Until Complete)
- Privacy Policy URL in Play Console is live and public
- Effective date updated
- Contact email and mailing address present in policy
- Data Safety answers re-verified against actual build
- Families declarations re-verified
- QA smoke test confirms no hidden trackers/SDK traffic

## 8. Change Log Template
For each release, record:

- Version:
- Date:
- Any new SDKs:
- Any new permissions:
- Any new network endpoints:
- Data Safety form changed? (Yes/No)
- Privacy Policy changed? (Yes/No)
- Reviewer:
