# Notifications

### Send Notification to a specific mail address
Tutorial for set specific email for notifications
- [Manage notifications for a team, project, organization or collection - Azure DevOps | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/organizations/notifications/manage-team-group-global-organization-notifications?view=azure-devops&tabs=new-account-enabled)
- For Add new mail addres: 
	- Project Settings > Notifications > + New Subscription
- For disable mail addres:
	- Project Settings > Notifications > toggle Status switch 
![[Pasted image 20221226140915.png]]

### Edit Mail Template
Currently this function is not available. But It is been requested.
- Functionality Request:
	- [Customise VSTS email templates - Visual Studio Feedback](https://developercommunity.visualstudio.com/t/customise-vsts-email-templates/365760)
- Stackoverflow disscussion
	- [How to modify Azure Devops email notification template? - Stack Overflow](https://stackoverflow.com/questions/55632159/how-to-modify-azure-devops-email-notification-template)


**Workaround to send custom emails:**
| # | Name | Workaround |
| - | - | - |
| 1 | Trigger external process | On Pipeline complate, trigger: </br> - PowerAutome </br> - Microsoft Flow |
| 2 | Send email from pipeline | Inside the pipeline execute a program that sends an emails or connects with and external sysmtem |

### Trigger for notification
- For trigger a notification when a pipeline finish its execution (regarding on the result), set the trigger to **Build -> A build completes**
![[Pasted image 20221226141235.png]]


