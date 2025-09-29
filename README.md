Real-time phase unwrapping of a screen portion
Holograms are captured using the software provided by the camera’s brand. The 2D-FFT of both holograms are computed. Once the images are translated 
into the spatial frequency domain, three frequency components are identified: the DC (autocorrelation) terms at zero (origin) and the CC (cross-correlation) 
terms which are spatially symmetric with respect to the zero and they lay in the negative semi-axis and positive semi-axis respectively. 
To retrieve only the phase information, which is of interest in quantitative-phase analysis, a mask is generated in order to isolate only the positive axis CC. 
The inverse 2D-FFT are then computed and the phase difference between the first hologram (reference) and the second hologram (sample or object) is calculated. 


The script allows to unwrap the phase from an hologram in a portion of the screen (for which the aspect ratio can be tuned)
where the camera real-time image is remotely projected. Once the script is started, it takes the first frame as a reference hologram and
the following are acquired every 1s. A live window shows the converted phase difference. This approach facilitates the overall analysis 
since no big amount of data are stored but only once the experimental conditions are satisfying, the holograms can be recorded with the camera's sw.
