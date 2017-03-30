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
