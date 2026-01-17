# ⏳ Live Countdown (Contagem Regressiva)

Um projeto elegante de contagem regressiva para eventos ao vivo. Ideal para páginas de "Em breve", lançamentos de produtos ou anúncios de lives.



## 🚀 Tecnologias Utilizadas

Este projeto foi construído utilizando as melhores práticas de Front-end básico:

* **HTML5:** Estrutura semântica para os blocos de tempo (Dias, Horas, Minutos e Segundos).
* **CSS3:** Uso de **Flexbox** para alinhamento, filtros de fundo (`background-color` com opacidade) e tipografia personalizada via Google Fonts (Montserrat).
* **JavaScript (ES6):** Lógica matemática para conversão de milissegundos em unidades de tempo e atualização dinâmica da interface em intervalos de 1 segundo.

## 📋 Funcionalidades

- **Cálculo de Tempo Real:** Calcula a diferença entre a data atual e a data do evento.
- **Formatação Automática:** Adiciona um zero à esquerda em números menores que 10 (ex: `09`, `08`) para manter o design simétrico.
- **Interatividade:** Botão de "Cadastre-se" com efeito *hover* para engajamento do usuário.
- **Design Imersivo:** Fundo com imagem e sobreposição escura para garantir o contraste do texto.

## ⚙️ Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/countdown-live.git](https://github.com/seu-usuario/countdown-live.git)
    ```
2.  **Configuração da Data:**
    No arquivo `main.js`, altere a constante `dataEvento` para a data desejada:
    ```javascript
    const dataEvento = new Date ('2026-12-31 23:59:59');
    ```
3.  **Abrir o arquivo:**
    Abra o `index.html` em seu navegador preferido.

---

## 🛠️ Lógica de Tempo

O projeto utiliza cálculos baseados em segundos para distribuir o tempo restante:

| Unidade | Cálculo Lógico |
| :--- | :--- |
| **Dias** | `tempo / (60 * 60 * 24)` |
| **Horas** | `(tempo % (24 * 3600)) / 3600` |
| **Minutos** | `(tempo % 3600) / 60` |
| **Segundos** | `tempo % 60` |

---

## 📁 Estrutura do Repositório

```text
├── index.html    # Estrutura principal
├── style.css     # Estilização e responsividade
├── main.js       # Lógica da contagem regressiva
└── bg.jpg        # Imagem de fundo (certifique-se de ter esta imagem)
