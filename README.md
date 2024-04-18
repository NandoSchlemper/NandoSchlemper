<p align="center">
  <img height="50%" width="auto" src="https://github-readme-stats.vercel.app/api?username=NandoSchlemper&show_icons=true&count_private=true&theme=darcula&hide_border=true&hide=issues,contribs&bg_color=00500700">
  <img height="50%" width="auto" src="https://github-readme-stats.vercel.app/api/top-langs/?username=NandoSchlemper&layout=compact&hide_border=true&theme=darcula&bg_color=00000000&langs_count=6&hide=jupyter%20notebook,tex,css,php">
  <img height="50%" width="auto" src="https://github-readme-stats.vercel.app/api/top-langs/?username=NandoSchlemper&layout=compact&hide_border=true&theme=darcula&bg_color=00000000&langs_count=6&hide=jupyter%20notebook,tex,css,php&exclude_repo=Pacman-AI">
  <img src="https://github-readme-streak-stats.herokuapp.com?user=NandoSchlemper&theme=darcula&hide_border=true&background=FFFFFF00">
  <br>
  <br>
</p>
// ProjectSor
#include <stdio.h>
#include <string.h>

// %s = colocar str no print

char W1[] = "Boa noite! Seja bem vindo, digite START para continuar! \n > ";

char QQ[] = "Gostaria de usar um de nossos serviços? \n 1. YES \n 2. NO \n > ";

char Q1[] = "1. Mensagem motivacional \n 2. Melhor linguagem de programação \n 3. Carinha fofa \n 4. Mensagem desmotivacional \n 5. Sair do nosso serviço :,( \n > ";

int S1 = 1;
char response[10];
int response1;
int response2;

char start[] = "START";

int main() {
    printf(W1);
    scanf("%s", &response);
    
    int value = strcmp(response, start);
    
    if (value == 0)
    
        while (S1 == 1) {
            printf("%s", QQ);
            scanf("%i", &response1);
            
            if (response1 == 1) {
                printf("%s", Q1);
                scanf("%i", &response2);
                
                switch (response2) {
                    case 1:
                    printf("Dê seu melhor todos os dias, por mais que você possa achar que tudo vai dar de errado, ainda assim, tente seu melhor!! :D \n");
                    break;
                    
                    case 2:
                    printf("\n PoRtUgOl \n");
                    break;
                    
                    case 3:
                    printf("\n (ﾉ◕ヮ◕)ﾉ*:･ﾟ✧\n");
                    break;
                    
                    case 4:
                    printf("\n São nos dias ruins como esse, que temos a chance de darmos nosso melhor >:3 \n");
                    break;
                    
                    case 5:
                    printf("\n Tchau tchau... \n");
                    return S1 = 0;
                    break;
                    
                    default:
                    printf("\n d[o_0]b Mensagem computada não reconhecida d[o_0]b enviando usuário par ao inicio... d[o_0]b \n");
                }
                
            } else if (response1 == 2) {
                printf("Então ta :(");
                return S1 = 0;
            } else {
                printf("Opção computada não reconhecida, favor, inserir novamente o valor que deseja! Retornando para o estado de inicio... [┐∵]┘\n");
            }

                
            
        }
        
    else
        printf("Não se esqueça do Capslock...");
    
}
