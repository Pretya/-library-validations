# library-validations

function validateEmail(emailValue, pattern) {
  if(emailValue.match(pattern)) {
    return true
  } else {
    return false
  }
}
* emailValue - принимет значение инпута
* pattern - принимает регулярные выражения

___
function validateLogin(loginValue, pattern, minLength, maxLength) {
  if(loginValue.length < minLength || loginValue.length > maxLength) {
    return false;
  } else if(!loginValue.match(pattern) == true) {
    return false;
  } else {
    return true;
  }
}
* loginValue - принимет значение инпута
* pattern - принимает регулярные выражения
* minLength - минимальное количество значение при вводе
* maxLength - максимальное количество значение при вводе
___
function validatePassword(passwordValue, pattern) {
  if(pattern.test(passwordValue)) {
    return true;
  } else {
    return false;
  }
}

* passwordValue - принимет значение инпута
* pattern - принимает регулярные выражения
