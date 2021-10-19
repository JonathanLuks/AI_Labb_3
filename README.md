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
