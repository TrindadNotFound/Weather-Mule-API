# Weather-Mule-API

Weather-Mule-API permite obter a temperatura de uma determinada cidade com base no seu nome.


## Como funciona?
A Weather-Mule-API executa dois HTTP Requests a dois endepoints destintos da WeatherAPI.

Num primeiro Request, é passado como parâmetro o nome da cidade que queremos consultar e a API Key da WeatherAPI.
Desse request, irá resultar um JSON Object condendo o nome da cidade traduzido em deversas linguas assim como os valores da latitude, longitude e a sigla do país a que pertence a cidade.

Para o segundo Request, é então utilizado os valores da longitude e da latitude obtidos no Request anterior para fazer uma nova chamada a um novo endepoint passando como parametros a latitude, a longitude e a API Key.

Como resposta iremos ter um novo JSON Object onde constam diversas informações sobre a temperatura que se faz sentir na cidade mencionada.


## Intalação
Numa primeira fase, é necessario proceder ao registo no site da WeatherAPI e obter a respectiva API Key.
De seguida, deve ser importado o ficheiro .zip do projeto mulesoft para o Anypoint Studio.
Após importação basta executar a API e proceder à chamada da mesma.


## Endpoint
Para procedermos à chamada da nossa API, usamos o endpoint **http://{host}:{port}/weather**. Para este endpoint passamos os parametros _'q'_ com o nome da cidade e o _'appid'_ com com a respetiva API Key.
Como resposta iremos obter o estado do tempo (um breve descrição) assim como a respetiva temperatura sentida.

![Screenshot_2](https://user-images.githubusercontent.com/75436524/190716308-c33afd60-ef7a-42af-a352-9d98fa6b2396.png)
