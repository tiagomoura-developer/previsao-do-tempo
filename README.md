Consulta de Clima (aplicativo de clima)
Nesse projeto, eu dei um passo além e saí do ambiente isolado do navegador para consumir dados reais da internet. Desenvolvi um aplicativo de consulta climática que se conecta à API do OpenWeatherMap para buscar informações de qualquer cidade do mundo.

O que o projeto faz?
É simples e funcional:

Você digita o nome de uma cidade no campo de busca.

O app faz uma requisição assíncrona.

Se existir uma cidade, ele exibe o nome da cidade, do país, a temperatura atual em Celsius e um ícone ilustrativo que representa o tempo no momento (sol, nuvens, chuva, etc.).

Caso a cidade não seja encontrada, ele avisa o usuário com um alerta.

O que eu uso de técnico:
Fetch API & Async/Await: Essa foi a parte principal. Usei funções assíncronas para garantir que o aplicativo não "trave" enquanto espera a resposta da API.
Manipulação de JSON: Aprenda a navegar pelos objetos complexos que a API retorna para extrair exatamente o que eu preciso (como o código do país e o ícone do clima)
Tratamento de Erros: Implementei um try/catche uma verificação do cod 404para tratar casos onde o usuário digita uma cidade inexistente ou acontece algum problema na rede.
Codificação de URL: Usei o encodeURIpara garantir que nomes de cidades com espaços ou acentos não quebrem a requisição.
CSS Dinâmico: O container de informações começa escondido ( display: none) e só aparece via JavaScript quando os dados chegam, deixando uma interface mais limpa.
