# eZdsp
Experiments using the TMDX5502EZDSP development kit for the TI C5502 DSP.

The dev board features a 16-bit fixed-point TMS320VC5502 DSP running at upto 300 MHz. It also includes:
1) On-board audio codec with stereo line in/out jacks
2) 96 × 16 monochrome OLED display
3) On-board XDS100 v2 emulator for JTAG debugging
4) GPIO expansion connector which can mate with Samtec MEC1-130-02-S-D-A

I have done simple experiments/mini-projects using the board to learn about the implementation of DSP algorithms. It also helped me learn about DSP architecture and use cases. The projects revolve around taking input from the audio-in jack, implementing filters and audio effects on the signal, and outputting the resultant signal through the audio-out jack.

## Index
1. ezdsp_demo: Demo which comes with the board
2. eZdsp_proj1: Toggle LED using timer
3. eZdsp_proj2: OLED display scroll
4. eZdsp_proj3: Loop audio in and out
5. eZdsp_proj4: Noise gate
6. eZdsp_proj5: Echo
7. eZdsp_proj6: Reverberation
8. eZdsp_proj7: Sine wave generator
9. eZdsp_proj8: Comb notch filter
10. eZdsp_proj9: FIR lowpass filter
11. eZdsp_proj10: Cascaded IIR filter
12. eZdsp_proj11: Phasing FIR highpass filter
13. eZdsp_proj12: Adaptive delayed LMS Filter
14. eZdsp_proj13: Wavelet filtering with soft thresholding
15. eZdsp_proj14: Goertzel algorithm
16. eZdsp_proj15: Autocorrelation noise detector
17. eZdsp_proj16: Nokia 5110 LCD interfacing via expansion connector
18. eZdsp_proj17: Spectrum analyser with Nokia 5110 display
19. eZdsp_proj18: Optimised vector subtract using assembly

The C55x Chip Support Library (CSL) is used for peripherals such as GPIO, I2C, MCBSP, etc. TI's C55x DSPLIB 2.4 is used to implement DSP functions such as FIR filters, FFT, etc. All code development was done using Code Composer Studio 4.2.4.00033.

Since this is an old board, resources are hard to find. Below are few which may be useful:
1) https://www.eecs.umich.edu/courses/eecs452/refs.html
2) https://www.eecs.umich.edu/courses/eecs452/proj.html
3) https://raulbehl.wordpress.com/2015/05/24/tms320c5535-ezdsp-usb-stick-audio-playback/
4) https://www.circuitvalley.com/2016/11/smallest-audio-spectrum-analyzer-ti-tms320-dsp-fft-example.html
5) https://www.ti.com/tool/SPRC133
