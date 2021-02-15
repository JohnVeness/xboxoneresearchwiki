# Protocol URIs (deep links)
Protocol URI are used to provide a means for apps to start other apps. An example of protocol URIs being used can be found in the url (`ms-windows-store://`) used to activate the store on the page for a certain app. Protocol URIs are also know as deep links or launch URIs. Info on how to implement them into your uwp app can be found [here](https://docs.microsoft.com/en-us/windows/uwp/launch-resume/handle-uri-activation).

## System apps:
The following list shows a complete list of deep links as of `10.0.19041.6630 (xb_flt_2103vb.210210-0000)` there may be a small number missing.
These were dumped by pulling all of the appx manifests accessible to a custom admin account in dev mode and then parsing all of them to get the protocol URIs.
| Identity Name                        | Display Name                                   | Publisher Display Name           | Publisher Identity                                                               | URI                                                            |
| ------------------------------------ | ---------------------------------------------- | -------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| Microsoft.Xbox.TvSettings            | TvSettings                                     | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbox-tvsettings://](ms-xbox-tvsettings://)                 |
| Xbox.SU                              | Xbox System Update                             | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [systemupdatenew://](systemupdatenew://)                       |
| Microsoft.MicrosoftEdge              | ms-resource:AppName                            | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [read://](read://)                                             |
| Microsoft.XboxCare                   | Xbox Assist                                    | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xcare://](ms-xcare://)                                     |
| Xbox.TrialOverlay                    | ms-resource:TrialOverlay_Package_Display_Name  | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [trialoverlay://](trialoverlay://)                             |
| Microsoft.storify                    | Microsoft Store                                | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-windows-store://](ms-windows-store://)                     |
| Microsoft.Xbox.Settings              | Xbox Settings                                  | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [kinecttuner://](kinecttuner://)                               |
| Microsoft.NTSCaptivePortal           | NTSCaptivePortal                               | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ntscaptiveportal://](ntscaptiveportal://)                     |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbox-gamedvr2://](ms-xbox-gamedvr2://)                     |
| Microsoft.WindowsStore               | ms-resource:StoreTitle                         | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [microsoftvideo://](microsoftvideo://)                         |
| Microsoft.MicrosoftEdge              | ms-resource:AppName                            | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [http://](http://)                                             |
| Microsoft.MicrosoftEdge              | ms-resource:AppName                            | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [https://](https://)                                           |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbox-dashboard://](ms-xbox-dashboard://)                   |
| Microsoft.XboxDevices                | ms-resource:LandingPageTitle\Text              | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbl-2d34608b://](ms-xbl-2d34608b://)                       |
| Microsoft.WindowsStore               | ms-resource:StoreTitle                         | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-windows-store://](ms-windows-store://)                     |
| Microsoft.WindowsStore               | ms-resource:StoreTitle                         | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-windows-store2://](ms-windows-store2://)                   |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [screenshots://](screenshots://)                               |
| Microsoft.Xbox.DevHome               | Dev Home                                       | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbl-1c835833://](ms-xbl-1c835833://)                       |
| Xbox.VideoPlayer                     | Xbox Video Player                              | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xpreviewkiosk://](xpreviewkiosk://)                           |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [gameclips://](gameclips://)                                   |
| Microsoft.XboxCare                   | Xbox Assist                                    | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xhelp://](xhelp://)                                           |
| Microsoft.XboxDevices                | ms-resource:LandingPageTitle\Text              | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xboxaccessories://](xboxaccessories://)                       |
| XdashLauncher                        | ConsoleSupport                                 | Microsoft                        | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xdash://](ms-xdash://)                                     |
| Microsoft.WindowsStore               | ms-resource:StoreTitle                         | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [microsoftmusic://](microsoftmusic://)                         |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbox-achievements://](ms-xbox-achievements://)             |
| Xbox.IdleScreen                      | Xbox IdleScreen                                | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [idlescreen://](idlescreen://)                                 |
| Xbox.SingleUserProxy                 | Xbox SingleUserProxy                           | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xsingleuserproxy://](xsingleuserproxy://)                     |
| XdashLauncher                        | ConsoleSupport                                 | Microsoft                        | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-content-picker://](ms-content-picker://)                   |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbl-gamedvr2://](ms-xbl-gamedvr2://)                       |
| Xbox.BroadcastSetup                  | Xbox BroadcastSetup                            | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xpositioningtcui://](xpositioningtcui://)                     |
| Microsoft.MicrosoftEdge              | ms-resource:AppName                            | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [microsoft-edge://](microsoft-edge://)                         |
| Microsoft.WindowsStore               | ms-resource:StoreTitle                         | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xboxmusic://](xboxmusic://)                                   |
| Xbox.Guide                           | Xbox Guide                                     | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [guide://](guide://)                                           |
| Xbox.HDRGameCalibration              | ms-resource:AppDisplayName                     | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [hdrgamecalibration://](hdrgamecalibration://)                 |
| Microsoft.XboxEvents                 | Xbox Events                                    | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xbox-events://](xbox-events://)                               |
| XdashLauncher                        | ConsoleSupport                                 | Microsoft                        | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-subscription://](ms-subscription://)                       |
| Microsoft.XboxCare                   | Xbox Assist                                    | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-oobe://](ms-oobe://)                                       |
| Xbox.SignIn                          | Xbox SignIn                                    | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [signin://](signin://)                                         |
| Microsoft.Xbox.LiveTV                | EPG                                            | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbl-162615ad://](ms-xbl-162615ad://)                       |
| Xbox.NetworkTroubleshooter           | Xbox NetworkTroubleshooter                     | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [networktroubleshooter://](networktroubleshooter://)           |
| Microsoft.StorePurchaseApp           | ms-resource:DisplayTitle                       | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbet-survey://](ms-xbet-survey://)                         |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [library://](library://)                                       |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbl-achievements://](ms-xbl-achievements://)               |
| Microsoft.WindowsStore               | ms-resource:StoreTitle                         | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [zune://](zune://)                                             |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [gamedvr2://](gamedvr2://)                                     |
| Microsoft.MicrosoftEdge              | ms-resource:AppName                            | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbl-3d8b930f://](ms-xbl-3d8b930f://)                       |
| Microsoft.Xbox.Settings              | Xbox Settings                                  | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-settings://](ms-settings://)                               |
| Xbox.StorageManagement               | Xbox Storage Management                        | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [storagemanagement://](storagemanagement://)                   |
| Microsoft.CloudExperienceHost        | ms-resource:appDescription                     | ms-resource:PublisherDisplayName | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-device-enrollment://](ms-device-enrollment://)             |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xbox-club://](xbox-club://)                                   |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbl-281d1c2f://](ms-xbl-281d1c2f://)                       |
| Microsoft.QuickBuy                   | QuickBuy                                       | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbox-quickbuy://](ms-xbox-quickbuy://)                     |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [social://](social://)                                         |
| Microsoft.CloudExperienceHost        | ms-resource:appDescription                     | ms-resource:PublisherDisplayName | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-cxh://](ms-cxh://)                                         |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xbox-gamehub://](xbox-gamehub://)                             |
| Microsoft.Xbox.OOBE                  | Xbox OOBE                                      | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [oobe://](oobe://)                                             |
| Xbox.Dashboard                       | Xbox Dashboard                                 | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [achievements://](achievements://)                             |
| Microsoft.Xbox.Settings              | Xbox Settings                                  | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [settings://](settings://)                                     |
| Xbox.VideoPlayer                     | Xbox Video Player                              | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [xpreview://](xpreview://)                                     |
| Xbox.EditorialHost                   | ms-resource:EditorialHost_Package_Display_Name | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [editorialhost://](editorialhost://)                           |
| Microsoft.Microsoft.Xbox.AdsLauncher | Microsoft.Xbox.AdsLauncher                     | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-ad-hwa://](ms-ad-hwa://)                                   |
| Microsoft.Xbox.LiveTV                | EPG                                            | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbox-livetv://](ms-xbox-livetv://)                         |
| Microsoft.Xbox.Settings              | Xbox Settings                                  | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-xbl-6d83c5c3://](ms-xbl-6d83c5c3://)                       |
| XdashLauncher                        | ConsoleSupport                                 | Microsoft                        | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [ms-survey://](ms-survey://)                                   |
| Microsoft.MicrosoftEdge              | ms-resource:AppName                            | Microsoft Corporation            | CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US | [microsoft-edge-holographic://](microsoft-edge-holographic://) |
|                                      |