# WinPrep
> [!WARNING]
> Review the script's code before running.

This script applies changes I make to fresh Windows installs + offers to run [CutEdge](https://github.com/azhcat/CutEdge).

<img src="https://github.com/user-attachments/assets/b7a8c94b-05cb-42cf-9e4f-70e1666f14d4" alt="WinPrep script preview image" width="75%">


## Explanation of what each change does
### These apply for LTSC and GAC
| Registry Key/Value | Setting | Description |
|--------------------|---------|-------------|
| JPEGImportQuality | 100 | Sets JPEG wallpaper quality to 100% (prevents compression) |
| VerboseStatus | 1 | Enables detailed status messages during boot/shutdown/logon |
| ExcludeWUDriversInQualityUpdate | 1 | Prevents driver installation through Windows Update |
| AllowTelemetry | 0 | Sets telemetry to Security level |
| Disabled (Windows Error Reporting) | 1 | Disables Windows Error Reporting |
| DiagTrack (Service Control) | Disabled | Stops and disables the DiagTrack (telemetry) service |
| DisableCAD | 0 | Forces CTRL+ALT+DEL requirement at login |
| DontDisplayUserName | 1 | Hides username during login |
| DontDisplayLastUserName | 1 | Hides last logged-in username |
| powercfg /h off | off | Disables hibernation & Fast Startup |
| DisableAutomaticRestartSignOn | 1 | Prevents automatic sign-in after updates/restarts |
| SubmitSamplesConsent (PowerShell) | 2 | Sets Windows Defender sample submission to "Never send" |
| HideFileExt | 0 | Shows file extensions for all files |
| Hidden | 1 | Shows hidden files and folders |
| LaunchTo | 1 | Sets File Explorer to open to "This PC" |
| ShowRecent | 0 | Disables "Show recently used files" in Quick Access |
| ShowFrequent | 0 | Disables "Show frequently used folders" in Quick Access |
| HttpAcceptLanguageOptOut | 1 | Prevents websites from accessing language list |
| Start_TrackProgs | 0 | Disables app launch tracking for Start menu |
| RestrictImplicitTextCollection | 1 | Disables typing data collection |
| RestrictImplicitInkCollection | 1 | Disables inking data collection |
| HarvestContacts | 0 | Prevents harvesting contacts for personalization |
| ActivityHistoryEnabled | 0 | Disables storing activity history on device |
| IsAADCloudSearchEnabled | 0 | Disables cloud search for work/school accounts |
| IsMSACloudSearchEnabled | 0 | Disables cloud search for Microsoft accounts |
| IsDeviceSearchHistoryEnabled | 0 | Disables search history on device |
| NumberOfSIUFInPeriod | 0 | Sets feedback frequency to "Never" |
| SafeSearchMode | 0 | Disables SafeSearch (sets to "Off") |
| AllowGameDVR | 0 | Disables Game Recording and Broadcasting |
| HideRecentlyAddedApps | 1 | Hides recently added apps in Start menu |
| Start_TrackDocs | 0 | Disables document tracking for Start menu |
| EnableAccountNotifications | 0 | Disables account-related notifications |
| DisableSpotlightCollectionOnDesktop | 1 | Disables Windows Spotlight image collection on the desktop background |
| DisableSoftLanding | 1 | Disables the "Soft Landing" first-run experience and tips in Windows |

### These apply only for GAC
| Registry Key/Value | Setting | Description |
|--------------------|---------|-------------|
| ContentDeliveryAllowed | 0 | Disables all content delivery features from Microsoft |
| SubscribedContentEnabled | 0 | Disables subscribed content |
| OemPreInstalledAppsEnabled | 0 | Disables installation of OEM preinstalled apps for the user |
| PreInstalledAppsEnabled | 0 | Disables installation of Microsoft preinstalled apps for the user |
| PreInstalledAppsEverEnabled | 0 | Indicates preinstalled apps have never been enabled for the user |
| SilentInstalledAppsEnabled | 0 | Disables silent installation of apps suggested by Microsoft |
| SubscribedContent-310093Enabled | 0 | Disables specific subscribed content (ID 310093) from showing |
| SubscribedContent-338393Enabled | 0 | Disables specific subscribed content (ID 338393) from showing |
| SubscribedContent-353694Enabled | 0 | Disables specific subscribed content (ID 353694) from showing |
| SubscribedContent-353696Enabled | 0 | Disables specific subscribed content (ID 353696) from showing |
| SystemPaneSuggestionsEnabled | 0 | Disables suggestions in the Start menu and system panes |
| SubscribedContent-338387Enabled | 0 | Disables specific subscribed content (ID 338387) from showing |
| RotatingLockScreenOverlayEnabled | 0 | Disables fun facts, tips, and more overlays on the lock screen |
| SubscribedContent-338388Enabled | 0 | Disables specific subscribed content (ID 338388) from showing |
| SubscribedContent-338389Enabled | 0 | Disables specific subscribed content (ID 338389) from showing |
| SoftLandingEnabled | 0 | Disables the "Soft Landing" first-run experience and tips |
| DisableWindowsSpotlightFeatures | 1 | Disables all Windows Spotlight features on lock screen and elsewhere |
| DisableWindowsSpotlightWindowsWelcomeExperience | 1 | Disables Windows Spotlight suggestions in the Welcome experience |
| DisableWindowsSpotlightOnActionCenter | 1 | Disables Windows Spotlight suggestions in the Action Center |
| DisableWindowsSpotlightOnSettings | 1 | Disables Windows Spotlight suggestions in the Settings app |
| DisableThirdPartySuggestions | 1 | Disables third-party app suggestions from Microsoft |
