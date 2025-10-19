# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [4.25.18] - 2025-10-19

### Added

- Refresh location when long press on self center on the map button.
- Feature Disabled centralized configuration.
- CHANGELOG.md

### Changed

- Workmanager plugin updated for background tasks when Location Updates enabled.
- onCreate behavior to avoid launch the app when accessing to a generic hugmeter url.
- Gradle update.

### Removed
- GoogleAuthService class.
- Unused code.

## [4.25.11] - 2025-08-23

### Added

- Enabling Multi Hugging Mood for testing.
- Fade effect on Hug Degrees discoverable on the Map.
- Enabled Travel Hug to all Android users.
- Name detail when managing Huggers from a Group.

### Changed

- Reshaped Location Updates options menu.
- Improved Travel Hug disclaimer.
- Reviewed signOut order operations and login displayed texts.
- Updated map Tile Providers.
- List of Tile Providers with their Attribution requirements to offer different map each time the user opens the app.

### Fixed

- Trigger Background Notification when hugger is in the Neighborhood.
- Location Detail information when Location Updates publication on background.
- Display map Tile Attribution requirement when Hugger is selected.

## [4.24.0] - 2025-07-10

### Added

- Manage Huggers belonging to a Group.

## [4.23.20] - 2025-07-07

### Added

- Modal to display Huggers belonging to a Group.
- Configuration window opt out to edge-to-edge enforcement on Android app.
- TimeZone on Push Notification timestamp.

### Changed

- Refactor Travel Hug feature for test experiment.
- App must target Android 15 Sdk (API level 35) or higher.
- Changing chanelName notification to Close Hug Notification.
- Adjusted minimum zoom on the map.
- Reviewed disclaimers and Tips notifications messages.
- Buttons alignment on Hug Degrees options.
- Refactorized Broadcast Hug into their own widget.

### Fixed

- Set the Dark or Light theme mode on SystemUiOverlayStyle to align the system navigation bar color.
- Redirect to Map screen when user applies to Delete Account.
- Database connection restoration after loading user timeout.

## [4.22.3] - 2025-04-02

### Changed

- Refactorized subscription refresh from notification channel.

### Fixed

- Calculation on Days in a Row user accessed.
- Unsubscribe from notification channel before renew the subscription after 30 days.

## [4.22.0] - 2025-04-02

### Changed

- Refactorized button to center user on the map feature into their own widget.

## [4.21.0] - 2025-03-22

### Added

- Feature to center user on the map.

## [4.20.9] - 2025-03-21

### Added

- Duplicated Push Notification investigation.
- Prefetch location when app opens to improve user experience.
- Duplicated Notifications Investigation.
- Rewarded Broadcast Hug.

### Changed

- Mitigate duplicated Push Notification.
- Golden Hug colors adjustment.
- Increased reward points when Hugger has been added.
- Improved loading times with parallel microtasks when the app opens.

### Fixed

- lastRewardedAccess and daysRowAccessed calculation.
- lastAccess storage and comparison with Golden Hug sent.

## [4.19.0] - 2025-03-12

### Added

- Rewarded Golden Hug.

## [4.18.2] - 2025-03-07

### Added

- Enabling Rewards feature for testing.

### Changed

- Rewards refactor.
- Clear Top Hugged every month.

## [4.17.14] - 2025-03-05

### Added

- Publish current timestamp when app opens to track last access.
- Draggable expansion and contraction user behavior on the Huggers list.
- Access to the Account Management from self user selected.
- Display hugs statistics from self user selected.

### Changed

- Rewards feature implementation.
- Lazy Hugs feature set to 65 minutes.
- Refactorized load Last Location when app opens.
- Refactorized Lazy Hugs feature.
- Self user selected refactorized to draggable menu.
- Kotlin upgrade to 2.1.10 and flutter_map upgrade to 8.0.0.
- Gradle Upgrade to 8.5 and related dependencies.

### Fixed

- Filter Lazy Hugs before active hugs to avoid repeated notifications when Close Hug Notifications enabled.

## [4.16.4] - 2025-02-14

### Added

- Select self user from huggers list.
- Configure profile name on Account Management.

### Changed

- Cleaning code.

### Fixed

- Publish configured profile name when sending a Push Notification.

## [4.15.0] - 2025-02-02

### Added

- Hug Statistics with Most Hugged added on profile screen.

## [4.14.7] - 2025-01-31

### Added

- Database online/offline behavior when app goes to resumed or paused lifecycle state.
- Profile screen first implementation for testing.
- Material banner as disclaimer for testing.
- Shortcut to Add Hugger feature when huggers list is empty.

### Changed

- Refactorized profile screen.
- Sorting huggers menu appearance.

