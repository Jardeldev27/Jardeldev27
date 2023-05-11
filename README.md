const introductions = [
  "Hey there! My name is %s and I'm a full-stack developer with a passion for coding.",
  ];
const aboutMe = [
    "Aside from coding, I also have a passion for Math.",
];
function generateIntroduction(name) {
  const introduction = introductions[Math.floor(Math.random() * introductions.length)];
  return introduction.replace('%s', name);
}
function generateAboutMe() {
  return aboutMe[Math.floor(Math.random() * aboutMe.length)];
}
const name = "Jardel";
const introduction = generateIntroduction(name);
const aboutMeMessage = generateAboutMe();
console.log(introduction);
console.log(aboutMeMessage);
