const words = [
"PEDEXX WEAR",
"PREMIUM STREETWEAR",
"BUILT FOR THE BOLD",
"GHANAIAN FASHION"
];

let i = 0;
let j = 0;
let currentWord = "";
let isDeleting = false;

function typeEffect(){

currentWord = words[i];

if(!isDeleting){
document.querySelector(".dynamic-text")
.innerHTML =
currentWord.substring(0,j++);

if(j > currentWord.length){
isDeleting = true;
setTimeout(typeEffect,1500);
return;
}
}
else{
document.querySelector(".dynamic-text")
.innerHTML =
currentWord.substring(0,j--);

if(j === 0){
isDeleting = false;
i = (i + 1) % words.length;
}
}

setTimeout(typeEffect,isDeleting ? 50 : 100);
}

typeEffect();

function orderProduct(product){

const message =
`Hello PedexX Wear, I would like to order ${product}`;

window.open(
`https://wa.me/233256355743?text=${encodeURIComponent(message)}`,
"_blank"
);

}
