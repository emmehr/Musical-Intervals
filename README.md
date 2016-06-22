# Musical-Intervals

Ultimately, this Python program will be able to read a music file and figure out the intervals used in it.
The current upload allows reading a .wav file and finding the maximum frequency components at each time window.
- *1st issue:* the fundamental would not always be the maximum frequency component. Sometimes one of the harmonics becomes exceeds the amplitude of the fundamental.
- *Second issue:* the length of the time window determines the fft resolution. Thus, in order to have 1 Hz resolution (still inadequate for the tuning bass notes) one second of the music needs to be sampled. During this 1-s interval multiple notes will be played in up-tempo music. 1 s is not long enough sampling time to give us adequate frequency resolution and not short enough time to assure all the notes that are played will be captured.
