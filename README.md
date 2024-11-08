java c
GEOG60941: Environmental Remote Sensing 2024-2025
Assessment 1:  Long term monitoring of the Earth’s surface
Deadline:  14:00  Thursday  7th  November  (week  7).  Submission  via  the  Assessment Submission tab on the BB site.This assessment is worth 20% of the overall mark. The total word limit for this assessment is 500 words. This includes all text but excludes the assessment title, reference list, numbers in tables and text that is included in ﬁgures and ﬁgure captions. Everything else is included.
Task:
Create a poster with the title “Remote sensing as a tool  for long term quantitative monitoring of land cover change: Opportunities and Challenges.”.Your  answer should discuss the question statement with speciﬁc  reference to  both the literature on the topic AND results obtained from your own data analyses. You should use what you learn in the practical sessions to generate data/outputs to graphically demonstrate key  points  made within your discussion  i.e.  refer to your own data as examples or case studies (think about the speciﬁc points mentioned below!).
Instructions. Please read them very carefully:
●   Make sure that your poster addresses at least the following:
o    The role of spectral indices in long term quantitative monitoring of land cover change
o    How  and why the  atmosphere  may  inﬂuence spectral  indices  and ways in which these issues may be minimised
o    The implications of using different sensors to monitor quantitative changes in land cover over time
o    Wider discussion of how such challenges are being/can be addressed
o    Conclusions with reference to the usefulness of remote sensing for long term quantitative monitoring of land cover change.
●    Include  a  URLlink  to  your fully commented Javascript code somewhere on your poster (see end of this document for further instructions)
●   Any  ﬁgures  or  tables  included  in your  answers  need  a  proper ﬁgure  number  and caption and should be referenced from the text.
●   You  must  use  references from the  literature to back-up your key points in each of your  answers.  The  references  (both  in  text  and  in the  reference  list)  need to  be formatted appropriately. As this is a poster assessment you are allowed to use the numeric referencing system to save space.
●   A complete list of references used in all of your answers should be included on your poster
●    Do  not  screen  grab  images or charts from Google  Earth Engine (GEE). All images should be exported from GEE and where necessary, tidied up (e.g. add legends, scale bars and N arrows) in a GIS software or spreadsheet package (e.g. redraw charts in Excel) prior to being inserted into your assessment.
●    The  poster  size  should  be A1  (the orientation  is up to you). An A1 page is 594 x 841mm. You can use a range of software to produce your poster; e.g. Powerpoint, Illustrator, Coral Draw, Inkscape. Whichever software you choose, remember to start by  deﬁ ning  the  document  page  size;  e.g.  If  you  are  producing  the  poster  using Powerpoint, you should go to the Design tab, then select Slide Size. Choose Custom Slide Size.
Further help and guidance
Background informationSentinel-2  is  a  relatively  new  platform,  which  will  become  increasingly  important  and prominent  in ecosystem studies going forward. However, for exploring historical trends in data, we need to turn to other platforms such as MODIS (since 2000) and Landsat (since the 1970s). There are two main challenges associated with the use of remotely sensed data for quantitative studies of temporal change:1) The signal recorded by the sensor is not necessarily a good measure of the change in surface conditions (Moran et al. 2001). This is because the signal measured by the sensor is a function of surface reﬂectance, coupled with sensor calibration, solar zenith angle, sensor viewing angle, and atmospheric inﬂuences. In order to be of lasting quantitative value, it is therefore recommended that remotely sensed data be calibrated to physical units such as reﬂectance.2) The  use of data from  multiple sensors  is often required to ensure data coverage and continuity, but differences in the spectral characteristics of sensors result in spectral index values  being  different.  Such differences  may  have  implications for  long term vegetation mo代 写GEOG60941: Environmental Remote Sensing 2024-2025 Assessment 1: Long term monitoring of the Earth’s surfaceJava
代做程序编程语言nitoring (Cund ill et al., 2015).
References citedCund ill, S.L., Van der Werff, H. and Van der Meijde, M., 2015. Adjusting spectral indices for spectral  response  function  differences of very  high spatial  resolution sensors simulated from ﬁeld spectra. Sensors, 15(3), pp.6221-6240.Moran, M. S., R. Bryant, K. Thome, W. Ni, Y. Nouvellon, M. P. Gonzalez-Dugo, and J. Qi. 2001. A  reﬁ ned empirical  line  approach for  reﬂectance factor  retrieval from  Landsat-5 TM and Landsat-7 ETM+. Remote Sensing of Environment 78:71-82.
Generating data to exemplify points within your answersI highly recommend that you complete your reading and outline a structure to your poster before embarking  upon the  practical component of the assessment. This is because you need to know what points you want to exemplify with your data - think about what data you want to display and then work out how to generate those data. Some hints as to what data you could generate to exemplify your  points  are  provided  below. Of course you can also generate other data - anything that you want to help with your answer!
●   Demonstrate the inﬂuence of the atmosphere on vegetation by comparing data from the same satellite  products with different  levels of  atmospheric correction. Think about the impact on the spectral signature(s) but also on any vegetation indices that will be derived from those spectral signatures.
●   Demonstrate the  potential/limitations  surrounding the  use  of  multiple sensors for long term  monitoring  by processing data from two different sensors for the same location and date (as close as possible!). Think about how the spatial patterns and data values differ between sensors and why?Whilst most of the image processing should be done using Google Earth Engine, you can also  use ArcGIS,  QGIS,  Excel,  R  and other  packages to further  analyse  and display your results.  It’s important to think about how “best” to create and display examples with a focus on demonstrating your points - you don’t have to create examples using GEE for every point that   you  make  if you  don’t deem  it to  be  necessary. You should  aim for 3-4 generated outputs.
Hints and tips:
●   The  bands  of  Sentinel-2  imagery  are  different  to that  of  Landsat e.g. cloud cover  is controlled  by the  band ‘CLOUDY_PIXEL_PERCENTAGE’. The spectral bands in Sentinel imagery  are  also of different spatial resolutions and different to that of Landsat data, which is 30 m spatial resolution. To reduce that level of complexity I have put together some example code for you here to do some additional pre-processing of the Sentinel-2 imagery for you
https://code.earthengine.google.com/5380939cc7e68fb9050c4c70fb393299
●   Remember  that  i) the band positions and   wavelengths might differ between different sensors, and ii) pixel size may differ between different sensors; and iii) time of year is an important  consideration.  For  Landsat  9,  the  metadata  property  for  cloud  cover  is ‘CLOUD_COVER’ but for Sentinel-2 it is “CLOUD_COVERAGE_ASSESSMENT” (you can get this  information from clicking on the name of the image collection and looking at the metadata!)
●   There are several “land cover  maps” available  in GEE if you want to use them. You can search for a land cover map that covers your area of interest and ﬁts your purpose best.
●   You   can  use  your   knowledge  of   how  to  generate  spectral signatures/proﬁles  from Practical 1 and 3 if you think a spectral plot may be useful to exemplify your point(s)!
●    If you want to “comment out” large chunks of code so that it is not run but not deleted, simply  highlight the  relevant  lines of code   and  select  ctrl+ / to reverse this process simply press ctrl + / again.
●   To obtain a link to your GEE script simply click Get Link. A url will appear in your browser address ﬁeld. You should paste this link at the end of your report (note do not copy and paste  the  web  address  from  your  browser  –  you  must  use  the  Get  Link  button!). However, if you continue to make edits on this code after the link is generated, they will
not be updated in the linked version so only do this when you are ﬁ nished with the code.
●    Remember to use the Google EE help documentation if you are unsure of anything







         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
