# MNIST-Experiments
Labb 3 i kursen AI-programmering

# Här är mina resultat hittils:

I den här filen ska ni beskriva:
- Era experiment
- Era slutsatser

### Convolutional (CNN):

#### Test #1:

```
Settings:    
    Epochs =            50    
    Learning Rate =     0.3  
    Batch Size =        64  
    Kernel Size =       (8, 8)
    Strides =           (1, 1)
    Layers =            2
    Neurons =           32
    
Results (Accuracy & Loss):
    Accuracy (Train & Validation):  1 & 0.9897
    Moved:                          23.74 Average
    Rotated:                        89.92 Average
    
    Loss (Train & Validation):      2.1445*10^-5 & 0.007792
    
    Time elapsed: 21 minutes 47 seconds
    
Anledning & Slutsats: Här försökte vi balansera slutsatserna utifrån föregående experiment för att hitta den bästa modellen.
Denna modell fick okej resultat men var väldigt långsam på att träna upp sig.
```



#### Test #2:

```
Settings:    
    Epochs =            50    
    Learning Rate =     0.35  
    Batch Size =        64  
    Kernel Size =       (8, 8)
    Strides =           (1, 1)
    Layers =            1
    Neurons =           16
    
Results (Accuracy & Loss):
    Accuracy (Train & Validation):  0.9963 & 0.9794
    Moved:                          21.01 Average
    Rotated:                        86.47 Average
    
    Loss (Train & Validation):      0.01093 & 0.1201
    
    Time elapsed: 2 minutes 15 seconds
    
Anledning & Slutsats: Här sänkte vi antalet layers & neuroner för att försöka snabba upp modellen. Vi ökade även LR för att se om resultaten blir bättre eller likadana.
Denna modell fick mycket sämre resultat, men var även mycket snabbare än föregående.
```



#### Test #3:

```
Settings:    
    Epochs =            50    
    Learning Rate =     0.40  
    Batch Size =        64  
    Kernel Size =       (8, 8)
    Strides =           (1, 1)
    Layers =            1
    Neurons =           32
    
Results (Accuracy & Loss):
    Accuracy (Train & Validation):  1 & 0.9875
    Moved:                          21.65 Average
    Rotated:                        90.17 Average
    
    Loss (Train & Validation):      2.9956*10^-4 & 0.06705
    
    Time elapsed: 2 minutes 57 seconds
    
Anledning & Slutsats: Här ökade vi antalet neuroner och LR för att se om vi kunde få ännu bättre resultat under ungefär likadan tid.
Denna modell fick mycket bättre resultat, dock var den lite långsammare.
Accuracy i Moved Data stannar runt 21 men i Rotated Data ökade Accuracy väldigt mycket. Loss blev även väldigt mycket lägre.
```



#### Test #4:

```
Settings:    
    Epochs =            50    
    Learning Rate =     0.4  
    Batch Size =        32  
    Kernel Size =       (8, 8)
    Strides =           (1, 1)
    Layers =            1
    Neurons =           64
    
Results (Accuracy & Loss):
    Accuracy (Train & Validation):  1 & 0.9866
    Moved:                          21.27 Average
    Rotated:                        89.29 Average
    
    Loss (Train & Validation):      8.0342*10^-5 & 0.0895
    
    Time elapsed: 5 minutes 22 seconds
    
Anledning & Slutsats: Vi dubblade antalet neuroner och halverade Batch Size för att se om resultatet kan bli ännu bättre under en kortare tid.
Denna modell fick sämre resultat i både Moved och Rotated Data. Den tog även nästan dubbelt så lång tid att köra igenom.
Loss under Train var dock en tiondel lägre än föregående modell.
```



#### Test #5:

```
Settings:    
    Epochs =            50    
    Learning Rate =     0.35
    Batch Size =        128  
    Kernel Size =       (8, 8)
    Strides =           (1, 1)
    Layers =            1
    Neurons =           32
    
Results (Accuracy & Loss):
    Accuracy (Train & Validation):  1 & 0.9877
    Moved:                          21.86 Average
    Rotated:                        89.97 Average
    
    Loss (Train & Validation):      8.7093*10^-4 & 0.05637
    
    Time elapsed: 2 minutes 59 seconds
    
Anledning & Slutsats: Här ville vi testa några andra slumpvalda värden utifrån föregående experiment för att se hur stor skillnad dem olika värdena gör.
Denna modell hade okej resultat. Accuracy i Moved Data var högst av alla modeller, men Accuracy i Rotated Data var ungefär lika. Loss var dock hyffsat låg.
Tiden spenderad var även runt genomsnittet.
```

#### Slutsats Experiment CNN:
Modellen i Test #3 gav oss bäst resultat när det gäller Accuracy och tid spenderad.





### Non-Convolutional (ANN):

#### Test #1:

```
Settings:    
    Epochs =            50    
    Learning Rate =     0.3  
    Batch Size =        64  
    Neurons =           32  
    
Results (Accuracy & Loss):
    Accuracy (Train & Validation):  0.994 & 0.9651
    Moved:                          15.54 Average
    Rotated:                        82.28 Average
    
    Loss (Train & Validation):      0.01946 & 0.2458
    
    Time elapsed: 23 seconds
    
Anledning & Slutsats: Här ville vi testa samma värden som med Convolutional för att få en grund att utgå ifrån.
Denna modell var väldigt dålig men väldigt snabb.
```


## Glöm inte!

Glöm inte att ha med figurer:

![TensorBoard download](fig/TensorBoardDownload.png "Glöm inte att kryssa i 'Show data download links' så att ni kan ladda ner era filer.")
