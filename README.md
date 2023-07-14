# News_country
Dada una noticia, ¿Es posible determinar de que país proviene?. 

El conjunto consta de 3,250 noticias provenientes de Mexico, Chile, Peru, Argentina y España. Se comparan diferentes modelos para realizar un clasificador efectivo.
Se abarcan multiples herramientas de NLP, reducción de dimensión y clasificadores, igual de varios 

Train/val set de 2,250 noticias y 1000 para el conjunto de test.

Preprocesamiento: Se hace uso de la libreria NLTK para realizar las siguientes acciones:
  * remove all the special characters
  * remove all single characters
  * Remove single characters from the start
  * Substituting multiple spaces with single space
  * Removing prefixed 'b'
  * Lemmatization
  * Converting to Lowercase

Modelos pre-entrenados
  * Distle BETO

Representaciones en baja dimesión:
  * PCA
  * Kernel PCA
  * MDS
  * $t-$SNE
  * Isomap

Ajuste de clasificadores:
  * Maquina de sorporte vectorial con multiples kernels
      *lineal
      * rbf
  * RandomForestClassifier
