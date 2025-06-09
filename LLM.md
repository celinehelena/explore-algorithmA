## Prompts Utilizados

Os prompts utilizados para gerar os códigos iniciais com a ajuda de ferramentas de LLM foram os seguintes:

### Implementação com A\*

> "Crie um código em Python que tenta otimizar rotas para agentes de zoonoses realizarem a coleta de amostras em pontos específicos.  
> O objetivo é ter rotas com a menor distância percorrida possível.  
> Temos 10 agentes para percorrerem 65 pontos.  
> Os agentes saem do centro de zoonoses em Natal/RN e percorrem os 65 pontos da cidade, cujas coordenadas estão descritas no arquivo `.csv` em anexo.  
> Cinco agentes devem visitar 6 pontos, e os outros cinco agentes devem visitar 7 pontos.  
> O programa deve utilizar o algoritmo A* para calcular as rotas e as bibliotecas OSMnx e NetworkX para obter e gerenciar o grafo que representa o mapa da cidade de Natal.  
> A saída deve exibir a distância percorrida por cada agente, o tempo de execução do programa e a pegada de carbono do programa, calculada com a biblioteca CodeCarbon.  
> Também mostre na saída um mapa com as rotas criadas e marcações no centro de zoonoses e nos pontos de coleta."

---

### Implementação com Dijkstra

> "Tenho 65 pontos distribuídos nas quatro zonas de Natal, que serão divididos entre 10 pessoas.  
> Cada colaborador parte da estação central (centro de zoonoses), visita X casas e retorna para a estação central.  
> Preciso criar uma estratégia de mapeamento de rotas, com 5 colaboradores visitando 6 casas e os outros 5 visitando 7 pontos.  
> No arquivo, estão disponíveis a latitude, longitude, bairro e zona de cada ponto.  
> Quero calcular as rotas usando uma implementação do algoritmo de Dijkstra tradicional (sem Min Heap).  
> Código utilizado na atividade anterior foi fornecido como base."

---

### Implementação com Dijkstra + Min-Heap

> "Pode fazer mais uma versão do código que utiliza o Dijkstra com Min Heap?  
> Código utilizado na versão anterior foi fornecido como base."
