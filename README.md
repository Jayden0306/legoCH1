# legoCH1
Lego EV3 1st project.

Team 1

Gabriel Summers   ghs9@uw.edu

Jayden Tan        jayden91@uw.edu

## Agreements:
  1) We are available MWFSaSu all day. TTH available 10-12:30
  2) We will use github to host our journal and code.
  3) simple plan is to use the RileyRover basic body build 

## 3/28/2017
  1) Made team
  2) Counted out pieces of kit
     * They all were there
  3) Set up lock and both of us practiced opening it.
  4) Set up git repo
     * Both are now contributers.
  5) Read the challenge 1 description.
      * We need to research biased random walk.
      * We think the walk shouldnt be too bad.
      * The sensors shouldnt be too much of a pain.
          * We want to have the ultrasonic mounted on top front,
          * two touch sensors in front.
      * Movement will be with treads for now.
  6) Plan to meet 3/29/17, 1:30PM, CP206D
  
## 3/29/2017
  1) Team met in CP 206 at 1:30PM
      * There was a class in the CP 206D lab so we just sat in the lounge and planned our robot.
  2) Once the class left the lab we went in and started building our bot.
      * We have settled on the RileyRover design for now, with two touch sensors modified on.
  3) We want to begin coding for RobotC but it requires a firmware update for our EV3 board which we do not have a usb for.
      * We looked for a usb but cannot find one. May have to do that tomorrow.
  4) From 2:45 to 4:30 we worked on building the robot.
      * Building the car was easy, but attaching the sensors was difficult.
          * We built a cage that sticks out the front and attached two swiveling arms that would press the sensors. This worked but we are concerned that there will be a skinny obstacle in front that it doesn't hit.
          * altered to have one bar in the center that would press both arms if hit in center. This does not work very well.
          * Removed arms and instead had one arm in the center that would press both if hit center, left if hit from left, right if hit from right. This seems to work the best.
          * Now we address issue of some parts that swivel "drooping". We attached more bars, added support to EV3 board. It works and looks pretty cool.
          * Tested it (without actually running cause we dont have usb to update firmware) manually by pressing it up against obstacles and it works like it should.
          * We have a concern that the sensers may be stuck pushed half in after bar presses against them if the spring inside the sensor doesn't push hard enough to clear the arm. This is something that we will be able to see better once we get code running.
  5) We plan to meet again durring class tomorrow, 3/30/17 at 8:00AM
  
## 3/30/17
  1) Team met for lab starting at 9:09AM
  2) Liscence is expired on mindstorms for the RobotC environment.
      * Talked to Fowler and Lab manager. They said they would send an email and get it sorted out.
  3) While waiting for liscencing issue, we ran demo program already installed on the brick. It seems to work perfectly but it is a limited test (just back and forth movement).
  4) We tried to connect USB from brick to computer, nothing happended.
  5) Jayden is now trying a different coputer to see if the IDE will work.
      * It didn't.
  6) We used the lego graphical IDE because that works and made a simple program that runs forward and then runs backward. This works perfectly and it ended up in relatively the same spot (about 3in off).
  7) Plan to meet monday 4/3/17 at 1:30PM
  
## 4/3/17
  1) Team met for lab starting at 2:00PM
  2) Jayden went to the lab first. He found out that the Robotc IDE is still expired. We could not test our robot without the IDE activate.
  3) We have decided to download the 10 day free trial for RobotC for lego mindstorms so we can start working on it today.
      * The VM that we are downloading the trial to is having some issues so we are restarting it.
  4) We have been viewing some internet resources on RobotC for when we get started writing code.
  5) While Jayden tries to download the trial on his laptop. I go through online tutorials on RobotC.
  6) We could not download the trial successfully on the laptop so we are now going to Snoqualmie building to check out a surface. Hopefully that works.
      * This doesn't work since we cannot download software onto the library's surfaces.
  7) We are calling it a day and plan to meet tomorrow during class. 4/4/17 at 8:00AM
  
## 4/4/17
  
  ### part 1:
  1) Team met for class today at 8:00AM
  2) We realize that only certain computers in the lab have the correct liscence for the RobotC so now we are downloading the kernal to our EV3 brick.
  3) We wrote a simple program to move forward.
  4) next we wrote a program to test bumpers and play sounds.
  5) Now we are writing a program that moves left and right.
  6) Now we combine the three programs we wrote to move forward, if it gets touched reverse and go in the opposite direction.
      * Syntax errors with method call vs. startTask().. We ended up siding with a simple method call.
  7) Now we test it in the explorer's space. It generally explores but sometimes has issues detecting when both of them are pressed.
      * We have added a wait to when the first sensor is triggered to when the trigger handler is called to allow time for both of them to be pushed.
      * We have also added a push bar to the front and increased stability of middle axel to ensure that both have a higher chance of being hit if they should be.
  8) Testing it in the explorer's space, this new design and sensor handler function work a lot better but there are still improvements to be made.
  9) We plan tomorrow, 4/5/17 at 3:30PM. For now we have made good progress for today.
  
  ### part 2:
  1) Jayden has free period so he added bar and cogs to front of robot while Gabe is in class.
        * The mods increase pressure so pushes to the front are more recognizeable.
        * The mods also have a latent feature where pushes from the side are less recognizeable when the test program is run.
  2) Because the computer has crashed and the robot build is stable and time is short, Jayden calls it a day.
  
## 4/5/17
  1) The team today meets at 3:30
  2) We begin by remodifying the front.
      * We move the sensors further apart.
      * We lengthen the bar to work with the more distant sensors.
          * To do this We need to raise it a slight bit but this requires rebuilding a large portion of the front
          * We do this but run into some issues getting parts to match up.
          * We are concerned that the sensors will now be too sensitive to touches from the side. But we need to test before we can say for certain.
          * Attaching wheels to the front has turned out to be more difficult than we thought as we do not want it to be too wide but we still want to differentiate sides from front pushes respectively.
          * The bar works well now good recognition of direction of push.
          * Small bug encountered where bar could snag on crossbeam causing forward push to be not be recognized.
          * Fixed the snag bug.
  3) We research some more robotC topics (array initialization, random library) to help in our implementation of biased random walking.
  4) We update the code some more.
      * Changed tones that are played.
      * recognizes push during turn.
      * shorter backup time.
      * Started writing biased random handler (commented out for now).
  5) We plan to meet again tomorrow at 8:00AM in lab.
  
## 4/6/17
   1) We spent time work on the CAD file after his class.
   2) The lego digital designer software was not working. The software UI keep flashing all the time.
   3) We have to use our own laptop instead of the school computer to work on the CAD file for our robot.
  
## 4/7/17
  1) We fixed the implementation of the random walk. 
      * Its randomness will be more depend on the probability/ratio to determine the direction.
  2) We spend time the work on the extra creadit: use motor feedback to detect obstacle.
  3) We were looking for the best fit function call to give useful motor feedback, then we can use the feedback detect obstacle
  4) The first approach was trying to use the motor encoder function. It didn't work because the function only return the total degree from the start program til end. 
  5) The second approach was using the motor rpm function. We were expect this function will be able to detect obstacle. It didn't. The robot's left and right wheel rpm is keep switching all the time. Also, the rpm of both motor gets higher and lowers depending on the friction of the ground. We have not figure out the correct threshhold for the rpm.
  
  
  
  
