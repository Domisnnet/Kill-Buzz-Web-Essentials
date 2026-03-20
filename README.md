<h2 id="sobre-o-projeto">1. 🦟 Mata Mosquito!</h2>

![Status do Deploy](https://img.shields.io/badge/Status-Online-brightgreen)
![Tecnologias](https://img.shields.io/badge/Tecnologias-HTML%20%7C%20CSS%20%7C%20JS%20%7C%20Bootstrap-blueviolet)
[![Licença MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/Domisnnet/Kill-Buzz/edit/main/LICENSE)

![Kill-Buzz](src/imagens/tela.png)

Em **Mata Mosquito**, seu objetivo é simples: eliminar o máximo de mosquitos que conseguir antes que o tempo acabe. Mas cuidado! A cada mosquito que escapar, você perde uma vida. Não deixe os mosquitos vencerem!
Prepare-se para testar seus reflexos neste divertido e desafiador jogo de ação!

---

## 📚 Tabela de Conteúdo

| 🎮 O Jogo | 🛠️ Técnico | 🤝 Comunidade |
| :---: | :---: | :---: |
| [![1. Sobre](https://img.shields.io/badge/1%20-%20Sobre-4CAF50)](#sobre-o-projeto) | [![5. Destaques](https://img.shields.io/badge/5%20-%20Destaques-607D8B)](#destaques-tecnicos) | [![9. Código](https://img.shields.io/badge/9%20-%20Código-795548)](#codigo-fonte) |
| [![2. Techs](https://img.shields.io/badge/2%20-%20Techs-2196F3)](#tecnologias-utilizadas) | [![6. Repositório](https://img.shields.io/badge/6%20-%20Repo-009688)](#codigo-fonte) | [![10. Créditos](https://img.shields.io/badge/10%20-%20Créditos-607D8B)](#créditos) |
| [![3. Jogar](https://img.shields.io/badge/3%20-%20Jogar-FF9800)](#como-jogar) | [![7. Contribuir](https://img.shields.io/badge/7%20-%20Contribuir-3F51B5)](#como-contribuir) | [![11. Licença](https://img.shields.io/badge/11%20-%20Licença-E91E63)](#licenca) |
| [![4. Regras](https://img.shields.io/badge/4%20-%20Regras-9C27B0)](#regras-do-jogo) | [![8. FAQ](https://img.shields.io/badge/8%20-%20FAQ-FFC107)](#faq) | [![12. Perfil](https://img.shields.io/badge/12%20-%20Perfil-212121)](#perfil-do-github) |

---

<h2 id="tecnologias-utilizadas">2. ⚙️ Tecnologias Utilizadas</h2>

| Camada | Tecnologias | Descrição |
| :--- | :--- | :--- |
| **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) | Estrutura e estilização do projeto. |
| **Lógica** | ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) | Manipulação dinâmica do DOM e lógica de jogo. |
| **UI/UX** | ![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white) | Layout responsivo e adaptável. |

---

<h2 id="como-jogar">3. 🎮 Como Jogar</h2>

| Passo | Ação |
| :---: | :--- |
| **1** | Escolha a dificuldade: **Normal** (1.5s), **Difícil** (1s) ou **Chuck Norris** (<1s). |
| **2** | Clique nos mosquitos que surgem aleatoriamente na tela. |
| **3** | Gerencie suas **3 vidas**. Se um mosquito sumir antes de você clicar, você perde uma vida. |
| **4** | Sobreviva por **15 segundos** para vencer a partida! |

---

🚀 Jogue Agora!</h2>

Clique no botão abaixo para iniciar o desafio no seu navegador no modo normal como padrão:

<div align="left">
  <a href="https://domisnnet.github.io/Kill-Buzz/app.html?normal" target="_blank">
    <img alt="Botão Iniciar Jogo" src="https://raw.githubusercontent.com/Domisnnet/Kill-Buzz/main/src/imagens/bot%C3%A3o.webp" height="70" width="70" />
  </a>
</div>

---

<h2 id="regras-do-jogo">4. 🧩 Regras do Jogo</h2>

O segredo para dominar o **Mata Mosquito** é o tempo de reação. Fique atento às diretrizes do duelo:

| Regra | Descrição |
| :--- | :--- |
| 🕒 **O Tempo** | Você tem exatamente **15 segundos** para sobreviver. O cronômetro decrescente dita o ritmo da partida. |
| ❤️ **As Vidas** | Você inicia com **3 vidas**. Se um mosquito desaparecer antes de ser clicado, você perde uma vida. |
| 🦟 **O Alvo** | Os mosquitos surgem em tamanhos e orientações aleatórias para testar sua percepção. |
| 🏁 **Vitória** | Se o cronômetro chegar a zero e você tiver ao menos uma vida, você vence! |
| 💀 **Derrota** | O jogo termina imediatamente se você perder todas as 3 vidas. |

### 📊 Níveis de Dificuldade
A velocidade de surgimento dos mosquitos define o seu desafio:
* 🟢 **Normal:** Mosquitos surgem a cada **1.5 segundos**.
* 🟡 **Difícil:** Mosquitos surgem a cada **1.0 segundo**.
* 🔴 **Chuck Norris:** Desafio extremo com surgimento em **menos de 1 segundo**.

---

<h2 id="destaques-tecnicos">5. 💻 Destaques Técnicos</h2>

Este projeto foca na manipulação pura do **DOM** (Document Object Model) e lógica procedural com JavaScript. Abaixo, os principais pilares da implementação:

### 📐 Posicionamento Randômico Inteligente
Para garantir que os mosquitos nunca saiam da área visível da tela, utilizamos o cálculo de coordenadas baseado na largura e altura da janela:
* Utilização de `window.innerWidth` e `window.innerHeight`.
* Função `Math.random()` combinada com `Math.floor` para gerar coordenadas X e Y dinâmicas.
* Tratamento de bordas para subtrair o tamanho da imagem do mosquito, evitando barras de rolagem indesejadas.

### 🔄 Ciclo de Vida do Elemento
Diferente de frameworks modernos, aqui o ciclo de vida é controlado manualmente:
1.  **Criação:** O elemento `<img>` é criado via `document.createElement`.
2.  **Estilização:** Aplicação dinâmica de classes CSS para tamanhos e lados aleatórios.
3.  **Remoção:** O elemento é removido automaticamente se não for clicado a tempo, disparando a lógica de perda de vida.

### 🚦 Gerenciamento de Estado de Vidas
O sistema de vidas alterna as imagens dos corações entre `coracao_cheio.png` e `coracao_vazio.png` através da manipulação do ID do elemento, garantindo feedback visual imediato ao jogador.

---

<h2 id="codigo-fonte">6. 🚀 Instalação e Configuração Local</h2>

Gostou da lógica do jogo? Sinta-se à vontade para explorar o código ou clonar o repositório:

```bash
# Clonar o repositório
git clone [https://github.com/Domisnnet/King-Domfy.git](https://github.com/Domisnnet/Kill-Buzz.git)

# Acessar a pasta
cd Kill-Buzz
```

---

<h2 id="como-contribuir">7. 🤝 Como Contribuir</h2>

Siga os passos abaixo para fortalecer este projeto:

| Fase | Ação | Link / Comando |
| :---: | :--- | :--- |
| **01** | **Fork** | [![Fork](https://img.shields.io/badge/-Fazer%20Fork-blue?style=flat-square&logo=github)](https://github.com/Domisnnet/Kill-Buzz/fork) |
| **02** | **Branch** | `git checkout -b feature/MinhaMelhoria` |
| **03** | **Commit** | `git commit -m 'feat: nova seção de álbuns'` |
| **04** | **Push** | `git push origin feature/MinhaMelhoria` |
| **05** | **PR** | [![Abrir PR](https://img.shields.io/badge/-Abrir%20PR-green?style=flat-square&logo=git)](https://github.com/Domisnnet/Kill-Buzz/compare) |

### 🐛 Encontrou um problema?
Se algo não estiver funcionando como esperado, não hesite em abrir um chamado:

[![Issues Abertas](https://img.shields.io/github/issues/Domisnnet/Kill-Buzz?style=flat-square&color=red&logo=github)](https://github.com/Domisnnet/Kill-Buzz/issues)
[![Report Bug](https://img.shields.io/badge/Reportar-Erro-critical?style=flat-square&logo=github)](https://github.com/Domisnnet/Kill-Buzz/issues/new)


---

<h2 id="faq">8. 🧠 Perguntas Frequentes</h2>

<details>
<summary><strong>Como faço para reiniciar o jogo ❓</strong></summary>
<p>🔄 <strong>Resposta:</strong> É simples! Ao final de cada partida, uma tela de <strong>Vitória</strong> ou <strong>Game Over</strong> será exibida. Basta clicar no botão centralizado para reiniciar o cronômetro e as vidas.</p>
</details>

<details>
<summary><strong>O que acontece se eu deixar um mosquito escapar ❓</strong></summary>
<p>🚫 <strong>Atenção:</strong> Cada mosquito que desaparece antes do seu clique consome <strong>1 ponto de vida</strong>. O coração no topo da tela mudará de cheio para vazio. Ao perder os 3 corações, o jogo termina.</p>
</details>

<details>
<summary><strong>O jogo funciona em dispositivos móveis ❓</strong></summary>
<p>📱 <strong>Sim!</strong> O projeto foi desenvolvido com <strong>Bootstrap</strong> para ser responsivo. Os mosquitos se adaptam ao tamanho da tela do seu celular, permitindo que você jogue usando o toque (touch).</p>
</details>

<details>
<summary><strong>Como a dificuldade é calculada ❓</strong></summary>
<p>⚡ <strong>Lógica:</strong> A dificuldade altera o <code>intervallo</code> de surgimento dos mosquitos via JavaScript. No modo <strong>Normal</strong> você tem 1.5s para reagir, enquanto no modo <strong>Chuck Norris</strong> esse tempo cai drasticamente.</p>
</details>

<details>
<summary><strong>Como entro em contato com o desenvolvedor ❓</strong></summary>
<p>Adoramos receber sugestões para novos níveis ou temas! Utilize os canais abaixo:</p>
<strong>👨‍💻 Networking e Contato:</strong><br>
<a href="https://github.com/Domisnnet">
  <img src="https://img.shields.io/badge/Meu_Perfil_GitHub-212121?style=for-the-badge&logo=github" alt="Perfil">
</a>
</details>

---

<h2 id="codigo-fonte">9. 💻 Código Fonte</h2>

Gostou do jogo? Explore o código ou faça sugestões:

[![Repositório](https://img.shields.io/badge/Repositório-Domisnnet%2FKill--Buzz-blue?style=for-the-badge&logo=github)](https://github.com/Domisnnet/Kill-Buzz)

---

<h2 id="créditos">10. 📝 Créditos</h2>

* **Desenvolvedor: 👨‍💻 DomisDev**.
* **Imagens:** 🖼️ Originais do projeto.
* **Bibliotecas: 📚 Bootstrap**.
* **Objetivo:** 🎯 Projeto prático para estudo e manipulação de DOM.
* **Diversão:** 🎉 Divirta-se eliminando todos os mosquitos!

---

<h2 id="licenca">11. 📄 Licença</h2>

Este projeto é *open source* e está licenciado sob a [![Licença MIT](https://img.shields.io/github/license/Domisnnet/GitHub-Stats)](https://github.com/Domisnnet/Kill-Buzz/edit/main/LICENSE)

---

<h2 id="perfil-do-github">12. 👨‍💻 Perfil do GitHub</h2>

<a href="https://github.com/Domisnnet"> 
  <img src="src/imagens/DomisDev.png" width="120" alt="Acessar perfil GitHub"> 
</a>