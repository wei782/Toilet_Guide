# Toilet Guide
## Concepts
The concept of this app comes from my daily experience: I am not used to use those public toilets which crowded, smells bad, etc. So, I thought there should be an online map service which can provide some statistics data or simply reviews to a toilet. But actually, most of the toilets on the major map platform has no review. The application here come for solve this problem.
## Design
This app is localization based, with a map component on the main screen to show all the nearby points of interest (apparently toilets here). User can use this screen to browse all the toilet nearby with different color, which can be customized, to determine which toilet is suited. By tabbed on the toilet icon, user can see details of selected toilet, including cleanness, crowdedness and so on. Users are encouraged to submit their reviews to the toilet, which is the main data source of this app. Without user reviews this app will very limited to a toilet map.

To satisfy all type of user, including disabled personnel, people prefer to identify themselves as neutral sex or family toilet needed person, this app will provide accessible and personalized toilet information as more as possible.

This app will be cross platform, the design element will adapt to what required by the operating system.

Design details will be discussed below.

### Color System
Human is sensitive to color. In this app, user can customize which color can show the toilet status directly. In detail, once certain condition is satisfied, the color can change to user defined one, otherwise, it will turn to another color.
<p align="center">
  <img src="/mockup/iOS/iOS_1.png" />
</p>
The picture above shows sample color strategies, which use traffic lights pattern: green means go to go, yellow means caution and red means no.

### Personalization
The app provides variety of preference options, users can customize their preferences in one place by simply choosing in segment control or list box.
<p align="center">
  <img src="/mockup/iOS/iOS_2.png" />
</p>
The picture above shows mockup preference page under iOS.

### Push Message
User can subscribe a toilet and app will push an information into notification center to notify the user when certain conditions are satisfied. For example, if the crowdedness of a subscribed toilet become acceptable to the user, the app will push a simple local message to the user. (Not go through Apple or Google push server)
<p align="center">
  <img src="/mockup/iOS/iOS_7.png" />
</p>

### Privacy
The app shall not use identification code on a device to analyze data. All data analyze and the algorithm should base on what user will to provide (mostly, toilet rating).

### Accessibility
The app will have voice description support (Apple VoiceOver, Google Talkback) for visual disability person.

## Implementation
Very technological details here.

Rather than just put a browser shell or something like that and make user experience bad, native application is more reasonable to the project. But that do not mean there will be no web client… actually, developing country and region like India and Africa have many Javascript and HTML5 based function phone operating system (KaiOS) running and have large market, this app will be helpful to people there.
