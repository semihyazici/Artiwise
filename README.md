# Deep Learning Cheat Sheet

With this cheat sheet you will have a basic understanding of Deep Learning without getting involved math too much.Lets begin ,but first things first, what are the advantages and disadvantages of Deep Learning.
# Advantages and Disadvantages

![alt text](https://github.com/semihyazici/Artiwise/blob/main/adv_disadv_dl.PNG)
# Architecture
![alt text](https://miro.medium.com/max/700/1*3fA77_mLNiJTSgZFhYnU0Q@2x.png)

## Input Layer:
Where data enters the model, computers interst in only tensors so if your data is an image you should be flatten it into tensor.

## Hidden Layer:
Where all computations happens. 

## Output Layer:
Where you get desired outputs.


# Activation Function:
Activation functions where power of deep learning lies, for visualizing a simple image.

![alt text](https://miro.medium.com/max/700/1*5l08QfsUsrsOxcPzfDoStg.png)

As data get more distributed it is harder to fit on it for linear function, but non-linear function seems okey and difference is quite obvious.So basically it creates non-linearity.

![alt text](https://github.com/semihyazici/Artiwise/blob/main/act_fonk_table.PNG)

# Loss Function:

Also known as error function, it indicates the error between what model predicted and what it really is.So basically goal is minimizing the loss function.

## Mean Square Error(MSE):

![alt text](https://miro.medium.com/max/808/1*-e1QGatrODWpJkEwqP4Jyg.png)

It's often used for regression problems.MSE is great for ensuring that model has no outlier predictions with huge errors.

## Binary Cross Entropy Loss:

![alt text](https://cdn.analyticsvidhya.com/wp-content/uploads/2019/06/entropy.jpg1.jpg)

It's often used for binary classification problems.

## Multi-Class Cross Entropy Loss:

![alt text](https://cdn.analyticsvidhya.com/wp-content/uploads/2019/06/mce.jpg1.jpg)

It's often used for multi-class classification problems.

# Optimizing:

![alt text](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fblog.paperspace.com%2Fcontent%2Fimages%2F2018%2F05%2Fchallenges-1.png&f=1&nofb=1)

Optimizing is basically minimizing the loss with rearranging the weights.Assume that we are at the point A.What we are trying to achieve is finding the Global Minimum which rarely happens the reason why is we use derivative to minimize the loss.To visualize it we can think it as a mountain what we are trying to achieve is go to the surface.

![alt text](https://miro.medium.com/max/700/1*70f9PB-RwFaakqD6lfp4iw.png)

## Batch Gradient Descent:

Using all the data at once and updates them all at once.With this approach we can find the direct way to minimum and more data we got standard error becomes less.But this approach has its disadvantages because it uses all the data to update weights, if dataset is large it uses so much time to calculate new weights.So using Batch gradient descend with large dataset is not so efficient.

## Minibatch Gradient Descent:

Unlike batch gradient descend it doesn't use all the data at once but rather it uses batches.With this approach we no longer can find the direct way to minumum but also we no longer have to wait to all the data processed.In conclusion it's faster than batch gradient descend but paths it find is indirect.

## Stochastic Gradient Descent:

It learns on every example which makes it both fast and path to minumum is more noisy.It's better to use SGD for larger datasets.



