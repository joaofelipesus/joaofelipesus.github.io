---
layout: post
title: "Por que aprender uma nova linguagem de programação?"
date: 2026-08-21
---

## Como escolhi a linguagem na qual trabalho

Bom, sou um rubista apaixonado pela linguagem desde a primeira vez em que vi os primeiros códigos em Ruby ainda na faculdade, na época trabalhava com Java e tinha algum conhecimento em PHP, era ok trabalhar com estas linguagens e aprender coisas novas mas algo ainda faltava para que pudesse descrever programar como sendo algo divertido. Um belo dia alguém me mostrou o lendário video do [blog em quinze minutos](https://www.youtube.com/watch?v=Gzj723LkRJY), e ali minha percepção sobre desenvolvimento de software mudou completamente.

Fiquei facinado em como era simples ser produtivo, e a sintaxe da linguagem permitia algo que ainda não tinha visto antes, o código fica com a cara de quem o escreveu e isso para mim possui uma conotação artistica, pois um desenvolvedor se expressa na forma de código e o Ruby permite me expressar de uma forma em que o código fica agradável. Ali comecei a estudar Ruby por conta, fazendo freelances e criando projetos pessoais para praticar, alguns destes projetos seguem em uso e venho mantendo ao longo dos ultimos sete anos. E depois de alguns anos consegui minha primeira vaga para trabalhar apenas com Ruby.

Desde então sigo estudando a linguagem e me aprofundando no uso do framework Ruby on Rails, lendo livros como [Programming Ruby](https://pragprog.com/titles/ruby5/programming-ruby-3-3-5th-edition/) e [Agile Web Development with Rails](https://pragprog.com/titles/rails8/agile-web-development-with-rails-8/), e praticando em novos projetos como [Bookfolks](https://bookfolks.io/pt/bookfolks-inicio/).

## Por que estudar uma nova linguagem?

Ao longo dos anos desenvolvi o hábito de estudar todos os dias, normalmente lendo um livro técnico e fazendo anotações no Obsidian ou praticando o que estudei nos ultimos dias, e este hábito funciona como uma espécia de terapia. Sou uma pessoa que gosta de rotina, e faz parte da minha rotina acordar por volta das sete horas da manhã, preparar um café e sentar no sofá da sala com meu notebook no colo para estudar por volta de quarenta minutos há uma hora, para então me arrumar e começar o dia de trabalho.

Nos ultimos anos trabalhei com linguagens como Python, JavaScript, e Elixir, mas nenhuma me deu a mesma sensação de quando uso Ruby para resolver algum problema. Mas queria aprendar uma nova linguagem para expandir meus conhecimentos e ver novas abordagens, e foi assim que escolhi a linguagem Go. Go é uma linguagem mais "quadrada", sem um framework como Rails ou Phoenix, no entando o que me chamou a atenção em Go foi o fato de que existe basicamente uma forma correta de fazer algo. É uma linguagem que não possui um apelo artistico, você não está tentando se expressar da forma mais compreensiva, o foco é resolver problemas de forma eficiente, sendo algo próximo de uma ferramenta.

Estava querendo algo realmente diferente de Ruby, e encontrei no Go este algo diferente.

## Dando os primeiros passos

Comecei lendo o livro [Programando em Go](https://www.casadocodigo.com.br/products/livro-google-go), e fiquei impressionado em como houveram poucos exemplos de código que ficaram depreciados, mesmo em um livro publicado em `06/2014`. Gostei do livro como introdução a linguagem, e comecei fazendo alguns projetinhos pequenos aqui e ali apenas para praticar o básico da sintaxe e sentir **a dor de aprender**.

<figure class="post-image">
  <img src="{{ '/assets/images/posts/2026-08-21-por-que-estou-estudando-go/bookfolks-programando-em-go.jpeg' | relative_url }}"
       alt="Tela do Bookfolks mostrando o livro Programando em Go finalizado, com avaliação cinco estrelas">
  <figcaption>O livro "Programando em Go" finalizado e avaliado no <a href="https://bookfolks.io/pt/bookfolks-inicio/">Bookfolks</a>.</figcaption>
</figure>

Em meus estudos, sigo me obrigando a usar LLMs apenas como fonte de pesquisa, não permitindo que gerem o código que faça o que eu quero pois quero **adquirir memória muscular**. Tenho a opnião que para aprender algo você precisa errar, testar, e debuggar o máximo possível, sofrendo um pouco no início mas sendo recompensado quando as coisas começam a funcionar. Aqui cabe um aviso, o código que escrevo para estudar é completamente diferente do que escrevo durante o trabalho, sou a favor do uso de LLMs e isso economiza bastante tempo e me torna mais produtivo pois sei o que estou fazendo na stack em que trabalho, no entando isso não é verdade quando você está aprendendo algo.

## Mais um livro e mais um projeto

Ao terminar o livro "Programando em Go" e praticar um pouco busquei um livro um pouco mais completo, agora pensando em focar em algo em que possa dar ganhos no meu dia a dia, e com isso iniciei a leitura do livro [Powerful Command-Line Applications in Go](https://pragprog.com/titles/rggo/powerful-command-line-applications-in-go/) pois tenho costume de criar scripts e pequenas ferramentas para facilitar me tornar mais produtivo. Apesar de este livro ser um pouco mais avançado, o autor da a base da linguagem e é uma leitura valiosa para quem está iniciando com a linguagem. No momento estou no campítulo quatro e estou achando o livro fantástico, ali aprendi manipulação de arquivos, me acostumei com o tratamento de erros, escrevi os primeiros testes automatizados, e tive uma base sobre o uso de interfaces. Futuramente publicarei meu resumo deste livro, mas fica o aviso que não será pequeno já que avancei até um terço do livro e meu resumo conta com 5.779 palavras até o momento.

Agora vamos para o caso prático, em um final de semana criei um [app para organizar minhas contas de casa](https://github.com/joaofelipesus/house-keep). Criei este projeto em rails pois ter uma visialização web é melhor neste caso, e também queria dar uso há meu [Raspberry Pi](https://www.raspberrypi.com/) e com isso consigo acessar o app em minha rede local.

Ao longo das semanas percebi que estava ficando chato fazer deploys ou consultar os logs para debugar o app, para fazer um novo deploy precisava me conecar via SSH com o raspberry py, e rodar os mesmos três ou quatro comandos para interromper o container, baixar o novo código, e iniciar o app novamente. Com isso pensei em usar o [kamal](https://github.com/basecamp/kamal) já que era um app rails, e a escolha fazia sentido, mas vi ali a oportunidade de criar minha própria ferramenta para gerenciar o app, e foi o que fiz na ultima semana durante minhas sessões de estudo.

<figure class="post-image">
  <img src="{{ '/assets/images/posts/2026-08-21-por-que-estou-estudando-go/cat-working.gif' | relative_url }}"
       alt="Gif de um gato digitando rapidamente em um teclado">
  <figcaption>Eu durante as sessões de estudo criando minha própria ferramenta.</figcaption>
</figure>

## O que o app faz e o que aprendi nesta ultima semana

Na ultima semana venho trabalhando no [maester](https://github.com/joaofelipesus/maester), uma referência aos meistres presentes nas Crônicas de Gelo e Fogo, já que os meistres são os responsáveis por entre outras tarefas gerenciar os castelos dos lordes. É um app simples que tem duas funcionalidades até o momento, sendo estas o download de um arquivo contendo os logs do app que é util para debug, e fazer o deploy de uma nova versão.

<figure class="post-image">
  <img src="{{ '/assets/images/posts/2026-08-21-por-que-estou-estudando-go/maestre.jpeg' | relative_url }}"
       alt="Um meistre das Crônicas de Gelo e Fogo, com seu colar de elos">
  <figcaption>Um meistre, responsável por gerenciar o castelo de seu lorde.</figcaption>
</figure>


Alguns rabiscos mais tarde comecei a ~~codar~~ me divertir criando as features.

<figure class="post-image">
  <img src="{{ '/assets/images/posts/2026-08-21-por-que-estou-estudando-go/rabiscos-maester.png' | relative_url }}"
       alt="Diagrama com o objetivo da ferramenta, o fluxo de execução de comandos via SSH da máquina de dev para o servidor, e os passos do deploy">
  <figcaption>Os rabiscos iniciais do maester: objetivo, comunicação via SSH e os passos do deploy.</figcaption>
</figure>

A seguir estão alguns dos principais aprendizados que tive durante o desenvolvimento da ferramenta.

#### É possível execurar comandos via SSH

Eu sabia que o comando SSH permitia se conecar com um outro computador, já fiz isso algumas vezes para deployar apps em meus primeiros trabalhos, mas nunca havia utilizado o SSH para executar comandos sem ficar "pendurado" em uma sessão.

Com isso modelei o `maester` para que executasse uma sequência de comandos SSH, os mesmos que eu executava sempre que precisava fazer um novo deploy. E mais legal, ao utilizar o SSH para executar um comando isolado este retorna a saída do comando executado o que permite exibir ou não as mensagens de log geradas durante a execução dos comandos para o usuário.

#### Geração de logs

Como todo bom dev backend gosto de ver os logs da aplicação em produção, o que foi util em algumas sessões de debug. Por padrão apps Rails não escrevem os logs em um arquivo, mas jogam os logs para a saída padrão STDOUT, e como a aplicação está rodando dentro de um container Docker pude adicionar a seguinte configuração  no docker-compose e com isso definir como os logs serão gerenciados.

```YAML
# total of 50MB of logs, been 10MB for each service
app:
    logging:
      driver: json-file
      options:
        max-size: "10m"
        max-file: "5"
```

Ao invés de criar algo ou re-inventar a roda apenas para acessar os logs utilizei o próprio comando do docker-compose que retorna os logs de um container dentro de uma janela de tempo.

```sh
docker compose -f docker-compose.yml -f docker-compose.prod.yml logs --since 2h app
```

Com isso ficou simples pegar a saída do comando que é executado via SSH e escrever em um arquivo na máquina que está executando o `maester`.

#### Comunicação entre máquinas

Gosto de estudar sobre comandos e ferramentas de terminal pois estas tornam possível simplificar tarefas e implementações, e antes de sair executando comandos em uma outra máquina é preciso certificar de que esta está responsiva, e com o servidor SSH ativo na porta padrão.

Apesar de poder tentar executar o comando SSH e caso este falhe sei que algo está errado, preferi dividir alguns passos para validar se a máquina que será acessada está apta a executar os comandos, e caso algo de errado sei qual é o problema.

Com isso, foram criadas duas etapas para verificação da disponibilidade da outra máquina, na primeira é executado o comando `ping` e caso este falhe pode ser que o Raspberry Py esteja desligado, ou eu esteja conectado em outra rede.

```Go
func PingServer(cfg config, createComand commandFactory) error {
	fmt.Printf("Start ping server on address %s\n", cfg.serverIP)

	cmd := createComand("ping", "-c", "1", cfg.serverIP)

	if _, err := cmd.CombinedOutput(); err != nil {
		return err
	}

	fmt.Println("Server ping [SUCCESS]")

	return nil
}
```

Caso o ping de certo faço a verificação se o SSH está funcionando na porta padrão, e para isso utilizei o comando `nc (netcat)` que serve para verificar se uma porta esta apta a receber conexões, assim consigo verificar se a máquina está respondendo na porta 22 que é a porta padrão do SSH.

```Go
// The command nc (netcat) is used for scan ports
func CheckSSHAvailable(cfg config, createCommand commandFactory) error {
	fmt.Printf("Start check SSH port on %s:22", cfg.serverIP)

	cmd := createCommand("nc", "-zv", cfg.serverIP, "22")

	if _, err := cmd.CombinedOutput(); err != nil {
		return err
	}

	fmt.Println("SHH check [SUCCESS]")

	return nil
}
```

#### Uso de interfaces em testes

Aqui vem a maior quebra de paradigma para um dev Ruby, estamos acostumados a escrever testes mockando a execução de métodos ou requests externas, no entanto em Go isso é feito utilizando interfaces e injeção de dependências.

Ao receber como argumento uma interface é possível utilizar tipos diferentes na implementação e nos testes desde que ambos implementem a mesma interface, uma interface que tenho utilizado bastante é a interface `io.Writer`. Com o uso de interfaces, posso definir um buffer ao invés de um arquivo durante a escrita do teste, e com isso ler o conteúdo e dar match com o valor esperado de forma simples.

```Go
func run(cfg config, createCommand commandFactory, outputFile io.Writer) { ... }
```

```Go
// uso em um teste

var mockWriter bytes.Buffer

run(cfg, createCommand, &mockWriter)

...

// verifica o conteúdo do buffer
if mockWriter.String() != string(expectedLogs) {
  t.Errorf("expected %q, got %q", expectedLogs, mockWriter.String())
}
```

## Conclusão

Considero o ato de aprender algo como sendo um bom uso de seu tempo, mesmo que não utilize esta nova habilidade profissionalmente no curto prazo é um bom exercício para manter o cérebro funcionando e quando **precisar algum assunto** sei os caminhos para estudar de forma mais eficiente.

Sinto que minha jornada no Go está apenas começando, não sei se irei utilizar Go profissionalmente ou apenas em meus projetos pessoais e de estudo, mas estou em paz com isso pois estou me divertindo bastante!

Por hoje é isso.
