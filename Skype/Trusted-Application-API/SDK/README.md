# README

Thank you for your interest in Skype for Business developer documentation!

## Release Notes

### 1.0.0-prerelease5

Key changes:
 1. IInvitation.WaitForInviteCompleteAsync() now returns the related IConversation

Bug fixes:
 1. AdhocMeetingCreationInput was ignoring the AccessLevel when creating the meeting
 2. Accessing IAnonymousApplicationToken.AuthTokenExpiryTime was throwing an exception
 3. IMessaginCall.IncomingMessageReceived wasn't providing the incoming Text/Html message in IncomingMessageEventArgs

Dependency changes:
 1. Microsoft.SkypeforBusiness.TrustedApplicationAPI.ResourceContract [7.0.1586.0,)
 2. Microsoft.AspNet.WebApi.Core [5.2.3,)

### 1.0.0-prerelease4

Key changes:
 1. ClientPlatformSettings, IClientPlatform and ClientPlatform don't expose IsInternalPartner and IsSandBoxEnv properties anymore; they are available as extensions
 2. New sample (QuickStartSamples/TrustedJoinMeeting.sln) is available showing how to do a trusted join into a meeting. It also introduces a sample TrouterBasedEventChannel which can be used to debug issues without having to deploy
 3. Some officially unsupported extension methods are available under Microsoft.SfB.PlatformService.SDK.ClientModel.Internal namespace to help developers

New methods:
 1. IApplication.GetAnonApplicationTokenForMeetingAsync() replaces IApplication.GetAnonApplicationTokenAsync().
 2. IApplication.CreateAdhocMeetingAsync() replaces IApplication.GetAdhocMeetingResourceAsync()
 3. IApplication.GetAnonApplicationTokenForP2PCallAsync()
 4. IParticipant.EjectAsync()
 5. IAudioVideoInvitation.AcceptAndBridgeAsync()
 6. IAudioVideoInvitation.StartAdhocMeetingAsync()
 7. IAdhocMeeting is now available and supports JoinAdhocMeeting()

Corresponding changes to Capability enums have been made

Dependency changes:
 1. System.Net.Http [4.0,4.1)
 2. Microsoft.SkypeforBusiness.TrustedApplicationAPI.ResourceContract [7.0.1567.0,)

### 1.0.0-prerelease3

Key changes:
 1. ClientPlatformSettings' constructor no longer accepts IsSandBoxEnv

Dependency changes:
 1. System.Net.Http (,4.1)
 2. CommonServiceLocator is no longer a dependency

### 1.0.0-prerelease2

Minor bug fixes

### 1.0.0-prerelease1

Initial release

## **Trusted Application SDK** documentation

The markdown documents in this repository project are the source of the **Trusted Application SDK** documentation available to the public preview release, the Microsoft developer site at msdn.microsoft.com/skype.

## Contribute to the documentation

You may want to contribute new content or improve existing **Trusted Application SDK** content. If you do, then clone this repoistory, 
create a new branch from the master branch, add your content, and then create a pull request to contribute your changes back into master branch.
Pull requests are the way to move changes from a topic branch back into the master branch.

Click on the **Pull Requests** page in the **CODE** hub, then click "New Pull Request" to create a new pull request from your topic branch to the master branch.

When you are done adding details, click "Create Pull request". Once a pull request is sent, reviewers can see your changes, recommend modifications, or even push follow-up commits.

First time creating a pull request?  Learn [about pull requests](https://help.github.com/articles/about-pull-requests/).

## Documentation images

The images in the **Trusted Application SDK** documentation are .png or .jpg images. They may not render with full fidelity in your browser. If you need to see more detail
in an image, right-click the image in your browser and download it to your computer. The original full size image is downloaded.

# Next steps

If you haven't already done so, [install Git](https://git-scm.com/downloads) (as well as [Git Credential Manager](https://java.visualstudio.com/Downloads/gitcredentialmanager/Index) for Linux or Mac OS)

Choose and install one of these supported IDEs:
* [Visual Studio](https://go.microsoft.com/fwlink/?LinkId=309297&clcid=0x409&slcid=0x409)
* [Visual Studio Code](https://code.visualstudio.com/Download) (with [Team Services Extension](https://java.visualstudio.com/Downloads/visualstudiocode/Index))

Then clone this repo to your local machine to get started with your own project.

Happy writing!
