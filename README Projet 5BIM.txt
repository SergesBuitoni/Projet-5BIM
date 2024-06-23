
# Projet de Détection d'Objets avec YOLOv5 et OpenCV

Ce projet utilise le modèle YOLOv5 pour effectuer la détection d'objets en temps réel via la webcam de votre ordinateur.

## Prérequis

Assurez-vous d'avoir les logiciels et bibliothèques suivants installés sur votre machine :

1. Python 3.6+
2. OpenCV
3. NumPy
4. PyTorch
5. Les fichiers du projet

### Instructions pour installer les bibliothèques nécessaires :

Vous pouvez installer les bibliothèques nécessaires en utilisant pip :

```
pip install opencv-python-headless numpy torch torchvision torchaudio
```

## Instructions pour exécuter le projet

1. Clonez le dépôt de ce projet ou téléchargez les fichiers nécessaires.
2. Ouvrez un terminal ou un invite de commande dans le répertoire du projet.
3. Exécutez le script Python avec la commande suivante :

```
python nom_du_script.py
```

Remplacez `nom_du_script.py` par le nom réel de votre script Python (par exemple, `detection_objets.py`).

## Description du script

### `ObjectDetection` Class

Cette classe contient les méthodes pour charger le modèle YOLOv5, accéder à la webcam et annoter les images avec les résultats de détection.

- `__init__(self, model_name='yolov5s')` : Initialise le modèle YOLOv5.
- `access_camera(self)` : Accède à la webcam et effectue la détection d'objets en temps réel.
- `get_color(self, class_id)` : Retourne une couleur spécifique pour chaque classe d'objet.
- `annotate_frame(self, frame, results)` : Annote les résultats de détection sur l'image.

### `main()` Function

La fonction principale initialise une instance de la classe `ObjectDetection` et lance la détection en temps réel.

## Utilisation

- Le script accède à la webcam par défaut de l'ordinateur (index 0).
- La détection d'objets est effectuée en temps réel et les résultats sont annotés directement sur les images de la webcam.
- Pour arrêter l'exécution, appuyez sur la touche `q`.

## Remarques

- Assurez-vous que votre webcam fonctionne correctement et que les pilotes sont à jour.
- Vous pouvez modifier les paramètres de détection en ajustant les hyperparamètres du modèle YOLOv5.

## Exemple de sortie

Une fois le script exécuté, la fenêtre de la webcam s'affichera avec les objets détectés annotés en temps réel. Chaque objet détecté sera encadré et étiqueté avec son nom et son niveau de confiance.

## Support

Pour toute question ou assistance, veuillez contacter l'auteur du projet ou consulter la documentation des bibliothèques utilisées.
