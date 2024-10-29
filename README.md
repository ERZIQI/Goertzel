# Conception dʼun émetteur acoustique par traitement récursif

**Objectif :**

Mis au point d’un émetteur acoustique qui détermine d’abord les canaux fréquentiels occupés par les autres émetteurs et, ensuite, émet un signal acoustique à un des canaux libres trouvés. La détection d’un canal se fera en utilisant l’algorithme de Goertzel. Les huit canaux utilisés par cet émetteur sont les suivants :

![image](https://github.com/user-attachments/assets/c172824f-c5bd-46eb-b2ad-cd62e20376f2)

Cet émetteur doit d’abord balayer le milieu marin pour déterminer les canaux déjà occupés par les 
autres émetteurs dans une portée de 500 m (Emission Cool Edit Pro entre 0 et -40 DB) et, ensuite, 
émet chaque seconde un pulse acoustique de largeur 10 ms et de fréquence un canal libre. Cet 
émetteur dont le schéma électronique est dans l’annexe, a été conçu dans les années 2000 en utilisant 
8 filtres analogiques et un microcontrôleur. Les inconvénients de cet émetteur sont le coût, la 
consommation, l’encombrement, … Nous souhaitons le moderniser en implémentant des solutions 
basées sur le traitement numérique du signal en utilisant le DSP. Plusieurs techniques peuvent être 
utilisées pour détecter les canaux occupés : Transformé de Fourier Rapide, Filtrage Passe Bande, 
Corrélation, Algorithme de Goertzel, ….
