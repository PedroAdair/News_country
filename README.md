# News_country
Dada una noticia, ¿Es posible determinar de que país proviene?. 

El conjunto consta de 3,250 noticias provenientes de Mexico, Chile, Peru, Argentina y España. Se comparan diferentes modelos para realizar un clasificador efectivo.
Se abarcan multiples herramientas de NLP, reducción de dimensión y clasificadores, igual de varios 

Train/val set de 2,250 noticias y 1000 para el conjunto de test.

Preprocesamiento: Se hace uso de la libreria NLTK para realizar las siguientes acciones:
  * Todas las noticias a 100 palabras (esto afecta en la precisioón del modelo, por cuestiones de hardware no se puede realizar con toda la longitud.)
  * remove all the special characters
  * remove all single characters
  * Remove single characters from the start
  * Substituting multiple spaces with single space
  * Removing prefixed 'b'
  * Lemmatization
  * Converting to Lowercase

Modelos pre-entrenados
  * Distle BETO: una versión es con los pesos congelados (reducir el coste computacional) y otra con todas las 

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

OBS: Se realizo con una MV de Coogle Colab Pro en la versión de RAM ampliada y con GPU disponible
