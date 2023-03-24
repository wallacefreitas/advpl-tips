# Uso do Return [**<div style="font-size:12px; float: right; height:40px; display: flex; align-items:center">Voltar</div>**](../../README.md)

Todo programa deve ter apenas um início e um fim, e com o AdvPL não é diferente. Prefira variáveis de controle a inserir Return no meio do código fonte e correr o risco de deixar de executar uma função importante para a rotina.

No exemplo abaixo corremos o risco de deixar de executar algum outro procedimento, em decorrência do _Return_ dentro do _msSeek_:
![](assets/images/return-no-meio-do-codigo.png)

Seu código deve ser linear, com apenas um _Return_:
![](assets/images/return-no-fim-do-codigo.png)
