# 🧠 Simulador de Escalonamento de Processos

Simulador interativo dos principais **algoritmos de escalonamento e paginação de memória** utilizados em sistemas operacionais.  
Desenvolvido com foco educacional, o projeto permite observar graficamente o comportamento de processos, prazos, trocas de contexto e alocação de memória em tempo real.

🔗 **Acesse online:** [GitHub Pages](https://lucasazoli.github.io/simulador-so/)

---

## 📘 Sobre o Projeto

O simulador permite criar, editar e remover processos com parâmetros configuráveis e executar diferentes algoritmos clássicos de **escalonamento de CPU** e **gerenciamento de memória**.

### 🧮 Algoritmos de Escalonamento Implementados
- **FIFO (First In, First Out)**
- **SJF (Shortest Job First)**
- **RR (Round Robin)** — configurável com *quantum* e *overhead*
- **EDF (Earliest Deadline First)** — prioriza processos com prazos menores

### 💾 Algoritmos de Paginação
- **FIFO (First In, First Out)**
- **LRU (Least Recently Used)**

O sistema também calcula o **tempo médio de resposta (Average Response Time)** e exibe um **diagrama de Gantt** com a execução dos processos.


## ⚙️ Como Executar Localmente

```bash
# Clone este repositório
git clone https://github.com/<seu-usuario>/<repositorio>.git

# Acesse o diretório
cd <repositorio>

# Abra o arquivo principal no navegador
start index.html
````

Não é necessário servidor local — o projeto utiliza apenas HTML, CSS e JavaScript puro.

---

## 🧩 Estrutura do Projeto

| Componente    | Descrição                                                       |
| ------------- | --------------------------------------------------------------- |
| `Process`     | Representa um processo (PID, tempo, deadline, chegada, páginas) |
| `Escalonator` | Implementa FIFO, SJF, RR e EDF                                  |
| `Memory`      | Gerencia a alocação de memória (FIFO / LRU)                     |
| `Queue`       | Estrutura auxiliar de fila para controle de execução            |
| `main.js`     | Lógica de interface e simulação                                 |
| `index.html`  | Página principal do simulador                                   |
| `style.css`   | Estilos e layout                                                |

---

## 📊 Exemplo de Configuração

| Processo | Tempo | Páginas | Deadline | Chegada |
| -------- | ----- | ------- | -------- | ------- |
| PID 01   | 5     | 4       | 10       | 0       |
| PID 02   | 3     | 2       | 8        | 2       |
| PID 03   | 9     | 6       | 13       | 0       |
| PID 04   | 11    | 3       | 26       | 5       |

---

## 🧮 Métricas Geradas

* Tempo médio de resposta (ART)
* Sequência de execução dos processos
* Indicação de sobrecargas (`S`) e tempos ociosos (`N`)
* Alocação e substituição de páginas na memória RAM e virtual

---

## 🧠 Tecnologias Utilizadas

* **JavaScript (ES6)**
* **HTML5**
* **CSS3**
* **DOM Manipulation**
* **GitHub Pages** (deploy)

---

## 👥 Colaboradores

Projeto desenvolvido em conjunto por:

* [**Dely Silva**](https://github.com/delysilva)
* [**Gabriel “Gabsizinio”**](https://github.com/gabsizinio)
* [**Lucas Azoli**](https://github.com/LucasAzoli)

---

## 📄 Licença

Este projeto está sob a licença MIT.
Consulte o arquivo `LICENSE` para mais informações.

---

## 💡 Futuras Melhorias

* Estatísticas visuais (gráficos de CPU e memória)
* Exportação dos resultados da simulação
* Interface reativa (React.js ou Vue.js)

---

> Projeto educacional desenvolvido para estudo e demonstração prática de **escalonamento de processos e gerenciamento de memória em sistemas operacionais**.
