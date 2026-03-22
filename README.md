# Flood Segmentation using Sen1Flood11 (Sentinel-1 SAR)
Work done by: Muvvala Krishna Kiriti
As a part of ISRO NRSC Internship
#
Contact: muvvalakiriti@gmail.com
<br>
<br>
Work done as of now: 
1) Identified SSL4EOS12 dataset being used in more than 1 FM so used pretrained RestNet50 of SSL4EOS12 with SSL MoCo (I started with this as it was first model mentioned in thier github) and used decoder/segmentation head of UNet with first frozen (30 epoch) then for 40 epoch unfoze it after 20 and then set max epouch as 200 with early stopping as 15, later increased to 20 but the best was same as 15.
2) (future work) Own restnet 50 with same UNet as segmentation head.
