# ⁉️ Troubleshooting GitBook's Entra ID Authentication

Our Internal Knowledge Base and some other services might require you to log in with your Indiana University Microsoft 365 Account (Microsoft Entra ID). If you run into issues, this is a good place to start!

## User {email} is blocked because they are not a direct member of a group with access

This error means that only members of the TEDxIndianaUniversity group in Entra ID have access to this resource. This means that either:

1. You're not a member of TEDxIndiana University (and won't receive access, sorry!)
2. You're a member but aren't a part of our Microsoft Teams group. If this is you, please contact the Director of Technical Production to resolve the issue.

## There's a different error

### It's Before July 2026

Please contact the Director of Technical Production to resolve the issue with the error and what you are attempting to do.

### It's After July 2026

If it is **after July 2026**, please contact the Director of Technical Production, telling them to "Update GitBook with a new Microsoft Azure Entra ID client secret for the application called TEDxAccess." Then send them a link to this article.

If you're on Technical Production and are attempting to update the client secret for [TEDxAccess](https://portal.azure.com/#view/Microsoft\_AAD\_RegisteredApps/ApplicationMenuBlade/\~/Credentials/appId/5efff15b-6594-46fa-80fe-c650dbadf4d7), you can visit [this support article](https://developer.gitbook.com/visitor-authentication/guides/integrations/how-to-use-azure-ad-integration-for-visitor-authentication) for more information. (Broken link? [Here's the archived version](https://web.archive.org/web/20240521002135/https://developer.gitbook.com/visitor-authentication/guides/integrations/how-to-use-azure-ad-integration-for-visitor-authentication).) Once you complete this process, update the dates in this support document to reflect the new client secret expiration date.
