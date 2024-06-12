# Dataset for Globally Optimal Event-Based Divergence Estimation for Ventral Landing

The ventral-landing-event-dataset was produced for the paper "Globally Optimal Event-Based Divergence Estimation for Ventral Landing" and contains real event streams from ventral landings.  There are eight different event streams, where each stream was produced under a similar ventral trajectory towards a different surface. The dataset represents each event stream in two different formats: 

* **Entire event stream:** In this format, the entire event stream is located in the file *undistorted_events.csv*. The *ground_truth_depths.csv* file contains the ground truth distances to the surface at the corresponding timestamps located in the file *ground_truth_timestamps.csv*. The *event_information.csv* file contains additional information on the event camera. Note that the event data has been undistorted so some of the events lie outiside the event camera's image frame.  Hot pixels have also not been accounted for.  This dataset can be downloaded [here](https://drive.google.com/drive/folders/14_KwWMmmpYtOZUYa4m3QlQQ9Bn7S0fDD?usp=sharing "entire event streams").

* **ECMD interpretable format:** This dataset format was used to get the results for our paper. Each event stream is split into event batches of 0.5 seconds and can be located in the directory *5000000_microsecond_event_chunks/csvs*, and the corresponding ground truth divergence values for each batch are also provided in the file *ground_truth_divergence.csv*. The *event_information.csv* file contains additional information on the event camera. Note that the event data has been undistorted, has had hot pixels removed, and has been subsampled. This dataset can be downloaded [here](https://drive.google.com/drive/folders/1I26pwHQLJlkpWzxHNkFDNj4yRmihmxjL?usp=sharing "event batches").

This dataset contains the following event sequences: 

* 7 real event sequences observing 2D prints of landing surfaces (Surf2D-X, where X = 1 to 7) of duration ~15 seconds each
* 1 real event sequence observing the 3D print of a landing surface (Surf3D) of duration ~15 seconds

All event sequences were recorded on the Prophesee event camera and all ground truth distances and timestamps were recorded on an Intel RealSense camera.

![alt text](https://github.com/s-mcleod/ventral-landing-event-dataset/edit/main/setup.png?raw=true)
![alt text](https://github.com/s-mcleod/ventral-landing-event-dataset/edit/main/high_contrast.png?raw=true)
![alt text](https://github.com/s-mcleod/ventral-landing-event-dataset/edit/main/low_constrast.png?raw=true)