## [4.13.8] - 2025-01-11

### Added

- Exception when placemarkFromCoordinates takes more than 4 seconds.
- iOS Test re-enableListeners when AppLifecycleState resumed.

### Changed

- Restore the Requests Pending button to access to the functionality.
- Refactor Events to avoid re-process duplicities.

### Fixed

- Event maximum name length when publish on analytics.
- Do not display Contacts modal when empty results.
- Return back to Add Hugger when navigated to Manage Groups.
- Update Hug info when it refreshes to Hidden option.

## [4.12.1] - 2025-01-03

### Added

- "You Have # Huggers" title on huggers list.

### Changed

- Refactor Add Hugger bottom sheet to group everything together.

### Fixed

- Iterate add hugger to all available groups.
- Remove hugger behavior.

## [4.11.0] - 2025-01-02

### Changed

- Refactorized background task to work with multiples groups.

## [4.10.6] - 2025-01-01

### Added

- Delete Hugger feature.

### Changed

- Refactor to storeHuggersGroupsWithLocationDetail.
- Refactor publish location when Location Detail has changed.
- Refactor send Virtual Hug with the Location Detail according to detail configured on each group.
- Increased draggable bar size for better user experience.

## [4.9.3] - 2024-12-31

### Changed

- Refactorized Groups management.

### Deprecated

- HuggersGroup internal control attribute.

## [4.8.0] - 2024-12-26

### Changed

- Publish Location on all Groups available.

## [4.7.1] - 2024-12-26

### Changed

- Enabled Hugs Degrees Infinite feature to discover any HugMeter user.
- Refactorized Groups management.

## [4.6.0] - 2024-12-18

### Changed

- Hug Degrees Infinite implementation phase.

## [4.5.0] - 2024-12-09

### Added

- Hug Degrees Infinite implementation phase.

## [4.4.0] - 2024-11-22

### Added

- Manage Pending Hugger requests feature.

## [4.3.0] - 2024-11-18

### Added

- Database connection listener for better performance.

## [4.2.0] - 2024-11-18

### Removed

- Old Virtual Hugs listener.

## [4.1.1] - 2024-11-18

### Changed

- Sign In standardization.

### Fixed

- Displayed name on Hugger connection request.

## [4.0.41] - 2024-11-05

### Added

- Monitor Connection Status.
- App version control.
- Add Hugger Flow with Events Listener.
- Add Hugger flow with Push Notification.
- Reject option on Add Hugger flow response.
- Virtual Hug Event publisher.

### Changed

- Launcher Service refactor.
- Refresh Degree selected to Hugger when accepted.

## [4.0.34] - 2024-11-05

### Added

- Add Hugger flow with event notification feature.
- Events listener.
- Measure Load Signed Services time.
- Measure fetch Placemark time.
- Measure Load User time.
- Measure Fetch Location time.
- Measure Fetch Huggers duration.
- Display Hug Degrees request disclaimer.
- Adding registerBGProcessingTask withIdentifier to test iOS BGTask.
- Broadcast Hug for testing.
- Golden Hug option with slider buttons.
- Travel Hug action icon to disable it.
- Timeout and Tolerance Policy when retrieve Location.

### Changed

- Migrate Hug Selected Options to be displayed fully with slider.
- Golden Hug Refactor.
- Delayed Virtual Hug received disclaimer. 
- Send Virtual Hug without disclaimer confirmation when triggered from the button.
- Libraries upgrade.
- Don't display Myself on the map when Location Detail is not Coordinates.
- SnackBar placement over ScopedBottomSheet.
- Load app refactor.
- Default background avatar when NetworkImage exception.
- BGTask timeouts refactor.
- Location Timeout Platform adjustment.
- Refactor Draggable and add shadows on BottomSheet.
- Hug Degrees refactor.
- Remove Huggers from Model to work with HuggersGroup.

### Fixed

- Allow only send Virtual Hug Back option when sender is a Hugger from the Group.

## [4.0.5] - 2024-09-09

### Added

- LastLocation when Background
- Minimize resetLocationUpdates on loading.
- LastLocation to start the map centered app.
- Back button behavior to navigate avoiding suspending the app.
- Codemagic configuration for iOS release.

### Changed 

- Restore allow to send Virtual Hug from Long Press.
- Hug Degrees refactor.

### Fixed

- Drawler Title back icon color.

### [4.0.0] - 2024-09-01

### Changed

- Application design revamp: The map becomes the center of the app usage.

## [3.0.0] - Pending

## [2.0.0] - Pending

## [1.0.0] - Pending

Realtime Database
Pseudonymised Yep
Encryption
Anonymisation (not yet)

## [0.0.0] - Pending
