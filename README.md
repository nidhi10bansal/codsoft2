# codsoft2
#include<iostream> //a prgrm that generates a random guess number and asks user to guess it.
#include<cstdlib>
#include<ctime>
using namespace std;
int main()
{srand(static_cast<unsigned int>time(0)); //the logic of random guess number
int randomnum = rand()%100+1;
int guess=0;
cout<<"Welcome to the game,mate!"<<endl;
cout<<"We have generated a random number guessing number 1 to 100.Please have fun with the game."<<endl;
while(true){
cout<<"Enter your guess number:"<<endl;
cin>>guess; //first we have to take input from the user then do the while loop and in while loop add if and else if for the right match for the users.
if(guess<randomnum){
cout<<"Nope, too low!Try again."<<endl;  //the guess is too low
} else if(guess>randomnum){
cout<<"Nope, too high!Trt again."<<endl;  //the guess is too high
}
else {
cout<<"Woohoo! Correct match="<<randomnum<<endl;  //right match
break;
}
}
return 0;
}


re
