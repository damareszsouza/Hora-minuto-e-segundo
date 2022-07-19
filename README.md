# Hora-minuto-e-segundo

Exercício 4: Hora, Minuto, Segundo
Gabarito do Exercício 4
Exercício 4: Faça uma sub-rotina que receba um único valor representando segundos. Essa função deverá convertê-lo para horas,  minutos e segundos. Todas as variáveis devem ser passadas como parâmetro, não havendo variáveis globais.

programa
{
    funcao inicio()
    {
        inteiro total, hora = 0, minuto = 0, segundo = 0
        escreva("Informe os segundos: \n")
        leia(total)
        tempo(total, hora, minuto, segundo)
        escreva("A soma é: ",hora,":", minuto, ":", segundo)
    }

    funcao tempo(inteiro t, inteiro &h, inteiro &m, inteiro &s)
    {
        h = t / (60*60)
        m = (t - (h*60*60))/60
        s = (t - (h*60*60))%60
    }

}
