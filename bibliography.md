https://www.geeksforgeeks.org/pandas/how-to-count-distinct-values-of-a-pandas-dataframe-column/
https://www.statology.org/pandas-count-duplicates/ 
https://stackoverflow.com/questions/7359510/how-to-count-the-number-of-words-in-a-paragraph-and-exclude-some-words-from-a-f
https://support.webai.com/hc/en-us/articles/43174017684115-Embedding-Token-Limits
https://www.geeksforgeeks.org/data-analysis/how-to-chunk-text-data-a-comparative-analysis/
https://thelinuxcode.com/how-to-remove-html-tags-but-keep-contents-using-beautifulsoup/
https://www.geeksforgeeks.org/python/detect-an-unknown-language-using-python/
https://www.geeksforgeeks.org/python/how-to-drop-rows-that-contain-a-specific-string-in-pandas/
https://alicege005.medium.com/creating-a-simple-recommendation-system-based-on-tf-idf-and-counter-vectorizer-b3c91aa3aff0
https://numpy.org/devdocs/reference/generated/numpy.save.html


Models:
https://ai.google.dev/gemini-api/docs/embeddings?hl=es-419
https://huggingface.co/BAAI/bge-m3
https://huggingface.co/intfloat/e5-base-v2?utm_source=chatgpt.com
https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2?utm_source=chatgpt.com
https://developers.openai.com/api/docs/models/text-embedding-3-small?utm_source=chatgpt.com
https://developers.openai.com/api/docs/models/text-embedding-3-large?utm_source=chatgpt.com

Santi scores:
https://www.geeksforgeeks.org/machine-learning/recommendation-system-in-python/
https://www.datacamp.com/tutorial/recommender-systems-python

Si quisieramos usar TF-IDF o Word2Vec:
https://procodebase.com/article/best-practices-for-text-preprocessing-in-embedding-generation

Experimento para santi para ver q variante va mejor (chat):

    La forma de comprobarlo es pasar un disco muy famoso (ej. el Discovery de Daft Punk) por el modelo de embeddings usando las 3 variantes y calcular la Similitud del Coseno con el resto de discos.

    Santi puede mirar a "ojo" el Top 5 de recomendaciones que saca cada variante para ese disco:

    Si la Variante A recomienda otros discos de electrónica franceses de esa época. -> Funciona bien.

    Si la Variante B recomienda discos de Jazz o Rap solo porque casualmente tienen la misma nota (ej. 10.0) y salieron el mismo año. -> El metadato ha introducido ruido.

    Si la Variante C recomienda discos que tienen descripciones con palabras como "sintetizadores", "baile" y "voces robóticas" (aunque sean de otro año o nota). -> El modelo está entendiendo la semántica pura.