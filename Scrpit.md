## 🛢️ Script completo do programa

#include <stdio.h>

int main()
{
    float nota1, nota2, projeto_final, nota3, media, media_final;
    
    printf("Informe a 1ºNota: ");
    scanf("%f", &nota1);
    
    printf("Informe a 2ºNota: ");
    scanf ("%f", &nota2);
    
    printf("Informe a nota do projeto final: ");
    scanf("%f", &projeto_final);
    
    media = nota1 + nota2 + projeto_final;
    
    
    if (media >= 6.0) {
        
        
        printf("Parabéns, você passou de ano, pois tirou %4.2f.", media);
    }
    
    else {
        
        printf ("Você pode fazer a recuperação para conseguir nota, pois tirou %4.2f\n", media);
        
        printf("Informe a 3ºNota: ");
        scanf("%f", &nota3);
        
        if (nota1 > nota2) {
            
            media_final = nota1 + nota3;
        }
        
        else {
            media_final = nota2 + nota3;
        }
        
        
         if (media > media_final) {
             
             media = media_final;
             
         }
         
         if (media_final >= 6) {
             
             printf("Parabéns, você passou de semestre, pois tirou %4.2f", media_final);
             
         }
         
         else {
             printf ("Infelizmente você reprovou, pois tirou %4.2f", media_final);
         }
        
    }

    return 0;
}
