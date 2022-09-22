## 💻 Projeto
Back-end utilizado na semana do evento do projeto NLW-eSports da Rocketseat. Nele contém os endpoints utilizados para adicionar novos anúncios para encontrar seu duo, assim como também endpoints para selecionar os anúncios já feitos, jogos registrados no aplicativo e o discord da pessoa que fez o anúncio.


## ✨ Tecnologias

- [Node JS](https://nodejs.org/en/)
- [TypeScript](https://www.typescriptlang.org/)
- [Express](https://expressjs.com/pt-br/)
- [Prisma](https://www.prisma.io/)


## :hammer_and_wrench: Front-end da aplicação

Para você visualizar o projeto Front-end web. Acesse [esse link](https://github.com/rquartaroli/nlw-esports-web).

Para você visualizar o projeto Front-end mobile. Acesse [esse link](https://github.com/rquartaroli/nlw-esports-mobile).


## 🔖 Layout

Você pode visualizar o layout do projeto através [desse link](https://www.figma.com/file/zlBqt2zwmdhNWRCeN1i8dF/NLW-eSports-(Community)?node-id=6%3A23). É necessário ter conta no [Figma](http://figma.com/) para acessá-lo.


## Executando o projeto

Utilize o **npm install** para instalar as dependências do projeto.
Em seguida, inicie o projeto.<br/>

```cl
npm run dev
```

Caso queira visualizar as tabelas através do prisma studio,<br/>
**Execute esse comando em outro terminal:**<br/>
 
 ```cl
npx prisma studio
```

**Observação**: O servidor irá executar na porta 3333, caso queira alterar a porta, o local para isso se encontra no arquivo em **server.ts**.

## 🎏 EndPoints

- **Listar Games** <img alt="GET" src="https://img.shields.io/badge/-GET-blue">
```json
{
	"http://localhost:3333/games"
}
```

- **Listar Anúncio por Game** <img alt="GET" src="https://img.shields.io/badge/-GET-blue">
```json
{
	"http://localhost:3333/games/:idGame/ads"
}
```

- **Pegar Discord por Anúncio** <img alt="GET" src="https://img.shields.io/badge/-GET-blue">
```json
{
	"http://localhost:3333/ads/:idAnuncio/discord"
}
```

- **Criar Anúncio** <img alt="POST" src="https://img.shields.io/badge/-POST-brightgreen">
```json
{
	"http://localhost:3333/games/:idGame/ads"
}
```

Body: JSON
```json
{
	"name": "OneShot",
	"yearsPlaying": 4,
	"discord": "OneSHot#9999",
	"weekDays": [0, 1, 2, 3, 4, 5, 6],
	"hourStart": "18:00",
	"hourEnd": "23:00",
	"useVoiceChannel": true
}
```
<br />

**Recomendação**: Para executar as rotas, recomendo a utilização do [Insomnia](https://insomnia.rest/).


## 📄 Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

---

Feito por Rafael Quartaroli na semana do evento Next Level Week da [Rocketseat](https://rocketseat.com.br/).

<br />