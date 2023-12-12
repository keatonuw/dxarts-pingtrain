# PingTrain

A quadraphonic sonic installation system.

### About

This project includes the code and image associated with my ping train project created 
during AU23 DXARTS 470 at the University of Washington. The project explores speculative
futures for peer-to-peer communication, distributed computing, and interoperability in
software and society.

The code is implemented for use with a 4-output audio interface - in the installation,
these outputs were wired to 4 transducers sitting in suspended cans. However, the projects
sonic behavior can be observed without the installation by setting Pure Data's audio output
to appropriate speakers.

### Running

The main file is `node-cluster-del.pd`, which contains several instances of `pulse-node.pd`.
Each `pulse-node` is an semi-autonomous cell which receives a clock signal and audio input to
produce its own audio output. The `node-cluster-del` sets up a network of these nodes such that
they can communicate with each over via audio.

To run, simply open `node-cluster-del.pd` in Pure Data and click the toggle in the top-left.
