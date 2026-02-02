div class="container" id="container"> <div class="form-container sign-up">... </div> <div class="form-container sign-in">... </div> <div class="toggle-container">... </div> </div>container{

background-color: #fff;

border-radius: 30px;

box-shadow:

5px 15px rgba(0, 0, 0, 0.35);

position: relative;

overflow: hidden;

width: 768px;

max-width: 100%:

min-height: 480px;

.container p{

font-size: 14px;

line-height: 20px;

letter-spacing: 0.3px;

margin: 20px 0;

container span{

font-size: 12px;
const container = document.getElementById("container");

const registerBtn = document.getElementById("register");

const loginBtn = document.getElementById("login");

registerBtn.addEventListener("click", () { container.classList.add("active"); });

loginBtn.addEventListener("click", () { container.classList.remove("active"); });
