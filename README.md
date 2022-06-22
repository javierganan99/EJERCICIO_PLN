# EJERCICIO_PLN

En este repositorio se modifica el trabajo presentado en el articulo **Bidirectional Recurrent Neural Network with Attention Mechanism for Punctuation Restoration** 
y públicamente disponible en https://github.com/ottokart/punctuator2 para generación de signos de puntuación. Las modificaciones principales que se hacen son:

- Se generan mayúsculas en la puntuación siempre después de un token de final de sentencia. Esta sección se incluye en el apartado 6 del notebook *EJERCICIO_PLN_FJGO.ipynb*.
- Se modifica el archivo de generación de datos *data.py* para incluir los signos de puntuación indicados en el enunciado.
- Se crea un archivo de tokenización diferente para *test* *train* y *val*. En *Tokenization_Test* se tokeniza teniendo en cuenta que no hay puntuación.
En *Tokenization_Model.py* se tokeniza convirtiendo todas las letras a minúscula para entrenar el modelo, que no considera las mayúsculas. En *Tokenization_Check.py*, 
sin embargo, se mantienen las mayúsculas porque en la evaluación del modelo estas se mantienen. 

Los pasos para probar la adaptación de este modelo al caso del ejercicio se incluyen en el apartado 6 del notebook *EJERCICIO_PLN_FJGO.ipynb*. 




**Referencia:**

TILK, Ottokar; ALUMÄE, Tanel. Bidirectional Recurrent Neural Network with Attention Mechanism for Punctuation Restoration. En Interspeech. 2016. p. 3047-3051.
