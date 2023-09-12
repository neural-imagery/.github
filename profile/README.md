Visit [neuralimagery.com](https://neuralimagery.com) to see an overview of our mission and our house.

The house is currently ongoing. Message us if you'd like to attend our demo day in mid to end September in Cambridge, MA.

[tomography-experiments](https://github.com/neural-imagery/tomography-experiments) includes simulation code for both CW and TD machines.
[brainscanner-matlab](https://github.com/neural-imagery/brainscanner-matlab) is a local MATLAB app to drive the TechEn CW BT-NIRS headset with 4 dual-wavelength sources (735 and 850 nm) and 8 detectors, forked from the original creator's repo and updated to run with less headache on Mac or Windows. We have also added a server to spit real-time data to a TCP endpoint. It includes a simulation mode in case you don't have a headset yet but want to run our pipeline yourself. Note that this is more fully featured than the default Windows .exe usually distributed with the headset, but has a higher setup overhead.
[neural-imagery-app](https://github.com/neural-imagery/neural-imagery-app) is our frontend code to visualize real-time data (and FFTs of the headset data!) from the backend that the MATLAB backend connects to.
[nlim](https://github.com/neural-imagery/nlim) is the source code for our [website](https://www.neuralimagery.com/).