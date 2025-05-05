# eece5554-lab1---robotics-sensing-and-navigation-solved
**TO GET THIS SOLUTION VISIT:** [EECE5554 LAB1 – Robotics Sensing and Navigation Solved](https://www.ankitcodinghub.com/product/eece5554-lab1-robotics-sensing-and-navigation-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;95060&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EECE5554 LAB1 - Robotics Sensing and Navigation&nbsp;Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

Contents:

1. Lab 1 instructions page 1-2

2. Submission instructions and Grading Rubric – page 3 3. Appendix: A serial driver example – page 4

Hardware/ Sensors

1. USB based GNSS puck, issued one per team.

Data collection Policy

Everyone in the team needs to

<ol>
<li>Write their own device driver for data acquisition.</li>
<li>Everyone will be collecting their own datasets individually. They will be sharing the GPS device issued to them.</li>
<li>What to Submit for Lab 1 ?</li>
</ol>
1. Setting up the GPS puck

When you will connect your GPS device, you can see the device name with this terminal command.

$ ls –lt /dev/tty* | head

You will see a list of devices from which you have to figure out your -device file i dentifier. Let us say it is /dev/ttyUSB2

Then you need to set the read write permissions for reading the device properly.

$ chmod 666 /dev/ttyUSB2

You are all set for reading the device using minicom now. Configure your device’s settings in minicom. A quick guide to use minicom

For saving data to a text file, you need to use –C flag on minicom. Save as gps-data.txt Or simply copy paste the terminal output and save it in a text file. Cd

This creates a gps-data.txt file in your current directory. When you want to stop writing to

1

</div>
</div>
<div class="layoutArea">
<div class="column">
Term: Spring 2021

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
the file, press ctrl c .

$ more gps_data.txt

For checking the contents of file

Additional note:

If you want to understand any command, you can either go to web man pages of linux or type the following on terminal.

$ man &lt;command_name&gt;.

<ol start="2">
<li>Write Device Driver for GNSS puck to parse $GPGGA
As we will see in class the GNSS puck provides a number of differently formatted messages. We will focus our attention on the messages that are formatted according to the $GPGGA format.

We need a driver to read in serial data from the puck, parse it for the latitude, longitude and altitude. We have provided an example device driver for a depth sensor in the appendix section, so that you can use that as a template.

You need to then convert the latitude and longitude to utm using the python package “utm” as discussed in class.

Define a custom ros message with header, latitude, Longitude, Altitude, utm_easting, utm_northing, Zone, letter as fields.

Your ros node should then publish all these values in your custom defined ros msg.
</li>
<li>Go outside and collect data

2.1 Stationary data outdoors

Data-collection

Go outside and collect 10 minutes of data at one spot in a rosbag.

2.2 Walk in a straight line outdoors

In a new ros-bag recording, walk in a straight line for a few hundred meters.
</li>
<li>Data analysis and report:
Read the rosbag data into matlab/python.

4.1 Analyse stationary data

Examine the data at your leisure (in a warm spot!) by plotting it or analyzing its statistics. What does this say about GPS navigation? What can you say about the distribution of
</li>
</ol>
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
the error in GPS? What is a good error estimate? Can we put a bounds to these errors? What is the source of these errors?

4.2 Analyse straight line walk data

Examine the utm data (by plotting it or doing statistics on it)

What does this say about GPS navigation when moving? How does the error estimate change as you move as opposed to stay in a spot? What can you say about the distribution of noise in this case?

4.3 Report:

Analyse the data as asked above and write your observations in a brief 1 – 2 page report with plots/charts and submit a PDF copy of it in your GitLab repository.

How to Submit Lab1

<ol>
<li>In your class repo ‘EECE5554’, create a directory called LAB1</li>
<li>Inside LAB1, create sub-directory structure ‘src’.</li>
<li>Push your device driver and analysis code to GitLab. The directory structure
should be:
</li>
</ol>
 src (directory)

<ul>
<li> &nbsp;Gps-driver (directory)</li>
<li> &nbsp;Report.pdf (file)</li>
<li> &nbsp;Analysis scripts  data</li>
</ul>
<ol start="4">
<li>Upload your lab1/src (local computer) to GitLab. Push your local commits to (remote) GitLab server. You can verify this by visiting gitlab.com and making sure you can see the commit there. Your repo structure should look similar to ‘&lt;Path_to_repo&gt;/EECE5554/LAB1/src/’</li>
<li>Upload your pdf report to GitLab (also under the src directory)</li>
</ol>
Grading Rubric (10 Points)

 2 points for working device driver

 3 points for Analysis of Stationary Data

 3 points for Analysis of Moving Data

 2 Points for overall Presentation of Report

Late submission policy is mentioned in the syllabus.

Appendix

1. Python based ros node for Depth sensor on an auv

#!/usr/bin/env python

3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
# -*- coding: utf-8 -*-

import rospy

import serial

from math import sin, pi

from std_msgs.msg import Float64 from nav_msgs.msg import Odometry

def paro_to_depth(pressure, latitude): ”’

Given pressure (in m fresh) and latitude (in radians) returns ocean depth (in m.). Uses the formula discovered and presented by Leroy and Parthiot in: Claude C. Leroy and Francois Parthiot, ‘Depth-pressure relationships in the oceans and seas’, J. Acoustic Society of America, March 1998, p1346-.

”’

# Convert the input m/fw into MPa, as the equation expects MPa. pressure = pressure * 0.0098066493

# Gravity at Latitude.

g = 9.780318 * (1 + 5.2788e-3*sin(latitude)**2 –

2.36e-5*sin(latitude)**4)

# Now calculate the ‘standard ocean’ depth.

Zs_num = (9.72659e2*pressure – 2.512e-1*pressure**2 + 2.279e-4*pressure**3 – 1.82e-7*pressure**4)

Zs_den = g + 1.092e-4*pressure return Zs_num / Zs_den

if __name__ == ‘__main__’:

SENSOR_NAME = “paro”

rospy.init_node(‘depth_paro’)

serial_port = rospy.get_param(‘~port’,’/dev/ttyS1′)

serial_baud = rospy.get_param(‘~baudrate’,9600)

sampling_rate = rospy.get_param(‘~sampling_rate’,5.0)

offset = rospy.get_param(‘~atm_offset’,12.121) # in meter ??

latitude_deg = rospy.get_param(‘~latitude’,41.526) # deg 41.526 N is Woods

Hole

port = serial.Serial(serial_port, serial_baud, timeout=3.)

rospy.logdebug(“Using depth sensor on port “+serial_port+” at “+str(serial_baud))

rospy.logdebug(“Using latitude = “+str(latitude_deg)+” &amp; atmosphere offset = “+str(offset))

rospy.logdebug(“Initializing sensor with *0100P4\\r\\n …”) 4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
sampling_count = int(round(1/(sampling_rate*0.007913)))

port.write(‘*0100EW*0100PR=’+str(sampling_count)+’\r\n’) # cmd from 01 to 00 to set sampling period

rospy.sleep(0.2)

line = port.readline()

port.write(‘*0100P4\r\n’) # cmd from 01 to 00 to sample continuously

latitude = latitude_deg * pi / 180.

depth_pub = rospy.Publisher(SENSOR_NAME+’/depth’, Float64, queue_size=5) pressure_pub = rospy.Publisher(SENSOR_NAME+’/pressure’, Float64, queue_size=5) odom_pub = rospy.Publisher(SENSOR_NAME+’/odom’,Odometry, queue_size=5)

rospy.logdebug(“Initialization complete”) rospy.loginfo(“Publishing pressure and depth.”)

odom_msg = Odometry() odom_msg.header.frame_id = “odom” odom_msg.child_frame_id = SENSOR_NAME odom_msg.header.seq=0

sleep_time = 1/sampling_rate – 0.025

try:

while not rospy.is_shutdown():

line = port.readline() #print line

if line == ”:

rospy.logwarn(“DEPTH: No data”) else:

</div>
</div>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
<div class="layoutArea">
<div class="column">
if line.startswith(‘*0001’): odom_msg.header.stamp=rospy.Time.now() try: pressure = float(line[5:].strip())

except:

rospy.logwarn(“Data exception: “+line)

continue

pressure_pub.publish(pressure)

depth_mes = paro_to_depth(pressure – offset, latitude_deg) depth_pub.publish(depth_mes) odom_msg.pose.pose.position.z = -depth_mes odom_msg.header.seq+=0

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
6

</div>
</div>
<div class="layoutArea">
<div class="column">
odom_pub.publish(odom_msg) rospy.sleep(sleep_time)

except rospy.ROSInterruptException: port.close()

except serial.serialutil.SerialException: rospy.loginfo(“Shutting down paro_depth node…”)

</div>
</div>
</div>
