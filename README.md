# Javascript-Jquery-Code
Practice Code for Javascript and Jquery

// var firstName=prompt("Enter your First name");
// var firstletter=firstName[0];
// var f=false;
// var lastName=prompt("Enter your Last name");
// var lastLetter=lastName[0];
// var l=false;
// var yourAge=prompt("Enter your age");
// var a=false;
// var petName=prompt("enter ur pet name");
// var p=false;
// var yourHeight=prompt("enter your height");
// var h=false;
// var petLastChar=petName[petName.length-1];


// if(firstletter===lastLetter){
//     f=true;
// }
// else{
//     f=false;
// }


// if(yourAge>20&&yourAge<30){
//     a=true;
// }
// else{
//     a=false;
// }

// if(petLastChar==="y"||petLastChar==="Y"){
//     p=true;
// }
// else{
//     p=false;
// }

// if(yourHeight==170){
//     h=true;
// }
// else{
//     h=false;
// }

// if(f==l==a===p==h==true){
// console.log("you are a spy comrad")
// }
// else{
//     alert("you are a goood person, normal one");
// }


// function stringfunc(str,n){
//     var name="";
//     var i=0;
//     while(i<n){
//         name+=str;
//         i++;
//     }
//     return name; 
// }

// function makebricks(small,big,goal){
//     return goal%5>=0 && goal%5-small<=0 && small+5*big>=goal;
// }

// var awesome=["python","javascript","jango"];

// function addawesome(name){
//     alert(name+" is awesome");
// }

// awesome.forEach(addawesome);

// var roster=[];

// function addNew(){
//     var addname=prompt("Input the name you want to add?");
//     roster.push(addname);
// }

// function remove(){
//     var remName=prompt("What name do you want to remove?");
//     var index=roster.indexOf(remName);
//     roster.splice(index,1);
// }

// function edit(){
//     var editName=prompt("Input the name you want to edit?");
//     var newName=prompt("Input the name you want to add now?");
//     var index=roster.indexOf(editName);
//     roster[index]=newName;
// }

// function display(){
//     console.log(roster);
// }

// var start=prompt("would you like to start the app? y/n");
// var request="empty";

// if(start==='y'){
//     while(request!=="Quit"){
//         request=prompt("Please select an action add,delete,edit or display?");
//         if(request==='add'){
//             addNew();   
//         }
//         else if(request==='delete'){
//             remove();
//         }
//         else if(request==='edit'){
//             edit();
//         }
//         else if(request==='display'){
//             display();
//         }
//         else{
//             alert("Not recognized");
//         }
//     }
// }
// alert("thanks for using web app");


// var headingOne=document.getElementById("heading");
// var headingTwo=document.getElementById("headingTwo");
// var headingthree=document.getElementById("headingthree");

// headingOne.addEventListener('mouseover',function(){
//     headingOne.textContent="Mouse currently Over";
//     headingOne.style.color='red';
// })

// headingOne.addEventListener('mouseout',function(){
//     headingOne.textContent="Hover me"
//     headingOne.style.color='black';
// })


// headingTwo.addEventListener('click',function(){
//     headingTwo.textContent="clicked";
//     headingTwo.style.color='purple';
// })

// headingthree.addEventListener('dblclick',function(){
//     headingthree.textContent='I WAS DOUBLE CLICKED!';
//     headingthree.style.color='cyan';
// })

// heading.style.color='red';  

// function getRandomColour(){
//     var letters="0123456789ABCDEF";
//     var color="#";
//     for(var i=0;i<6;i++){
//         math=Math.random()*16;
//         color+=letters[Math.floor(math)];
//     }
//     return color;
// }

// function changeHeaderColour(){
//     colourInput=getRandomColour()
//     heading.style.color=colourInput;
// }

// setInterval("changeHeaderColour()",1000)





// //restart game button
// var restart=document.querySelector("#b");

// //grab all the squares
// var squares= document.querySelectorAll('td');

// //clear all the squares
// function clearBoard(){
//     for(var i=0;i<squares.length;i++){
//         squares[i].textContent='';
//     }
// }

// restart.addEventListener('click',clearBoard);

