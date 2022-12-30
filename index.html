const langSwitch = document.querySelector(".lang-switch");
const langSwitchSVG = document.querySelector(".lang-switch svg");
const formTopSection = document.querySelector(".form-top-section");
const advanceSection = document.querySelectorAll(".advance-option");
const copyButton = document.querySelector(".copy-wrapper");
const passwordLengthRange = document.querySelector(".password-length-range");
const form = document.querySelector(".form");
console.log(language);
//Getting Checkboxes
const lowercaseCheckbox = document.getElementById("lowercase");
const uppercaseCheckbox = document.getElementById("uppercase");
const numbersCheckbox = document.getElementById("numbers");
const symbolsCheckbox = document.getElementById("symbols");
const wordsCheckbox = document.getElementById("words");
const similarCharactersCheckbox = document.getElementById("similarCharacters");
const doNotIncludeField = document.getElementById("doNotInclude");
const passfield1 = document.getElementById("passfield1");
const passfield2 = document.getElementById("passfield2");
const advanceSwitch = document.getElementById("advance-switch");

//Toggle Select Boxes to indicate checked and unchecked
function toggleCheckBoxes(e) {
  e.preventDefault();
  e.target.parentElement.classList.toggle("selected");

  wordsCheckbox.checked = false;
  wordsCheckbox.parentElement.classList.remove("selected");

  formTopSection.classList.remove("has-textarea");

  if (form) {
    form.addEventListener("submit", generatePassword);
  }

  return;
}

function toggleWordsCheckBox(e) {
  e.preventDefault();
  e.target.parentElement.classList.toggle("selected");

  if (e.target.id !== "advance-switch") {
    //uncheck all the other checkboxes if word-based is checked\
    lowercaseCheckbox.checked = false;
    lowercaseCheckbox.parentElement.classList.remove("selected");

    uppercaseCheckbox.checked = false;
    uppercaseCheckbox.parentElement.classList.remove("selected");

    numbersCheckbox.checked = false;
    numbersCheckbox.parentElement.classList.remove("selected");

    symbolsCheckbox.checked = false;
    symbolsCheckbox.parentElement.classList.remove("selected");

    similarCharactersCheckbox.checked = false;
    similarCharactersCheckbox.parentElement.classList.remove("selected");

    // Show/Hide textarea if word-based is checked/Unhide
    formTopSection.classList.toggle("has-textarea");

    if (form) {
      form.addEventListener("submit", generatePassword);
    }
  } else {
    [...advanceSection].map((section) => {
      section.classList.toggle("advance-active");
    });
  }

  return;
}

//toggle lowercase checkbox
if (lowercaseCheckbox) {
  lowercaseCheckbox.addEventListener("change", toggleCheckBoxes);
}

//toggle uppercase checkbox
if (uppercaseCheckbox) {
  uppercaseCheckbox.addEventListener("change", toggleCheckBoxes);
}

//toggle numbers checkbox
if (numbersCheckbox) {
  numbersCheckbox.addEventListener("change", toggleCheckBoxes);
}

//toggle symbols checkbox
if (symbolsCheckbox) {
  symbolsCheckbox.addEventListener("change", toggleCheckBoxes);
}

//toggle symbols checkbox
if (similarCharacters) {
  similarCharacters.addEventListener("change", toggleCheckBoxes);
}

//toggle word-based checkbox
if (wordsCheckbox) {
  wordsCheckbox.addEventListener("change", toggleWordsCheckBox);
}

//toggle word-based checkbox
if (wordsCheckbox) {
  wordsCheckbox.addEventListener("change", toggleWordsCheckBox);
}

//toggle word-based checkbox
if (advanceSwitch) {
  advanceSwitch.addEventListener("change", toggleWordsCheckBox);
}

// Set password strength meter
function setPasswordStrength(passwordLength) {
  const passwordStrength = document.querySelector(".password_strength");

  const weakPasswordMaxLength = 9;
  const semiWeakPasswordMaxLength = 20;
  const goodPasswordMaxLength = 40;

  if (passwordLength <= weakPasswordMaxLength) {
    passwordStrength.style.backgroundColor = "var(--color-danger-dark)";
    passwordStrength.style.width = "15%";
  } else if (passwordLength <= semiWeakPasswordMaxLength) {
    passwordStrength.style.backgroundColor = "var(--color-warning-dark)";
    passwordStrength.style.width = "45%";
  } else if (passwordLength <= goodPasswordMaxLength) {
    passwordStrength.style.backgroundColor = "var(--color-success)";
    passwordStrength.style.width = "75%";
  } else {
    passwordStrength.style.backgroundColor = "var(--color-success-dark)";
    passwordStrength.style.width = "100%";
  }
}

// Display password length value to the user.
function passwordLength(e) {
  let lengthDisplay = document.querySelector(".length-display");

  lengthDisplay.innerText = e.target.value;
  setPasswordStrength(e.target.value);

  generatePassword();

  return;
}

if (passwordLengthRange) {
  passwordLengthRange.addEventListener("input", passwordLength);
  passwordLengthRange.addEventListener("change", passwordLength);
}
//function to copy password from the textfield
function copyPassword() {
  let passfield;

  if (wordsCheckbox.checked) {
    passfield = document.getElementById("passfield1");
  } else {
    passfield = document.getElementById("passfield2");
  }

  let feedbackEle = document.querySelector(".copy-feedback");

  /* Select the text field */
  passfield.select();
  passfield.setSelectionRange(0, 99999); /*For mobile devices*/

  /* Copy the text inside the text field */
  document.execCommand("copy");

  // Only display feedback when passfield contains a value.
  if (passfield.value) {
    feedbackEle.style.top = "22px";
    setTimeout(() => {
      feedbackEle.style.top = "";
    }, 2000);
  }

  return;
}

