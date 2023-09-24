# Simulacao_Elementos_Finitos
Utilizando de matrizes de rigidez e massa são calculados os deslocamentos, esforços e a vibração do sistema.

Para o funcionamento do software deve-se atribuir as coordenadas dos pontos nas matrizes nos_estaticos e nos_dinamicos, onde na primeira se atribuem as coordenadas dos ponto de apoio e na seguinte as demais, nesse software os pontos de apoio não possuem qualquer deslocamento ou rotação.

Essa matrizes em seguida serão unidas em uma matriz de coordenadas, seguindo uma ordem crescente onde os nos listados na matriz nos_estaticos vem primeiro, com menor numeração, digamos que de 0 a n-1 (para n nós), enquanto a númeração dos nos dinamicos será dada por n a m+n-1, para m nós.

Em seguida é necessario fornecer as conexões entre os nós na matriz ligacao_ref onde fornecendo o par de nos que se conecta e se deseja refinar, indicando o número de pontos intermediaros que se deseja implementar.

Um alerta que deixo aqui é que nesse codigo é considerado apenas extruturas cilindricas, se deseja utilizar outras estruturas, será necessario realizar algumas modificações adicionando a requisição de informar os momentos de inercia manualmente.
