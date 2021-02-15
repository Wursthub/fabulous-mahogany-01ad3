---
title: LaserEye
subtitle: Protecting against all laser types while expanding human vision
date: '2019-04-30'
thumb_image: images/Lasereye-worldsbest.jpg
thumb_image_alt: An orange on a blue background
image: images/Lasereye-worldsbest.jpg
image_alt: An orange on a blue background
template: project
---
This project was born out of the desperation to bridge the gap to business at the end of the PhD studies. Together with Ugur Sezer, a quantum physicist I collaborated with at the time, we developed this idea during a startup incubator. Together we learned basic business skills and applied lean methodology during 150+ customer interviews conducted within 6 months: Not wasting any money on building anything before not thorougly understanding the problem.

### The Problem

Neuroscience and quantum physics often requires the use of dangerous and often invisible lasers which can leave holes in the walls. The protective goggles are heavy, expensive and make the light you want to work with or of oszilloscopes invisible all while still being penetrateableby lasers of other colors.

> Did you know that companies have to spend hundreds of millions of euros each year for laser safety goggles which in the end nobody wants to wear? We want to transform this annoying cost factor into a thing people WANT to wear. With our solution we improve the users visibility and display digital parameters

![](https://raw.githubusercontent.com/Wursthub/fabulous-mahogany-01ad3/master/Lasereye-Problem2.png)

### The Solution

The best protection would be having no photons from the outside hitting your eyes. By blocking the light path with camera lenses and showing the outside world only via augmented reality protects from all light, enables digital head-up displays and even visualizes infrared and UV-light due to the camera sensors sensitivity in these regions.

![](https://raw.githubusercontent.com/Wursthub/fabulous-mahogany-01ad3/master/static/images/Lasereye-Problem.png)

Most basic sensors cover a large infrared regime including often used 1064nm lasers. This would potentially make all existing lasergoggles obsolete and add SAAS business models due to the availability of an AR-device in the lab as a basistechnology for digital ocumentation, QA, remote control etc. 

![](https://raw.githubusercontent.com/Wursthub/fabulous-mahogany-01ad3/master/static/images/Lasereye-spectral%20range.png)

### The Team

Without the help of my genious friends and lots of free time this idea would have not been possible

*   Ugur Sezer - customer development, business development

*   Philipp Geyer - basic technology prototype

*   Christoph Götz - customer development, business development

### The Result

*   Admitted to prestigeous high-tech incubator [Inits](https://www.inits.at/en/home/). 9 Month program including tutoring financial support and goverment grants

*   150+ customer interviews, patent research, profit loss calulation, bill of materials, supplier evaluation etc.

*   Communication strategy, pitching, business models, 

### Lessons Learned

Diving into business, while understanding the use of lasers in medicine, manufacturing and science was an insane amount of work, but so interesting. Especially meeting over a hundred users & stakeholders from workers insurance to doctors operating prostate using green lasers, visiting a laser google manufacturing line and meeting with chinese AR-goggle producers in Kopenhagen. 

The summary is, that the need is there. People do have problems with goggles, however - at least in science - scientists are not sooooo careful and often just circumvent the safety protocols to get the experiment done. For repetitive tasks in industry almost everything involving a terrible laser is secured with organizational measures e.g. putting everything in a tight box to avoid the need for goggles completely. Medicine would need a medical device certification and extremely high standards which would make the solution potentially very expensive. 

The market itself is thus, pretty niche albeit the field itself (laser tech) is a key technology and had a 30% CAGR at the time. 

Furthermore, biology and technology just did not match (yet). The lesson is, that the human eye is just damn good at what its doing! The dynamic range is incredible which allows us to operate fairly well in dark lit environments even with some bright spots around. 

**CMOS chips** on the other hand have a really limited dynamic range and especially fair bad in low light conditions. Having a laser source around thats 90 000 000 times brighter than the sun (180 W / mm2 / nm compared to 2 W / m2 / nm of the sun) does produce grainy or oversaturated images that you would not want to watch 5h a day working with lasers.

**AR-goggles** also have their limitations: While Fresnel lenses have increased the field of view, peripheral vision is still fairly low. The displays  technology at the time in 2016/2017 were limited to full HDish resolution which makes it hard to see details - a thing absolutely necessary when working in the lab. Also the form factor, cables, power supply etc. add to the weight and make it unlikely people wouldnt complain about ergonomics. 

**Low latency FPGA computing** is required especially when watching your real environment. Motion sickness already can be induced with few ms of delay between the recording of the image and its display which pushed us towards using FPGAs for the processing. These chips are expensive and hard to program especially when trying to implement lens correction algorithms, HDR etc. Using see-through enabled AR-headsets with fancy chips from e.g. [Qualcomm](https://www.qualcomm.com/products/snapdragon-xr1-platform) might shift the development effort to companies that can actually afford it. However, certifying a consumer headset for use in the laser lab is a challenge by itself. 

All in all, thinking through a business case in emerging fields like optical sensors, AR-goggles and laser-tech gave me a good impression of the state of the art in high-tech and the limitations of this technology when it comes to bio-vision that was optimized for a few billion years by evolution.



