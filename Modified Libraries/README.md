These are existing library files that replace the Teensyduino installed ones. ST7735_t3.cpp just has a modification to the start number of the column for my particular TFT. 
synth_waveform has a modification to call a new function sync() to reset the waveform start - this is to allow LFOs to retrigger when note on is received. 
effect_combine has an extra combineMode enumeration to turn it off and allow audio to pass through.

effect_ensemble.h and effect_ensemble.cpp go in .....\Arduino\hardware\teensy\avr\libraries\Audio\   
effect_ensemble.h needs adding to Audio.h. This is mainly the work of another member of the PJRC forum, I modified it to allow adjustment of the chorus rate.
