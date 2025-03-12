let secretNumber = Math.trunc(Math.random()*20) + 1;

let score = 20;
let highscore = 0;

document.querySelector('.check').addEventListener('click',function() {
    const guess = Number(document.querySelector('.guess').value);
    if(!guess){
        document.querySelector('.message').textContent='   No Number...';

    }  
         
    else if(guess===secretNumber){ //  The Guess Is Correct
        document.querySelector('.message').textContent = 'Correct Guess';
        document.querySelector('.number').textContent=secretNumber;
        document.querySelector('.game').textContent= 'You Won The Game 🏆'
        document.querySelector('body').style.backgroundColor = '#60b347';
        document.querySelector('.number').style.width ='30rem';
        if(score>highscore) {
            highscore=score;
            document.querySelector('.highscore').textContent = highscore;
        }
    }
         
    else if(guess>secretNumber){ // The Guess Is Greater Than SecretNumber
        if(score>1){
        document.querySelector('.message').textContent = ' 📈 To High';
    score--;
    document.querySelector('.score').textContent = score;
        }
    else {
        document.querySelector('.message').textContent = ' 💥 You Lost The Game';
        document.querySelector('.score').textContent = 0;
        
    }}
      
    else if(guess<secretNumber){     // The Guess Is Less Than SecretNumber
        if(score>1){
        document.querySelector('.message').textContent = ' 📉 To Low';
    score--;
    document.querySelector('.score').textContent = score;
        }
    else {
        document.querySelector('.message').textContent = '💥 You Lost The Game';
        document.querySelector('.score').textContent = 0;
        
    }}


})
 
document.querySelector('.again').addEventListener('click',function(){ // To Reset Or Play The Game Again Where The Highscore Remain Same in Again Play
    score = 20;
  secretNumber = Math.trunc(Math.random()*20) + 1;
  document.querySelector('.message').textContent = 'Start Guessing';
  document.querySelector('.number').textContent = '?';
  document.querySelector('.guess').value = '';
  document.querySelector('body').style.backgroundColor='#003566';
      document.querySelector('.game').textContent= 'Guess My Number!';
  document.querySelector('.number').style.width='15rem';
  document.querySelector('.score').textContent=20;

})



