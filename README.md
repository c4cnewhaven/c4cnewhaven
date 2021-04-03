### Hi there 👋

<!--
**c4cnewhaven/c4cnewhaven** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

//JS code for randNum
var oneDayInMs = 1000*60*60*24;
var currentTimeInMs = new Date().getTime();  // UTC time
var timeInDays = Math.floor(currentTimeInMs / oneDayInMs);
var numberForToday = timeInDays % 9999;
console.log(numberForToday);
// zero-filling of numbers less than four digits might be optional for you
// zero-filled value will be a string to maintain its leading 0s
var fourDigitNumber = numberForToday.toString();
while(fourDigitNumber.length < 4)
{
  fourDigitNumber = 0+fourDigitNumber;
}
console.log(fourDigitNumber);
