**ERG signal processing**

we used mapping to make different diagnosis normal and abnormal

we made a datarfame contain label(0 for normal and 1 for abnormal), patient id and signal type

transform signal using wavelet transorm (ricker) for each type of signal 
( sr, pr , mr)

the transformed images saved in directory and then we made augmentation to increase samples and saved them iv csv file

the data splitted 80% training, 10% validation and 10% test

we made a data generator for entering the data to the model to be able to train with learning rate = 0.001, epochs =10 and batch sie=32
model architecture(ResNet-50), accuracy reached 62% in model fit
