# Matching-Game
February 2, 2022: Today I am adding the file headers and the card interface for users of the game.  
#include <iostream>

using namespace std;
int main(){
  //declaring variables 
  char card[5][6]={{'a','c','e','B','D','g'},
  {'b','b','d','B','D'},{'c','a','f','C','F'},{'d','e','A','E','F'},{'f','A','E','C','g'}};

cout <<"       CHARACTER MATHING GAME  "<<endl;//title of game
//card game interafce
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;

return 0;
  }

February 3, 2022: Adding prompt lines 
  #include <iostream>

using namespace std;
int main(){
  //declaring variables 
  char card[5][6]={{'a','c','e','B','D','g'},
  {'b','b','d','B','D'},{'c','a','f','C','F'},{'d','e','A','E','F'},{'f','A','E','C','g'}};

cout <<"       CHARACTER MATHING GAME  "<<endl;//title of game
//card game interafce
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<endl;
cout << "|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<"|    |  "<<endl;
cout << "+----+  "<<"+----+  "<<"+----+  "<<"+----+  "<<"+----+  \n"<<endl;

//prompting game rules
cout << "This a character matching game. Choose two cards and the computer will determine \n if you have a match. In order to chose a card, input the row number and the colum number. "<<endl;

return 0;
}
