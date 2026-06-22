Real-time Phase Unwrapping of Holograms Directly from the Desktop Screen

Holograms are captured using the acquisition software provided by the camera manufacturer and displayed on the desktop screen. The 2D Fast Fourier Transform (2D-FFT) of both holograms is computed. Once the images are translated into the spatial frequency domain, three frequency components are identified: the DC (autocorrelation) term at the origin (zero frequency) and the CC (cross-correlation) terms, which are spatially symmetric with respect to the origin and lie along the negative and positive semi-axes, respectively.

To retrieve only the phase information, which is of interest in quantitative phase analysis, a mask is generated to isolate the positive-axis CC component. The inverse 2D-FFT is then computed, and the phase difference between the first hologram (reference) and the second hologram (sample or object) is calculated.

The script allows phase unwrapping from a hologram within a selected portion of the screen (with an adjustable aspect ratio) where the camera’s real-time image is displayed lively or accessed through remote desktop from another computed connected to the camera. Once the script is started, it captures the first frame as the reference hologram, and subsequent frames are acquired every 1 s. A live window displays the computed phase difference in real time.

This approach simplifies analysis by avoiding the need for large data storage; holograms are recorded using the camera’s native software only after the experimental conditions are optimized.

How to cite this work?
 
If you use this repository or the associated digital off-axis holography workflow, please cite:
[1] Ricchiuti, G.; Allec, S. I.; Ziatdinov, M.; Prabhakaran, V. Toward Intelligent Multimodal Holography for Real-Time Chemical Imaging of Dynamic Ion Separation. Advanced Intelligent Discovery 2026, e202500237. DOI: 10.1002/aidi.202500237.


