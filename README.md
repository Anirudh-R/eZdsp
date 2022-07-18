# eZdsp
Experiments using the TMDX5502EZDSP development kit for the TI C5502 DSP.

The dev board features a 16-bit fixed-point TMS320VC5502 DSP running at upto 300MHz. It also includes:
1) On-board audio codec with stereo line in/out jacks
2) 96 × 16 monochrome OLED display
3) On-board XDS100 v2 emulator for JTAG debugging
4) GPIO expansion connector which can mate with Samtec MEC1-130-02-S-D-A

I have done simple experiments/mini-projects using the board to learn about implementation of DSP algorithms. It also helped me learn about DSP architecture and use cases. The projects revolve around taking input from the audio-in jack, implementing filters and audio effects to the signal, and outputting the resultant signal through the audio-out jack. Some projects such as eZdsp_proj17 display the FFT of the waveform on a Nokia 5110 display interfaced through the GPIO expansion connector.

The C55x Chip Support Library (CSL) is used for peripherals such as GPIO, I2C, MCBSP, etc. TI's C55x DSPLIB 2.4 is used to implement DSP functions such as FIR filters, FFT, etc. All code development was done using Code Composer Studio 4.2.4.00033.

Since this is an old board, resouces are hard to find. Below are few which may be useful:
1) https://www.eecs.umich.edu/courses/eecs452/refs.html
2) https://www.eecs.umich.edu/courses/eecs452/proj.html
3) https://raulbehl.wordpress.com/2015/05/24/tms320c5535-ezdsp-usb-stick-audio-playback/
4) https://www.circuitvalley.com/2016/11/smallest-audio-spectrum-analyzer-ti-tms320-dsp-fft-example.html
5) https://www.ti.com/tool/SPRC133
