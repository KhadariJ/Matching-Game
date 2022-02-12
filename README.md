# Matching-Game
February 2, 2022: Today I am adding the file headers and the card interface for users of the game.  
#include <iostream>
#include <cstdlib>

using namespace std;
int main(){
  //declaring variables 
  char comma;
    int r1, c1, r2, c2, cards[5][5];
    srand((unsigned)time(NULL));
    //initialing array 
    for (int r=0; r<5; r++)
    {
        for (int c=0; c<5; c++)
        {
            cards[r][c]=rand()%9+0;
            cout <<" "<<cards[r][c];
        }
        cout<<endl;
    }
cout <<"\n";
    // board display
    cout<<" INTEGER MATCHING GAME "<<endl;
    cout<<"    1 2 3 4 5\n";
    cout<<"  ";
    for (int i=0; i<=10; i++)
    {
        cout<<"-";
    }
    cout<<endl;
    for (int r=0; r<5; r++)
    {
        cout<<r+1<<" | ";
        for (int c=0; c<5; c++)
        {
            cout<<"* ";
        }
        cout<<endl;
    }
    cout<<endl;
return 0;
  }

February 3, 2022: Adding prompt lines 
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;
int main(){
  //declaring variables 
  char comma;
    int r1, c1, r2, c2, cards[5][5];
    srand((unsigned)time(NULL));
    //initialing array 
    for (int r=0; r<5; r++)
    {
        for (int c=0; c<5; c++)
        {
            cards[r][c]=rand()%9+0;
            cout <<" "<<cards[r][c];
        }
        cout<<endl;
    }
cout <<"\n";
    // board display
    cout<<" INTEGER MATCHING GAME "<<endl;
    cout<<"    1 2 3 4 5\n";
    cout<<"  ";
    for (int i=0; i<=10; i++)
    {
        cout<<"-";
    }
    cout<<endl;
    for (int r=0; r<5; r++)
    {
        cout<<r+1<<" | ";
        for (int c=0; c<5; c++)
        {
            cout<<"* ";
        }
        cout<<endl;
    }
    cout<<endl;
               //selection
    cout<<"Please insert the first card row and column seperated by a comma.\n";
    cin>>r1>>comma>>c1;
    cout<<"Please insert the second card row and column seperated by a comma.\n";
    cin>>r2>>comma>>c2;
return 0;
  }

February 7, 2022: Revealing the selections
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;
int main(){
  //declaring variables 
  char comma;
    int r1, c1, r2, c2, cards[5][5];
    srand((unsigned)time(NULL));
    //initialing array 
    for (int r=0; r<5; r++)
    {
        for (int c=0; c<5; c++)
        {
            cards[r][c]=rand()%9+0;
            cout <<" "<<cards[r][c];
        }
        cout<<endl;
    }
cout <<"\n";
    // board display
    cout<<" INTEGER MATCHING GAME "<<endl;
    cout<<"    1 2 3 4 5\n";
    cout<<"  ";
    for (int i=0; i<=10; i++)
    {
        cout<<"-";
    }
    cout<<endl;
    for (int r=0; r<5; r++)
    {
        cout<<r+1<<" | ";
        for (int c=0; c<5; c++)
        {
            cout<<"* ";
        }
        cout<<endl;
    }
    cout<<endl;
     
    //prompt lines
    cout<<"Please insert the first card row and column seperated by a comma.\n";
    cin>>r1>>comma>>c1;
    cout<<"Please insert the second card row and column seperated by a comma.\n";
    cin>>r2>>comma>>c2;
    
    //revealing selections
    cout<<"    1 2 3 4 5\n";
    cout<<"  ";
    for (int i=0; i<=10; i++)
    {
        cout<<"-";
    }
    cout<<endl;
    for (int r=0; r<5; r++)
    {
        cout<<r+1<<" | ";
        for (int c=0; c<5; c++)
        {
            if ((r==r1)&&(c==c1))
            {
                cout<<cards[r][c]<<" ";
            }
            else if((r==r2)&&(c==c2))
            {
                cout<<cards[r][c]<<" ";
            }
            else
            {
                cout<<"* ";
            }
        }
        cout<<endl;
    }
return 0; 
  }

