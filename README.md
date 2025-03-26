# Desenho-de-Coração-com-Turtle-e-Matem-tica
Este código utiliza a biblioteca Turtle e funções matemáticas para desenhar um coração na tela.

📜 Explicação do Código
Importação de Bibliotecas

math: Usada para cálculos matemáticos.
turtle: Utilizada para desenhar na tela.
Definição das Funções Matemáticas

hearta(k): Define a coordenada x do coração com base em funções trigonométricas.
heartb(k): Define a coordenada y do coração usando uma combinação de funções trigonométricas.
Configuração do Turtle

speed(0): Faz a tartaruga desenhar o mais rápido possível.
bgcolor("black"): Define o fundo da tela como preto.
Loop para Desenho do Coração

Um loop for com 6000 iterações calcula as coordenadas (x, y) usando as funções hearta e heartb.
goto(hearta(i)*20, heartb(i)*20): Move o cursor para a posição calculada, escalada por 20 para ampliar o desenho.
Um loop interno for j in range(5) parece não ter efeito prático, pois apenas define a cor como "red" repetidamente sem desenhar.
goto(0,0): Faz a tartaruga voltar para o ponto central a cada iteração, o que pode estar impedindo o desenho correto.
Finalização

done(): Finaliza a execução do Turtle.
🛠️ Problemas no Código
O uso do goto(0,0) dentro do loop faz com que a tartaruga volte sempre ao centro, impedindo que o coração seja desenhado corretamente.
O loop interno for j in range(5) é desnecessário, pois não afeta o desenho.
✅ Melhorias Sugeridas
Para corrigir o código e garantir que o coração seja desenhado corretamente:

Remover o goto(0,0).
Definir a cor antes do loop principal.
Usar penup() antes do primeiro goto() e pendown() após ele, para evitar linhas indesejadas.
