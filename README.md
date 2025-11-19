THIS IS A C PROGRAM TO CREATE TIC TAC TOE GAME
#include<stdio.h>
int main()
{
    int pos,moves=0;
    char ttt[9]={' ',' ',' ',' ',' ',' ',' ',' ',' '};
    char move='x';
    for(int i=1;1<=9;i++)
    {
        printf("enter the move: ");
        scanf("%d",&pos);
        ttt[pos]=move;
        moves++;
        printf("%c|%c|%c\n",ttt[0],ttt[1],ttt[2]);
        printf("--+--+--\n");
        printf("%c|%c|%c\n",ttt[3],ttt[4],ttt[5]);
        printf("--+--+--\n");
        printf("%c|%c|%c\n",ttt[6],ttt[7],ttt[8]);
        printf("--+--+--\n");
        if(move=='x')
        move='o';
        else
        move='x';
    if(ttt[0]=='x'&&ttt[1]=='x'&&ttt[2]=='x'||ttt[3]=='x'&&ttt[4]=='x'&&ttt[5]=='x'||ttt[6]=='x'&&ttt[7]=='x'&&ttt[8]=='x'||ttt[0]=='x'&&ttt[4]=='x'&&ttt[8]=='x'||ttt[0]=='x'&&ttt[3]=='x'&&ttt[6]=='x'||ttt[2]=='x'&&ttt[5]=='x'&&ttt[8]=='x'||ttt[2]=='x'&&ttt[4]=='x'&&ttt[6]=='x'||ttt[1]=='x'&&ttt[4]=='x'&&ttt[7]=='x')
       {
        printf("x wins,game over: ");
        break;
       }
        else if(ttt[0]=='o'&&ttt[1]=='o'&&ttt[2]=='o'||ttt[3]=='o'&&ttt[4]=='o'&&ttt[5]=='o'||ttt[6]=='o'&&ttt[7]=='o'&&ttt[8]=='o'||ttt[0]=='o'&&ttt[4]=='o'&&ttt[8]=='o'||ttt[0]=='o'&&ttt[3]=='o'&&ttt[6]=='o'||ttt[2]=='o'&&ttt[5]=='o'&&ttt[8]=='o'||ttt[2]=='o'&&ttt[4]=='o'&&ttt[6]=='o'||ttt[1]=='o'&&ttt[4]=='o'&&ttt[7]=='o')   
       {
           printf("o wins,game over: ");
           break;
       }
       
       else if(moves==9)
       {
           printf("tie");
           break;
       }
    }
    
        
    }
    



