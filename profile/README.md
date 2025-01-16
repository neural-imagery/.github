# Neural Imagery
Visit [neuralimagery.com](https://neuralimagery.com) to see an overview of our mission and our house. The goal is to stream visual imagination from your brain.

The house has concluded, and we are pending paper publication. The zoom recording of our September 24 demo day in Cambridge, MA can be accessed [here](https://harvard.zoom.us/rec/share/Lu1hCwnSOzA3Ms1T4iTq03R5-1q_OFMjEjbjNOoZIRDYvADXaTt75Lo5FnetV28-.JQ90F8r4fbi9JLg1). Our paper is [here](https://arxiv.org/abs/2406.07662).

## Repo Breakdown

[tomography-experiments](https://github.com/neural-imagery/tomography-experiments) includes simulation code for both CW and TD systems, primarily based around noise-less simulations aiming to reconstruct a set of shapes with different optical properties of absorption and scattering coefficients, with detectors placed on its circumference. It runs Monte-Carlo simulations for speed.

[brainscanner-matlab](https://github.com/neural-imagery/brainscanner-matlab) is a local MATLAB app to drive the TechEn CW BT-NIRS headset with 4 dual-wavelength sources (735 and 850 nm) and 8 detectors, forked from the original creator's repo and updated to run with less headache on Mac or Windows. We have also added a server to spit real-time data to a TCP endpoint. It includes a simulation mode in case you don't have a headset yet but want to run our pipeline yourself. Note that this is more fully featured than the default Windows .exe usually distributed with the headset, but has a higher setup overhead.

[neural-imagery-app](https://github.com/neural-imagery/neural-imagery-app) is our frontend code to visualize real-time data (and FFTs of the headset data!) from the backend that the MATLAB backend connects to.

[nlim](https://github.com/neural-imagery/nlim) is our Python backend to both relay the MATLAB code and connect to the ML pipeline.

[signal-classifier](https://github.com/neural-imagery/signal-classifier) contains an ML pipeline specifically for retinotopy data.

[ml](https://github.com/neural-imagery/ml) contains various pre- and post-processing algorithms to reconstruct images from the raw fNIRS data.

[movie-player](https://github.com/neural-imagery/movie-player) provides pre-configured stimulus to subjects during experiments and saves stimulus presentation timestamps for later analysis.

[data-experiments](https://github.com/neural-imagery/data-experiments) is similar to `movie-player`, but runs more types of experiments and stores more metadata.