// var cellone=document.getElementById("cellOne");




// function changemarker(){
//     if(this.textContent===''){
//         this.textContent='X';
//     }
//     else if(this.textContent==='X'){
//         this.textContent='O';
//     }
//     else{
//         this.textContent=''
//     }
// }
// for(var i=0;i<squares.length;i++){
// squares[i].addEventListener('click',changemarker)
// }

//check the square marker


//For loop to add event listeners to all the squares

// $('h1').click(function(){
//     console.log("there was a click");
//     $(this).text("I was changed");
// })



// $('h1').dblclick(function(){
//     console.log("there was a click");
//     $(this).text("I was changed with double");
// })


//event toggle
// $('input').eq(0).keypress(function(event){
//     if(event.which===13){
//         $('h1').toggleClass('turnblue')
//     }
// })



//hoverovermouse

// $('h1').on('mouseenter',function(){
//     $(this).toggleClass('turnBlue');
// })



//SlideUp container Program

// $('button').on('click',function(){
//     $('.container').slideUp(3000)
// })

// var player1=prompt("Player one: Enter ur name, ur color will be blue");
// var player1Color='rgb(86,151,255)';

// var player2=prompt("Player one: Enter ur name, ur color will be red");
// var player1Color='rgb(237,45,73)';

// var game_on=true;
// var table=$('table tr');

// function reportWon(rowNum,colNum) {
//     console.log("You won starting at this row,col");
//     console.log(rowNum);
//     console.log(colNum);
// }

// function changeColor(rowIndex,colIndex,color){
//     return table.eq(rowIndex).find('td').eq(colIndex).find('button').css('background-color',color);
// }

// function returnColor(rowIndex,colIndex){
//     return table.eq(rowIndex).find('td').eq(colIndex).find('button').css('background-color');
// }

// function checkBottom(colIndex){
//     var colorReport=returnColor(5,colIndex);
//     for (var row = 0; row >-1 ; row--) {
//         colorReport=returnColor(row,colIndex);
//         if(colorReport==='rgb(128,128,128)'){
//             return row
//         }
//     }
// }


// function colorMatchCheck(one,two,three,four) {
//     return (one===two&&two===three&&three===four&&one!=='rgb(128,128,128)'&&one!==undefined)
// }

// function horizontalWinCheck() {
//     for (var row = 0; row < 6; row++) {
//         for (var col = 0; col < 4; col++) {
//             if(colorMatchCheck(returnColor(row,col),returnColor(row,col+1),returnColor(row,col+2),returnColor(row,col+3))){
//                 console.log('horiz');
//                 reportWon(row,col)
//                 return true;
//             }
//             else{
//                 continue;
//             }
//         }
//     }
// }

// function verticalWinCheck() {
//     for (var col = 0; col< 7; col++) {
//         for (var row = 0; row < 4; row++) {
//             if(colorMatchCheck(returnColor(row,col),returnColor(row+1,col),returnColor(row+2,col),returnColor(row+3,col))){
//                 console.log('Vertical');
//                 reportWon(row,col)
//                 return true;
//             }
//             else{
//                 continue;
//             }
//         }
//     }
// }

// //start with player one

// var currentPlayer=1;
// var currentName=player1;
// var currentColor=player1Color;




// $('h1').text(player1+" it is your turn, pick a column number to drop in!");

// $('.board button').on('click',function(){

//     var col=$('this').closest('td').index();

//     var bottomAvail=checkBottom(col);

//     changeColor(bottomAvail,col,currentColor);

//     if(horizontalWinCheck()||verticalWinCheck()){
//         $('h1').text(currentName+"you have won");
//         $('h3').fadeOut('fast');
//         $('h2').fadeOut('fast');
//     }

// })




//Class Program

class Person{
  constructor(){
    this.name='Max';
  }
  
  printMyName(){
    console.log(this.name);
  }
}

const person=new Person();
person.printMyName();




//Object Program with SPREAD and REST operator



var person={
  name:"Shayan",
  age:25
}

var newPerson={
  ...person,
  class:"4th year"
}

console.log(newPerson.age);

