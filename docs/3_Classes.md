### Aluno



- RF01, RF04, RF05, RF06, RF10



- idAluno



- nome



- cpf



- email



- telefone



- endereco



- rfid



- status



- matricular(plano: Plano), 



- realizarAgendamento(aula: Aula), 

  

- efetuarPagamento(), 



- visualizarTreino(), 



-consultarFrequencia(),



- visualizarAvaliacao():,



- consultarFrequencia()



### Plano



- RF01, RF02, RF04



- idPlano



- nome



- tipo



- valor



- ativo



- duracaoMeses: int



- calcularVencimento(): Date



- alterarPreco(novoPreco: double):



### Pagamento



- RF03, RF04, RF09



- idPagamento



- data



- valor



- formaPagamento



- status



- processarTransacao(): boolean



- gerarComprovante(): String



- registrar ()



- confirmar ()



- cancelar () 



### Acesso



- RF05, RF09



- idAcesso



- dataHora



- autorizado



- registrarEntrada(): void



- registrarSaida(): void



- validarAcesso(): boolean

### Aula



- RF06, RF07, RF09



- idAula



- nome



- horario



- capacidadeMaxima



-  verificarVagas(): boolean

  

-  CancelarAula(): void



- listarInscritos(): List



- agendar aula ()



### Agendamento



- RF06, RF10



- idAgendamento



- dataReserva



- status



- confirmar(): void

  

- cancelar(): void



### Presenca



- RF07



- idPresenca



- data



- presente



- registrar(): void



- justificarAusencia(motivo: String): 



### AvaliacaoFisica



- RF08, RF10



- idAvaliacao



- data



- peso



- imc



- percentualGordura



- observacoes



- anexo



- calcularIMC(): double



- gerarRelatorio(): String



### Notificacao



- RF10



- idNotificacao



- tipo



- dataEnvio



- status



- mensagem



- enviar(): void



- marcarComoLida(): void



### Instrutor



- RF07, RF08



- idInstrutor



- nome



- especialidade

  

- fazerLogin(): boolean



- baterPonto(): void



- ministrarAula(aula: Aula): 



- realizarAvaliacao(aluno: Aluno): 



- prescreverTreino(): void



### Recepcionista



- RF01, RF03



- idRecepcionista



- nome



- cadastrarAluno(aluno: Aluno):



- renovarPlano(aluno: Aluno): 



- venderProduto(): void



### Gerente



- RF02, RF09



- idGerente



- nome



- contratarFuncionario(f: Funcionario), 



- gerarRelatorioFinanceiro(), 



- configurarPrecos(p: Plano), 



- demitirFuncionario()
