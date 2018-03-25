# xDaysOfcode_ReactNative
Daily log of learning and creating a production ready react native app

### Day 1.
Finally, I decided to learn React Native and wanted to re-write one of the existing app of my client ( Yes, for free );
Question was where to start from and ofcourse google ad did its work properly and I was shown an Udemy ad every time, so then I decided to take a course from Udemy by Stephen Grider.

### Day 2.
Some how spent the entire day watching videos at the 2X speed. Also, an empty editor was open through out the day in the background, Just in case I felt like writing a line of code. 😴


### Day 3.
I am always fascinated by the code editors. Hence, decided to install Webstorm IDE. Although, Stephen used Atom through out his course, I decided to use Webstorm because I have never used it before. I thought this would motivate me enough to write the code now.

### Day 4.
Finally Completed the Video course. 🎇

### Day 5.
Bootstraped and empty project and kept staring 👀 at the sample app in a simulator and thinking about the various components.


### Day 6.
Decided to start with Login component, Basically a Name and MobileNumber as I will be using the OTP based Authentication. Again spent entire day figure out how the hell layouts worked in ReactNative. Tried the UI Library '@Shoutem/ui'. After struggling for 4 hours decided to scrap this library and find something else.

### Day 7.
Read about another UI library for React Native component called NativeBase. After spending an hour on the documentation, Decided to go with own custom component and only use the library when building own component is too complex.
Also, I faced an issue when I uninstalled the @Shoutem/ui library. Came to know that first you have to unlink the library and then uninstall it. The correct process goes like this
```
react-native unlink @shoutem/ui  
npm uninstall --save @shoutem/ui
```

### Day 8. Sat, 24/Mar/18
Created the LoginForm component which consist of childrens such as Input. Struggled for a while to get the layout right.
Things to note: Height plays a vital role in component layout. Trying to understand whether components are by default absolutely positioned or relative, still it is not clear.

### Day 9. Sun, 25/Mar/18
Wired up the action creator and redux store using react-redux. In Stephen's video he dispatched action on every change of the Input, However I decided to try to dispatch action only on the click of Submit button. By doing this I came to know that the component maintains their state even if it is re-rendered but still need to confirm this because I think react's diffing mechanism does the magic here and that particular part of the component is not re-rendered. 🤯
Also, added [country list picker](https://github.com/xcarpentier/react-native-country-picker-modal) for allowing the user to select the correct country code for his mobile number.
LoginForm is almost there, time to add Validation or the Error message and the loading state to the component.


