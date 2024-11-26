RCNN vs CNN :
Performance (Accuracy, F1 Score, Loss) :
Le RCNN surpasse le CNN sur toutes les métriques de performance. La complexité ajoutée par l'utilisation des blocs RPN dans le RCNN permet d'extraire des caractéristiques plus discriminatives, ce qui conduit à une meilleure classification.

Training Time :
Les deux modèles ont des temps d'entraînement similaires (environ 175-176 secondes), ce qui montre que le RCNN n'ajoute pas une surcharge significative malgré son architecture plus complexe.
2. RCNN vs CNN vs Vision Transformer (ViT):
Performance (Précision et F1 Score) :

Le modèle ViT atteint une précision de 96.84% et un F1 score de 0.9683, ce qui est inférieur aux performances de RCNN et CNN.
Le RCNN obtient les meilleures performances avec une précision de 99.22% et un F1 score de 0.9922, suivi par le CNN avec 98.25% de précision et un F1 score de 0.9826.
La performance de ViT est donc moins bonne que celle des modèles CNN et RCNN, probablement en raison de la simplicité du dataset MNIST. Les modèles basés sur les convolutions sont mieux adaptés à ce genre de tâche simple, tandis que les Vision Transformers nécessitent généralement plus de données et des tâches plus complexes pour révéler leur plein potentiel.
Perte Moyenne :

La perte moyenne de ViT est 0.1100, ce qui est plus élevé que celle de RCNN (0.0315) et CNN (0.0664). Cela montre que ViT a eu plus de difficultés à minimiser la fonction de perte pendant l'entraînement, ce qui est cohérent avec sa performance moins bonne.
Temps d'Entraînement :

Le temps d'entraînement pour ViT est beaucoup plus long (1718.21 secondes) par rapport à RCNN et CNN, qui ont pris environ 176 secondes chacune.
Ce temps d'entraînement plus long est dû à la complexité du modèle ViT, qui utilise des mécanismes d'attention globale (self-attention) plus coûteux en termes de calcul, en particulier lorsqu'il est formé à partir de zéro. De plus, ViT nécessite souvent des jeux de données plus vastes et des préformations pour être efficace, ce qui n'est pas le cas sur MNIST

Au cours de ce laboratoire, j'ai acquis une bonne compréhension des différentes architectures de réseaux neuronaux et de leur utilisation dans la classification d'images, en particulier sur le jeu de données MNIST.
Ce laboratoire m’a permis de me familiariser avec différentes architectures de réseaux neuronaux pour la vision par ordinateur en utilisant PyTorch. J'ai conçu et entraîné un modèle CNN pour classifier le dataset MNIST, puis comparé ses performances à celles du modèle Faster R-CNN pour la détection d'objets. J’ai également exploré les Vision Transformers (ViT) pour comprendre leur fonctionnement et leurs applications en classification d'images. Enfin, j’ai travaillé sur l’apprentissage par transfert avec des modèles pré-entraînés comme VGG16 et AlexNet, ce qui m’a permis d’améliorer les performances et d’accélérer l’entraînement des modèles.
