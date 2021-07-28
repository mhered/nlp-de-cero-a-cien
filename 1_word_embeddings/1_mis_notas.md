# Intro

## Spain AI

[spain-ai.com](http://www.spain-ai.com)

[@Spain_AI_](https://twitter.com/Spain_AI_)

webinars jueves

podcast [Lo que AI que oír](https://open.spotify.com/episode/1TwGzBcRCjUQn0SI8rEShK?si=yqzLj0XDSCm31d5dzFtLPQ).

## AI learners 

## 1er curso NLP en ES

* [@NLP_en_ES](https://twitter.com/NLP_en_ES)  

* transmisiones live 18:00 - 18:30 + 10' Q&A y [playlist en youtube](https://www.youtube.com/spainai) :
* 13 Jul: Introducción, contexto y Word Embeddings
* ~~27 Jul:~~ 03 Ago: Modelos secuenciales (RNNs, LSTMs) + caso práctico: clasificación de texto
* 10 Ag: Transformers I. Attention, arquitectura Transformer, sequence-to-sequence
* 24 Ag: Transformers II. Transfer learning + caso práctico: mejorar clasificación de texto
* 7 Sep: Transformers III. Encoder based, decoder based
* 21 Sep: Modelado del lenguaje: entrenar un LM con Hugging Face
* 5 Oct: Aplicación con FastAPI: NLP en producción

* GitHub repo: [https://github.com/nlp-en-es/nlp-de-cero-a-cien ](https://github.com/nlp-en-es/nlp-de-cero-a-cien)

* [Slack](https://bitly.com/nlp-en-es) 

​        ![Natural Language Processing with Transformers](https://learning.oreilly.com/library/cover/9781098103231/250w/)      

# Natural Language Processing with Transformershttps://www.oreilly.com/library/view/natural-language-processing/9781098103231/



# Notas 1a Sesion

word embedding un vector que representa una palabra, mapeados en tabla

tokenizar: separar en unidades (palabras of raiz + sufijo)

UNK token especial para embedding fuera de vocabulario

one-hot encoding: matriz con tantas columnas como palabras

No escala bien y no captura nada sobre el significado o contexto de las palabras 

word2vec

corpus: dataset of text

sliding window de 5 centrada en el token

calcula probabilidad de palabras en la ventana

optimiza por gradient descent ajustando los parametros

2 variantes: skip-gram predice el contexto dada una palabra central, 

continuous bag of words predice la palabra central dado el contexto

propiedades: los vectores word embedding son lineales!! 

semantico: espana-madrid + paris = francia!!

sintactico: reyes-rey + reina = reinas!!

Riesgo: propagar sesgos hombre a cura como mujer a prostituta

# Notas ejercicios

jupyter notebook edited in github thorugh collaboratory and saved in Drive

# Notas on [Speech and Language Processing (3rd ed. draft)](https://web.stanford.edu/~jurafsky/slp3/) 

Dan Jurafsky and James H. Martin

## Chapter 6

### Section 1

**lemma** or citation form es la raíz, may have several **wordforms** (e.g. declinations, verb tenses, gender and number endings etc)

a lemma can be **polysemous** i.e a word may have different meanings or **word senses** --> requires word sense **disambiguation**

**synonyms** are never exact

**word similarity**

**word relatedness** traditionally word association. Different types: by event (e.g. cup and coffee), opposites, part-whole, etc

**semantic field** set of words that cover a field and have structured relations. (see also **topic models**)

**semantic frames and roles**: set of words that denote perspectives or participants in an event, e.g. a sale can be framed from buyer, seller, goods, money etc

**connotations** (or affective meanings):aspects of meaning that express emotion. positive and negative evaluation are called **sentiment**

3 dimensions: valence (pleasentness) arousal (intensity of emotion) and dominance (degree of controlof stimulus)

### Section 2 

Vector semantics: represent words by vectors in multidimensional space (embeddings)

