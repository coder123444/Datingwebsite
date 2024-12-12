# Dating Website Project

## Overview

This project is a fully functional dating website designed to connect users based on their interests, hobbies, and personal details. It offers a visually appealing and interactive user experience, making it engaging for users to find their perfect match in the digital age.

## Features

### Core Functionalities

1. **User Authentication**:
   - Secure login system with username and password verification.
   - Password recovery through a security question.

2. **Profile Matching**:
   - Users can find their most compatible match based on their input details.
   - Ability to browse other profiles through swipeable functionality.
   - Percentage-based compatibility calculation with all profiles.

3. **Interactive Navigation**:
   - Dynamic homepage with CAPTCHA verification.
   - Easy-to-use navigation buttons with sound effects and animations.
   - Logout functionality available on all pages.

4. **Customizable Animations and Effects**:
   - Dynamic background changes every 20 seconds.
   - Stylish headings with gradient effects and animations.
   - Hover effects and fade-in animations for interactive elements.

### CAPTCHA Verification

- **Human Verification**: The homepage implements a CAPTCHA system to ensure that visitors are human, enhancing the security and reliability of the platform.
- **Dynamic CAPTCHA Codes**: Randomized CAPTCHA codes are generated to prevent automated access.
- **Interactive Validation**: Users must correctly input the displayed CAPTCHA to proceed to the login page. This step adds an essential layer of protection to the site.

### Pages and Functionalities

1. **Login Page**:
   - Input validation against stored user data in `login.json`.
   - Dynamic animations and sound effects for enhanced interactivity.

2. **Forgot Password Page**:
   - Allows users to recover their password by answering a security question.
   - Consistent styling and animations.

3. **Dating Form Page**:
   - Collects user details including IITB Roll Number, name, age, email, gender, interests, and hobbies.
   - Multiple options for matching and browsing profiles.

4. **Match Found Page**:
   - Displays the best match with a compatibility percentage.
   - Includes options to contact the match, ask for a date, or find another match.

5. **Swipe Through Profiles Page**:
   - Allows users to swipe through potential matches with interactive navigation buttons.

6. **Percentage Match with All Profiles**:
   - Calculates compatibility with all profiles and presents results dynamically.

### Matching Algorithm

The matching algorithm is designed to optimize compatibility based on:

- **Common Interests and Hobbies**: Higher weightage given to shared interests.
- **Year of Study and Age**: Ensures relevance by considering year of study and age differences.
- **Gender Preferences**: Inclusive matching system that respects user preferences.

```javascript
for (const interest of user.Interests) {
  if (profile.Interests.includes(interest)) {
    interestscore++;
  }
}
for (const hobby of user.Hobbies) {
  if (profile.Hobbies.includes(hobby)) {
    hobbiescore++;
  }
}
const percentagematch = Math.max(
  10,
  100 - yearDiff - (ageDiff / 2) - ... // Additional factors
);
```

## Customizations

### Animations

- **Background Change**: Cycles through images every 20 seconds.
- **Dynamic Headings**: Gradient effects and subtle shaking animations.
- **Interactive Buttons**: Enlarges on hover for engaging visuals.
- **Entrance Effects**: Elements fade in smoothly on page load.
- **Compatibility Meter**: Circular progress bar dynamically fills based on match percentage.

### Sound Effects

- Click sounds for input boxes and navigation buttons.
- Distinct sounds for different actions, enhancing user engagement.

### Email Features

- **Contact Them**: Sends a casual email to initiate communication.
- **Ask for a Date**: Sends a personalized email to propose a date.

## Setup Instructions

1. Unzip the project folder.
2. Open `index.html` using a live server on your local device.
3. Navigate through the website and explore its features.

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript.
- **Backend Data**: JSON files for storing user details.
- **Styling and Animations**: CSS with advanced animations and effects.
- **Audio Effects**: Integrated using JavaScript.
- **Dynamic Content**: JavaScript-driven logic and interactivity.

## Future Enhancements

- Real-time chat functionality.
- Integration with social media for user authentication.
- Advanced AI-based matching algorithms.

## Conclusion

This dating website is designed to provide an engaging and user-friendly platform for finding meaningful connections. With its unique animations, sound effects, and compatibility algorithms, the project demonstrates a perfect blend of technology and user-centric design.
