# Flood Segmentation using Sen1Flood11 (Sentinel-1 SAR)
Work done by: Muvvala Krishna Kiriti
<br>
As a part of ISRO NRSC Internship
<br>
Contact: muvvalakiriti@gmail.com
#
Work done as of now: 
1) Identified SSL4EOS12 dataset being used in more than 1 FM so used pretrained RestNet50 of SSL4EOS12 with SSL MoCo (I started with this as it was first model mentioned in thier github) and used decoder/segmentation head of UNet with first frozen (30 epoch) then for 40 epoch unfoze it after 20 and then set max epouch as 200 with early stopping as 15, later increased to 20 but the best was same as 15.
2) (future work) Own restnet 50 with same UNet as segmentation head.
3) (future work) the same SSL4EOS12 model with gradual unfreeze instead of complete unfreeze.

#
Citations/ Refrences: <br>
1) SSL4EOS12: (the pretrained model) https://github.com/zhu-xlab/SSL4EO-S12
2) SMP: (segmentation models) https://github.com/qubvel-org/segmentation_models.pytorch, https://segmentation-modelspytorch.readthedocs.io/en/latest/
3) 
