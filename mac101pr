 
#include <iostream>
#include <string>
using namespace std;
int win ();          //a function to check if the user wins by looking if 3 signs are alligned
void drawTable (char SQ[]);    // this function is to draw a normal table
void updateTable (char SQ[], char sign, char Case);  //this function is to update the table and reprinting when the user choose a position
char SQ[10] = { '0', '1', '2', '3', '4', '5', '6', '7', '8', '9' };


int
main ()
{
  int choice, Case, Case2, check, player = 1;
  char sign, sign2;
  cout << "\t \t The Tic Tac Toe Game: \n";
  string player1, player2;
  cout << "Hello there, What's your name: \n";
  getline (cin, player1);
  cout << "And you are playing against? \n";
  getline (cin, player2);
  if (player % 2)
    {
      player = 1;          //this correspond to the string player1
    }
  else
    {
      player = 2;    //this correspond to the string player2
    }


  cout << endl;
  cout << player1 << " chose Your Symbol: \n\n";
  cout << "1 for X\n";
  cout << "2 for O\n";
  cin >> choice;


  switch (choice)             //swtich to let the user choose his preferable sign
    {
    case 1:
      cout << player1 << " You picked X\n";
      sign = 'X';
      cout << player2 << " you are O";
      sign2 = 'O';
      break;
    case 2:
      cout << player1 << " You picked O\n";
      sign = 'O';
      cout << player2 << " you are X \n";
      sign2 = 'X';
      break;
    default:
      cout << "Your choice is invalid.\n";
    }






  do
    {


      drawTable (SQ);
      cout << player1 << " enter a number:  ";
      cin >> Case;      //case is for player1
      updateTable (SQ, sign, Case);            //whenever a user enter a number update the table
      drawTable (SQ);
      check = win ();
      if (check == 1)
	{


	  cout << player1 << " you win ";
	  return -1;
	}


      cout << player2 << " enter a number:  ";
      cin >> Case2;    //case2 is for player2
      updateTable (SQ, sign2, Case2);




      check = win ();     //we need to put the win function inside a loop to it could runs everytime until there is a match
    }
  while (check == -1);
  if (check == 1)
    {


      cout << player2 << " you win ";
    }
  else
    {
      cout << " The grame is a draw.";
    }
}


void drawTable (char SQ[])
{
  cout << endl;
  cout << endl;
  cout << "     |     |     " << endl;
  cout << "  " << SQ[1] << "  |  " << SQ[2] << "  |  " << SQ[3] << endl;


  cout << "_____|_____|_____" << endl;
  cout << "     |     |     " << endl;


  cout << "  " << SQ[4] << "  |  " << SQ[5] << "  |  " << SQ[6] << endl;


  cout << "_____|_____|_____" << endl;
  cout << "     |     |     " << endl;


  cout << "  " << SQ[7] << "  |  " << SQ[8] << "  |  " << SQ[9] << endl;


  cout << "     |     |     " << endl << endl;


}


void updateTable (char SQ[], char sign, char Case)
{


  if (Case == 1 && SQ[1] == '1')
    {


      SQ[1] = sign;
    }
  else if (Case == 2 && SQ[2] == '2')
    {


      SQ[2] = sign;
    }
  else if (Case == 3 && SQ[3] == '3')
    {


      SQ[3] = sign;
    }
  else if (Case == 4 && SQ[4] == '4')
    {


      SQ[4] = sign;
    }
  else if (Case == 5 && SQ[5] == '5')
    {


      SQ[5] = sign;
    }
  else if (Case == 6 && SQ[6] == '6')
    {


      SQ[6] = sign;
    }
  else if (Case == 7 && SQ[7] == '7')
    {


      SQ[7] = sign;
    }
  else if (Case == 8 && SQ[8] == '8')
    {


      SQ[8] = sign;
    }
  else if (Case == 9 && SQ[9] == '9')
    {


      SQ[9] = sign;
    }
  else
    {
      cout << "Invalid move ";
      cin >> Case;
    }


}


int win ()
{
  if (SQ[1] == SQ[2] && SQ[2] == SQ[3])


    return 1;
  else if (SQ[4] == SQ[5] && SQ[5] == SQ[6])


    return 1;
  else if (SQ[7] == SQ[8] && SQ[8] == SQ[9])


    return 1;
  else if (SQ[1] == SQ[4] && SQ[4] == SQ[7])


    return 1;
  else if (SQ[2] == SQ[5] && SQ[5] == SQ[8])


    return 1;
  else if (SQ[3] == SQ[6] && SQ[6] == SQ[9])


    return 1;
  else if (SQ[1] == SQ[5] && SQ[5] == SQ[9])


    return 1;
  else if (SQ[3] == SQ[5] && SQ[5] == SQ[7])


    return 1;
  else if (SQ[1] != '1' && SQ[2] != '2' && SQ[3] != '3'
	   && SQ[4] != '4' && SQ[5] != '5' && SQ[6] != '6'
	   && SQ[7] != '7' && SQ[8] != '8' && SQ[9] != '9')


    return 0;
  else
    return -1;
}

