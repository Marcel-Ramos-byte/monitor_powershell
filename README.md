# monitor_powershell
codigo em powershell visando monitorar um computador remoto sem acesso a internet

situação
computador em area remota isolado e sem acesso a redes
computador foi projetado para varias falhas mas não foi projetado para uma especifica que ocorre a cada 6000h por fim da vida util de um componente
não existe ponto para monitorar esse componente
existe preventiva no sistema completo, porem nao existe monitoramento desse componente

solução
substituir o componente uma vez
criar um script em powershell para enviar um POP UP na tela toda vez que estiver proximo da vida util, algo em torno de 4000h
esse script parte um contador de horas e registra essa contagem em um arquivo txt
o script inicia simplesmente pela criação de um arquivo de texto chamado startN.txt
a cada 4000h abre uma janela de aviso na tela, caso o usuario clique em ok inadvertidademente o contador emite novo alerta após 1h
contagem so reinicia após a criação de um novo start.
caso seja necessario auditar é possivel abrir o arquivo de log e verificar qual o tempo desde a ultima "substituição/criação de start"

esperado
como existe acesso de pessoas no local mensalmente, essa pessoa deverá ver se não há janelas de alerta e tambem verificar o arquivo de log e 
registrar em ordem de serviço o tempo registrado
caso haja mensagem deve ser aberto um pedido de substituição do componente.
diminuição de tempo de equipamento parado
monitoramento automatico e com registro de todas as substituições

