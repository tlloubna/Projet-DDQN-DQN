# Projet DDQN-DQN  

Ce projet a été réalisé dans le cadre de mon master *Robotique et Perception Artificielle* à l’école **EUPi**.  

## Objectif  
L’objectif était d’analyser un article scientifique et d’illustrer le phénomène de **surestimation des Q-values** dans les algorithmes d’apprentissage par renforcement.  
Cette surestimation apparaît dans les grands espaces d’états, en raison des erreurs d’estimation qui s’accumulent lorsqu’on sélectionne systématiquement l’action maximisant la Q-value.  

##  Méthodologie  
- Implémentation initiale sur des environnements simples (**CartPole-v1**, **Acrobot-v1**) avec un réseau de neurones entièrement connecté (*fully connected neural network*).  
- Comparaison des performances de **DQN (Deep Q-Network)** et **DDQN (Double Deep Q-Network)**.  
- Extension aux jeux Atari nécessitant un traitement d’images : remplacement des couches entièrement connectées par des **couches convolutives (CNN)** pour extraire des caractéristiques visuelles pertinentes.  

##  Expérimentations  
- **Environnements simples** :  
  - CartPole-v1  
  - Acrobot-v1  

- **Jeux Atari (via la bibliothèque Gymnasium)** :  
  - Space Invaders  
  - Zaxxon  
  - Alien  

## Outils et bibliothèques  
- Python  
- Gymnasium  
- PyTorch / TensorFlow (selon implémentation)  

##  Résultats attendus  
- Mise en évidence de la surestimation des Q-values avec DQN.  
- Amélioration de la stabilité et des performances grâce à DDQN.  
- Validation sur des environnements de complexité croissante (du simple contrôle à la vision par CNN).  
