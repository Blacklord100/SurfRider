# SurfRider
Plastic Detection for an ONG

### File user guide *(I know it is messy ...)*
Bonjour, 

Je n'ai malheureusement pas le temps de up le projet complétement en lfs sur git. Cependant, je vous partage le lien de mon drive sur lequel tout les fichiers sont présent:

https://drive.google.com/open?id=13MSTvy-VsZqIuCTRbpcbMQBBGdPaaQiK


Ce readme vous permettra de vous retrouver parmi les différents fichiers:
*	SurfRider_Project_Turi.ipynb est le notebook coeur du projet
*	SurfRider_Project_Appendix_TACO_dataset.ipynb est un notebook permettant de transformer le dataset TACO en SFrame
*	SurfRidder_coreML_yolo_taco.mlmodel est le modèle finale après entrainement intégré dans ObjectDetection-CoreML_APP.app
*	ObjectDetection-CoreML_APP.app est le build issue de Xcode a faire tourner sur IPHONE. Il est basé sur le template Apple Breakfast
*	Les autres dossiers sont des backups des modèles et les datasets.
*	Rapport_video.mov est le rendu finale de 5 minutes. Il explique notre approche de manière succinte.
*	Les autres vidéos sont des extraits de notre application en réel 

Merci,

Author: Mithuran GAJENDRAN, Hugo MALLET


# HI ! SURFRIDER PROJECT

![](https://zupimages.net/up/19/09/1gz8.png)
![](https://raw.githubusercontent.com/m2dsupsdlclass/project-surfrider/master/imgs/surfrider.png)

* This course project makes use of an ongoing open source project led by Surfrider Europe, which aims at quantifying plastic pollution in rivers through space and time. Plastic Waste in oceans mostly comes from rivers (80%), and it is very difficult to assess precisely where they come from. This will be used to monitor river banks to take local decisions, measure effectiveness of policies at local and global scales, and has thus a very concrete importance.
* In practice, video streams are captured on river banks from kayaks (with their geolocalisation), and then fed to a model which aims at quantifying the number and types of objects. 
* Our goal is to build a short project around plastic detection using modern Deep Learning algorithms and also **provide ideas to tackle this issue**.

We both are trying to reduce our ecological footprint and are engaged in environmental issues. Moreover, we fancy kayaking too. 

Therefore, rather than implementing a model straight away, **we decided to brainstorm**. These are the keypoints we found interesting:
* In rough water, this mission would be inefficient as the plastic would be moving fast, we considered kayaking only calm water. What do we usually have ? Our smartphones !
* People tend to kayak for leasure purpose: they park there car at spot A, enjoy their adventure till point B before heading back to point A. In other words, rather than feeding a model afterwards, they could be feeding the model while reaching point B. Then the algorithm will focus them to the dirtiest area while they are heading back to point A. 
* While kayaking, we tend to put our cells on airplane mode to reduce battery consumption. 

Having considered the aforementionned keypoints, and having iPhones, we decided to build a solution that would work on Apples ecosystem.

### Aim:
* Use Deep Learning algorithm/methods to maximize our performance in detecting objects.
* Do it on IOS ecosystem
* Provide a different point of view to tackle this plastic issue that seems to be more efficient ( according to our thoughts ahaha ! )