if (copyButton) {
  copyButton.addEventListener("click", copyPassword);
}

function alphabets() {
  return "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
}

function numberList() {
  return "0123456789";
}

function symbolList() {
  return "~`!@#$%^&*()_-+={[}]|\\:;\"'<,>.?/";
}

function wordsList() {
  return WordList();
}

function generatePassword(e) {
  let lowerletters;
  let upperletters;
  let numbers;
  let symbols;
  let words;
  let generatedPassword = "";

  e?.preventDefault();

  // Return an error to the user if no option is selected.
  if (
    !lowercaseCheckbox.checked &&
    !uppercaseCheckbox.checked &&
    !numbersCheckbox.checked &&
    !symbolsCheckbox.checked &&
    !wordsCheckbox.checked
  ) {
    let feedbackElement = document.querySelector(".error-wrapper");

    feedbackElement.style.display = "block";
    feedbackElement.children[0].innerText = language.no_option_error_text;

    setTimeout(() => {
      feedbackElement.style.display = "";
    }, 3000);

    return;
  }

  // Return an error to the user if only symbol option is selected.
  if (
    !lowercaseCheckbox.checked &&
    !uppercaseCheckbox.checked &&
    !numbersCheckbox.checked &&
    !wordsCheckbox.checked &&
    symbolsCheckbox.checked
  ) {
    let feedbackElement = document.querySelector(".error-wrapper");

    feedbackElement.style.display = "block";
    feedbackElement.children[0].innerText = language.symbol_only_error_text;

    setTimeout(() => {
      feedbackElement.style.display = "";
    }, 3000);

    return;
  }

  // Add lowercase letters to generatedPassword if the option is checked.
  if (lowercaseCheckbox.checked) {
    //shuffle letters and reduce the length to the password length the user choosed
    lowerletters = alphabets()
      .repeat(4)
      .toLowerCase()
      .split("")
      .sort(function () {
        return 0.5 - Math.random();
      })
      .join("")
      .slice(0, passwordLengthRange.value);
    generatedPassword += lowerletters;
  }

  // Add uppercase letters to generatedPassword if the option is checked.
  if (uppercaseCheckbox.checked) {
    // shuffle letters and reduce the length to the password length the user selected.
    upperletters = alphabets()
      .repeat(4)
      .split("")
      .sort(function () {
        return 0.5 - Math.random();
      })
      .join("")
      .slice(0, passwordLengthRange.value);
    generatedPassword += upperletters;
  }
  // Add numbers to generatedPassword if the option is checked.
  if (numbersCheckbox.checked) {
    //shuffle numbers and reduce the length to the password length the user selected.
    numbers = numberList()
      .repeat(10)
      .split("")
      .sort(function () {
        return 0.5 - Math.random();
      })
      .join("")
      .slice(0, passwordLengthRange.value);
    generatedPassword += numbers;
  }
  // Add symbols letters to generatedPassword if the option is checked.
  if (symbolsCheckbox.checked) {
    //shuffle symbols and reduce the length to the password length the user selected.
    symbols = symbolList()
      .repeat(4)
      .split("")
      .sort(function () {
        return 0.5 - Math.random();
      })
      .join("")
      .slice(0, passwordLengthRange.value);
    generatedPassword += symbols;
  }

  // Get random words and hyphenate it if the option is checked.
  if (wordsCheckbox.checked) {
    //shuffle words and reduce the length to the password length the user selected.
    words = wordsList()
      .split(" ")
      .sort(function () {
        return 0.5 - Math.random();
      })
      .splice(0, passwordLengthRange.value)
      .join("-");
    generatedPassword = words;
  }

  // Exclude 0, 1, I, i, O, ., |, `, ' from the generated password if the option is checked
  if (similarCharactersCheckbox.checked) {
    generatedPassword = generatedPassword
      .repeat(4)
      .replace(/0|1|I|i|O|\.|\||`|'/gi, "");
  }

  // Exclude custom characters from the generated password if the exclude custom characters field is not empty
  if (doNotIncludeField.value !== "") {
    let excludeCharacters = doNotIncludeField.value.split("");

    // Escape the characters to be excluded to prevent regex errors
    excludeCharacters = excludeCharacters
      .map((character) => {
        // eslint-disable-next-line no-useless-escape
        return character.replace(/[-\/\\^$*+?.()|[\]{}]/g, "\\$&");
      })
      .join("|");

    generatedPassword = generatedPassword
      .repeat(4)
      .replace(new RegExp(excludeCharacters, "ig"), "");
  }

  if (!wordsCheckbox.checked) {
    // Shuffle final password and reduce the length to the password length the user selected.
    generatedPassword = generatedPassword
      .split("")
      .sort(function () {
        return 0.5 - Math.random();
      })
      .join("")
      .split("")
      .sort(function () {
        return 0.5 - Math.random();
      })
      .join("")
      .slice(0, passwordLengthRange.value);
  }

  // Set value of the text field to the generated password.

  if (wordsCheckbox.checked) {
    passfield1.value = generatedPassword;
  } else {
    passfield2.value = generatedPassword;
  }

  return;
}

if (form) {
  form.addEventListener("submit", generatePassword);
}

function toggleSiteLanguages(e) {
  e.target.parentElement.classList.toggle("active");
  return;
}

function toggleSiteLanguagesAlt(e) {
  e.target.classList.toggle("active");
  return;
}

if (langSwitch) {
  langSwitch.addEventListener("click", toggleSiteLanguages);
}

if (langSwitchSVG) {
  langSwitchSVG.addEventListener("click", toggleSiteLanguagesAlt);
}
(function () {
  setPasswordStrength(passwordLengthRange.value);
  generatePassword();
})();
