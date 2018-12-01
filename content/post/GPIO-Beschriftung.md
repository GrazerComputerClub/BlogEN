+++
showonlyimage = false
draft = false
image = "img/pileaf.jpg"
date = "2018-12-01"
title = "Raspberry Pi GPIO labelling"
writer = "Martin Strohmayer"
categories = ["Raspberry Pi"]
keywords = ["pileaf", "reference card", "pi", "gpio"]
weight = 1
+++


One problem that often occurs when building circuits are the unlabelled GPIO pins of the Raspberry Pi. Counting the GPIO pins is a typical task when working with the inputs and outputs. Labels or so called "reference cards" that put on the GPIO pin header, can solve the problem.
<! - more ->

## creation

The GPIO contacts of the Raspberry are not labeled. But you can find reference cards on many Raspberry Pi Shops. They are put over the GPIO connector pins. Of course, these reference cards do not have to be made of a hard material. They can easily made of paper with some manual work. They are printed out and then cut to size. The holes can be made with a nail. Such PDF templates are often found on the Internet for example at [http://noxmiles.de/Raspberry-Pi-GPIO-Beschriftung.pdf](http://noxmiles.de/Raspberry-Pi-GPIO-Beschriftung.pdf). A special option here is the project Pi Leaf [https://www.raspberrypi.org/blog/raspberry-leaf](https://www.raspberrypi.org/blog/raspberry-leaf). The drawing was not done in a graphics program, it is defined by a description language. Originally the project was described on [Dr. Monk's DIY Electronics Blog] (http://www.doctormonk.com/2013/02/raspberry-pi-and-breadboard-raspberry.html) and published on [Sourceforge] (https://sourceforge.net/projects/pileaf/) .

For the outdated project, a fork was created by "Sanderr" on [Sourceforge] (https://sourceforge.net/u/sanderr/pileaf). This version also includes a template for the 40-pin connector of the current Raspberry Pi variants. The description file "pi-leaf.asy" can be used to create the PDF file with the program Asymptote.

```
sudo apt-get install asymptote git
cd / usr / src /
git clone git: //git.code.sf.net/u/sanderr/pileaf u-sanderr-pileaf
cd u-sanderr-pileaf
asy -f pdf pi-leaf.asy
```

An already created PDF template file can be downloaded from our homepage at [http://raspjamming.at/PDF/pi-leaf.pdf](http://raspjamming.at/PDF/pi-leaf.pdf). When printing (e.g. with the browser Chrome), the setting "Fit to page" must be deactivated!

! [Chrome print dialog] (../../img/pileaf-printer.png)
