# 🧭 Trabalho U2T2 - Mapeamento de Rotas para Coleta Domiciliar

O Centro de Controle de Zoonoses de Natal é responsável por ações de vigilância e controle de doenças transmitidas por animais. Uma das atividades realizadas pelo órgão envolve a vigilância e o controle do mosquito Aedes aegypti através de uma estratégia que usa os ovitrampas (recipientes atrativos para as fêmeas do mosquito depositarem os seus ovos). Então, os agentes do CCZ selecionam pontos estratégicos para a instalação das ovitrampas e periodicamente visitam esses locais para coletar as palhetas com ovos, substituindo-as por novas.

O objetivo desse trabalho é desenvolver uma estratégia de mapeamento de rotas que otimize a distânci total percorrida por cada colaborador e distribua os pontos equitativamente entre os 10 colaboradores, considerando que cada agente parte da estação central, visita X casas e retorna para a estação.

### Responsável
- Celine Helena Abrantes de Andrade.  Matrícula: 20200078207.
- Gustavo Pereira de Carvalho. Matrícula: 20210039543.
- Matheus Bezerra Dantas Saraiva. Matrícula:

---

## 📁Estrutura do Repositório

No total, foram utilizadas três versões diferentes de um programa em Python para calcular as melhores rotas para o percurso de coleta das amostras pelos 10 agentes. Os códigos utilizados estão disponíveis na pasta `src` e implementam abordagens diferentes para calcular o caminho mais curto. A primeira versão utiliza o algoritmo A*, a segunda utiliza o algoritmo de Dijkstra e, finalmente, a terceira utiliza uma versão otimizada do Dijkstra com *min heap*.

Os mapas gerados pelos programas estão salvos na pasta `img`, na forma de imagens, além de serem apresentados junto dos resultados. Além disso, os prompts utilizados para gerar os códigos iniciais com a ajuda de ferramentas de LLM estão disponíveis no arquivo `LLM.md`.

---
## 🛠️ Desenvolvimento 

Os códigos iniciais foram gerados utilizando as ferramentas de LLM ChatGPT e Gemini 2.5 Pro. A partir desses códigos, foram feitas pequenas correções para que os programas funcionassem da forma desejada e, a partir daí, foram realizados testes, executando os programas no ambiente do Google Colab.

Como o trabalho foi desenvolvido voltado para a cidade de Natal-RN, foi necessário importar o mapa viário da cidade através da biblioteca OSMnx. Esse mapa, organizado na forma de grafo, pode ser manipulado através de funções disponíveis na biblioteca NetworkX.

A implementação do algoritmo A* utilizada foi a opção disponibilizada pela própria biblioteca NetworkX, junto de uma heurística Euclidiana. As versões com Dijkstra e *min heap* utilizam implementações próprias.

Ao fim da execução, os programas exibem métricas de desempenho, como tempo de execução e pegada de carbono — esta última calculada através da biblioteca CodeCarbon. Também são exibidas as distâncias percorridas por cada agente nas rotas calculadas e um mapa que mostra todas as rotas encontradas, a distância de cada uma e o trajeto total.

---
## 📊 Resultados

## Vídeo explicativo
🎥 [Link para o vídeo](https://www.loom.com/share)
