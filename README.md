# Lighten Ghost(Kinect Game)
Video Link:https://youtu.be/0mk80QwWzaY 

Game Demo:https://youtu.be/NX_7Lh5U-Wo

## Idea development
![IMG_0669](https://git.arts.ac.uk/storage/user/588/files/ce94aa9e-8c46-45fb-a991-e86525503541)

During my travels, I can see different cemeteries in various cities. Some are bustling and some are depressed. In front of some tombstones, some are quiet and beautiful, and they are often cleaned there. And some tombstones are already full of dust, no one cares about them. I thought of the movie Coco. The world of the undead is connected with the real world. On the Day of the Dead, the dead will meet their family members. But what about the dead without family? Will they fade away because they are not remembered?
This reminds me of Chinese mythology. Chinese gods need human beings to keep offering and worshiping to survive and bless the world. But gods who are not worshiped and enshrined will go to death and exhaustion. So I plan to create such a character. He went to worship these undead souls who are about to disappear, so that they can still survive in the world of undead.

## Final Idea: Game rule
The dead lives still exist in this world, and their dead souls are still free. However, when the living gradually forget them, their souls will gradually be extinguished until they disappear. The Skeleton is the savior of the dead souls, and he is going to save these dying souls.
The skeleton man with the task needs to go to light up the dead souls that are about to be forgotten. Souls of the dead are scattered anywhere in the cemetery, especially in front of tombstones. Skeletons need to find them anywhere in the cemetery. When all the revenants are lit, the skeleton's mission is complete. The revenants are no longer forgotten, so they won't disappear.

## Neokinect & HTC Vive Controller
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 002](https://git.arts.ac.uk/storage/user/588/files/e4cb0e36-7d47-4784-b689-7a2eee8deef8)

https://www.unrealengine.com/marketplace/en-US/product/neo-kinect
Kinect is my main interactive device. There is a plug-in called Neo Kinect in UE5, which fully realizes the function of controlling game characters with body movements. It contains 5 functions of body tracking, face tracking, sensor control, remapping and frame texture. And I only need the body tracking function in it. In this model, I need to match the bones and joints of the character with my character to achieve manipulation. And I want to use HTC Vivi Controller to realize the operation of hand buttons. It's like a remote button. I can perform operations such as attacking by pressing the button on the controller.

## Technical test & Challenge
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 003](https://git.arts.ac.uk/storage/user/588/files/7e9e31a4-d200-4369-998f-3659369ee770)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 004](https://git.arts.ac.uk/storage/user/588/files/e4bfc100-7b30-48d0-b26c-0786992447a0)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 005](https://git.arts.ac.uk/storage/user/588/files/781f4f35-faa7-4aa6-82e2-a9cb99def339)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 006](https://git.arts.ac.uk/storage/user/588/files/cd06b1a3-927c-4963-a856-61249aebfba0)

I connected the Kinect V2 to the computer, tried its flexibility, and the effect is very good. This device can detect people's limbs very well, as well as the depth of field. So Kinect can identify all parts of the human body very well.

Then I combined it with Neo Kinect to test its feasibility. The effect is very good. The sensitivity of the characters is very good, like a mirror. In this plugin, there are a total of 6 character models. So my character can be added to 6. Of course, in my current game production, only one character model is needed.

![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 007](https://git.arts.ac.uk/storage/user/588/files/bb0c6a1e-19dc-4b4a-a93d-33021b4667cf)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 008](https://git.arts.ac.uk/storage/user/588/files/4d915f2f-4006-4304-a9ec-d2fee77b9ff7)

However, when I tested the HTC VIve Controller, the computer could not recognize the device. Although I changed the code for Steam VR to recognize the device, the handle does not work without the HMD.
Later, I used a USB connection, although Steam AR can recognize the handle, UE5 can't.
So I have to give up the interactive mode of the handle, leaving only Kinect. At the same time, I will no longer use the attack mode of the game, because there is no handle controller. I control the movement of the character through the movement of the body.

## Build Characters and Environments
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 009](https://git.arts.ac.uk/storage/user/588/files/c9fea897-2e7f-42aa-b848-740778707301)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 010](https://git.arts.ac.uk/storage/user/588/files/f69980af-8251-47c9-971d-39b6d078c6c1)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 011](https://git.arts.ac.uk/storage/user/588/files/e1f13472-e02c-4cda-8d72-e10e5e6e4184)

After I downloaded and modified the main character's model, I started adding skeletal meshes to it. Because this character will have a lot of motion animations later, I need to build the branch points of the body. I created bones in Blender. In order to make the skeleton faster, I used the Auto-Rig Pro plug-in. This can be used to create a skeletal mesh by positioning the jaw, shoulders, wrists, knees, and pelvis.

![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 012](https://git.arts.ac.uk/storage/user/588/files/c2ce6cb2-18ba-4c4c-8b56-1decdaa90fc0)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 013](https://git.arts.ac.uk/storage/user/588/files/1b210d4f-cc76-4107-9e08-0e779df9ad5e)

![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 014](https://git.arts.ac.uk/storage/user/588/files/096f581d-2f20-4ced-b158-8ba9cf0fe9b1)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 015](https://git.arts.ac.uk/storage/user/588/files/7308826e-3578-4f2f-9eeb-a4cda3aa43c9)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 016](https://git.arts.ac.uk/storage/user/588/files/20f524b9-e969-4658-96f8-896d2c6af27a)

![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 017](https://git.arts.ac.uk/storage/user/588/files/66c0919b-c44a-4dd4-a0fd-f6d202db1b12)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 018](https://git.arts.ac.uk/storage/user/588/files/c05e8a83-6b5f-44cc-b4dc-ec90c1101b8c)

I downloaded some models and put them together to make a game environment. Because ghosts and spirits appear, the background is a cemetery at night. I didn't set the sky light. But since there is no light, the character's back is dark. So I had to add a follower dim light behind the character, which can be seen by the audience but not very bright. At the same time, some streetlamps and candles are added on the road, which can guide the player in the direction to go. There are 3 levels in my game, one is the dark forest, one is the cemetery, and the other is the river on the other side. There are scattered forgotten tombstones in the dark forest. There are neat and crowded tombstones in the cemetery. The Bana River is the dividing line between the soul and the human world, and the soul will rest in peace if it crosses this river. So the Bana River is also the end point, where there are many Bana flowers.

## Animation and Movement
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 019](https://git.arts.ac.uk/storage/user/588/files/36646c2d-e762-46b0-94ad-1a03c1ee2ede)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 020](https://git.arts.ac.uk/storage/user/588/files/83fb56b9-be0f-40db-87e8-1a9b1337bebf)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 021](https://git.arts.ac.uk/storage/user/588/files/769b0466-6dd6-444f-b9c3-2cf416d1c10d)

Then I started to input animations and commands to the character. Through the character blueprint and animation blueprint, the character is given actions such as walking and jumping. And when there is no command, the character also has its own static state. I added a look around animation to him, which keeps the character always dynamic.

![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 022](https://git.arts.ac.uk/storage/user/588/files/41a9e354-a9a5-48d5-962e-3fb1d6371c4a)

However when I make my character do an animation, it can't go back to the original standing animation state. This is what has troubled me for a long time. Later, I found that after adding the command to control the time of the animation mode, the character will return to the initial state of the animation blueprint after the animation is played. So I added animations of characters worshiping the dead, victorious and losing.

![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 023](https://git.arts.ac.uk/storage/user/588/files/8479ad9d-8dbc-4ddd-9f68-17c056e1bf85)

So far, all my animations have been edited. As long as the operation control buttons are added, the game can be executed smoothly. Before adding the Kinect device, I connected the mouse and keyboard to test the integrity of the game. The effect is very good The next step is to link the character's actions to the Kinect's operating system.

## Movement with Kinect
Referring to the example given by Neo Kinect, I made the animation blueprint of my character (connected with Kinect). In particular, there is an option of "Interface" under "Add" in the blueprint. Here I need to select "Joints Transforms" in "Neo Kinect". Then connect to the Kinect device in the event blueprint.

![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 024](https://git.arts.ac.uk/storage/user/588/files/d29675c7-2b86-4d97-9778-fd833e0e121e)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 025](https://git.arts.ac.uk/storage/user/588/files/614a285f-7c9b-4859-b1cc-b4986948d90c)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 026](https://git.arts.ac.uk/storage/user/588/files/569cc778-de00-48ef-b8c6-73a419c50c57)

The most critical point after that is the settings in “AnimGraph”. Each item here is to make the body parts recognized in Kinect correspond to the body parts of the animated character in UE5, through the operation of "Joints Transforms". Mainly Spine, Left arm, Right arm, Left leg, Right leg, these 5 parts.

![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 027](https://git.arts.ac.uk/storage/user/588/files/3e56e0c8-63b5-44e8-9bb2-fa5f604cff73)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 028](https://git.arts.ac.uk/storage/user/588/files/d3c2a486-1ec1-424e-b1b9-d79d5d19c1fd)

Then I designed actions to control the character. The character has 5 actions in total: forward, left, right, flashlight, and Prey. The player only needs to raise the left and right arms to realize the operation. The forward operation is the player He kept raising his legs and walking on the spot. Then I input the operation into UE5, and then test it. The test is successful.

## Final test
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 029](https://git.arts.ac.uk/storage/user/588/files/16f33f58-b82a-4a5e-b3eb-2a3923635ad5)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 030](https://git.arts.ac.uk/storage/user/588/files/fae5e911-0c6d-4fc4-a072-4e19b9d1e8e3)
![Aspose Words 8acaca51-7f7b-4c03-a9ad-c5c2e58141e4 031](https://git.arts.ac.uk/storage/user/588/files/fd357ca8-30d4-4974-bf1c-729b4dab3991)

Finally, I use a projector to project the game. Then let the player play the game in front of the Kinect. Showing went well.