February 9, 2022: Verifying matches
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;
int main(){
  //declaring variables 
  char comma;
    int r1, c1, r2, c2, cards[5][5];
    srand((unsigned)time(NULL));
    //initialing array 
    for (int r=0; r<5; r++)
    {
        for (int c=0; c<5; c++)
        {
            cards[r][c]=rand()%9+0;
            cout <<" "<<cards[r][c];
        }
        cout<<endl;
    }
cout <<"\n";
    // board display
    cout<<" INTEGER MATCHING GAME "<<endl;
    cout<<"    1 2 3 4 5\n";
    cout<<"  ";
    for (int i=0; i<=10; i++)
    {
        cout<<"-";
    }
    cout<<endl;
    for (int r=0; r<5; r++)
    {
        cout<<r+1<<" | ";
        for (int c=0; c<5; c++)
        {
            cout<<"* ";
        }
        cout<<endl;
    }
    cout<<endl;
     
    //prompt lines
    cout<<"Please insert the first card row and column seperated by a comma.\n";
    cin>>r1>>comma>>c1;
    cout<<"Please insert the second card row and column seperated by a comma.\n";
    cin>>r2>>comma>>c2;
    
    //revealing selections
    cout<<"    1 2 3 4 5\n";
    cout<<"  ";
    for (int i=0; i<=10; i++)
    {
        cout<<"-";
    }
    cout<<endl;
    for (int r=0; r<5; r++)
    {
        cout<<r+1<<" | ";
        for (int c=0; c<5; c++)
        {
            if ((r==r1)&&(c==c1))
            {
                cout<<cards[r][c]<<" ";
            }
            else if((r==r2)&&(c==c2))
            {
                cout<<cards[r][c]<<" ";
            }
            else
            {
                cout<<"* ";
            }
        }
        cout<<endl;
    }
    if (cards[r1][c1]==cards[r2][c2])
    {
      cout <<"This is a match!";
    }
    else
    {
      cout <<"This is not match.";
    }
return 0; 
  }

February 12, 2022: Finalizing code
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;
int main(){
  //declaring variables 
  char comma;
    int r1, c1, r2, c2, cards[5][5];
    srand((unsigned)time(NULL));
    //initialing array 
    for (int r=0; r<5; r++)
    {
        for (int c=0; c<5; c++)
        {
            cards[r][c]=rand()%9+0;
            cout <<" "<<cards[r][c];
        }
        cout<<endl;
    }
cout <<"\n";
    // board display
    cout<<" INTEGER MATCHING GAME "<<endl;
    cout<<"    1 2 3 4 5\n";
    cout<<"  ";
    for (int i=0; i<=10; i++)
    {
        cout<<"-";
    }
    cout<<endl;
    for (int r=0; r<5; r++)
    {
        cout<<r+1<<" | ";
        for (int c=0; c<5; c++)
        {
            cout<<"* ";
        }
        cout<<endl;
    }
    cout<<endl;
     
    //prompt lines
    cout<<"Please insert the first card row and column seperated by a comma.\n";
    cin>>r1>>comma>>c1;
    cout<<"Please insert the second card row and column seperated by a comma.\n";
    cin>>r2>>comma>>c2;
    //fixing formating 
    r1--;
    c1--;
    r2--;
    c2--;
    
    //revealing selections
    cout<<"    1 2 3 4 5\n";
    cout<<"  ";
    for (int i=0; i<=10; i++)
    {
        cout<<"-";
    }
    cout<<endl;
    for (int r=0; r<5; r++)
    {
        cout<<r+1<<" | ";
        for (int c=0; c<5; c++)
        {
            if ((r==r1)&&(c==c1))
            {
                cout<<cards[r][c]<<" ";
            }
            else if((r==r2)&&(c==c2))
            {
                cout<<cards[r][c]<<" ";
            }
            else
            {
                cout<<"* ";
            }
        }
        cout<<endl;
    }
    //verifying matches
    if (cards[r1][c1]==cards[r2][c2])
    {
      cout <<"This is a match!";
    }
    else
    {
      cout <<"This is not match.";
    }
return 0; 
  }


