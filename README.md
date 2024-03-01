# Body-Action-From-iPhone-Motion-Data

![guy walking](https://media.licdn.com/dms/image/D5622AQH-XNQ3xKFUiw/feedshare-shrink_800/0/1705608480551?e=1712188800&v=beta&t=KT2JRq97I7i_j-axumQd6pf1DrV3X7FHWHqSMQkt4Zc)

This project implements the encoder side of the [Pytorch Transformer](https://pytorch.org/docs/stable/generated/torch.nn.Transformer.html) to train on and predict a user's body action from iPhone motion data. \
I used the [MotionSense](https://github.com/mmalekzadeh/motion-sense/tree/master/data) dataset, which is data from an iPhone 6's motion, gyroscope, and accelerometer. The available class outputs are:
- 0 : Walking Down Stairs
- 1 : Walking Up Stairs
- 2 : Walking Normally
- 3 : Jogging
- 4 : Sitting
- 5 : Standing

As you can see below, the model achieved over 85% F1 score
![](https://media.licdn.com/dms/image/D5622AQHxISYiaVx0CA/feedshare-shrink_800/0/1705608480654?e=1712188800&v=beta&t=zgnHZulfpcq_Y0K4J0nhwhJxqJ42n5KE4p41e4e3K4s)


The confusion matrix shows excellent results, with most tricky output being whether the user is walking up, down, or straight (several wrong outputs in the 0-3 section) but still a convincing majority correct.
![](https://media.licdn.com/dms/image/D5622AQG9rCxkDDYVKA/feedshare-shrink_800/0/1705608480831?e=1712188800&v=beta&t=awxIbi2iUCnYAmNY69BD_w8aNbz3fbITBuQ8K35hkBo)
