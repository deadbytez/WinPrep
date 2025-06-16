# PostInstall-WindowsLTSC
> [!WARNING]
> Review the script's code before running.

This script applies changes I make to fresh Windows LTSC installs + offers to run [CutEdge](https://github.com/azhcat/CutEdge).

## Explanation of what each change does
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
