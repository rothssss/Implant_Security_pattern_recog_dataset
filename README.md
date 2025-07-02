# Pattern Recognition for Securing Bio-implants

Waveforms from an ADC output representing multiple bits are segmented into chunks representing a single bit and saved to all_chunks.pt. 

These chunks were splitted into train and evaluation sets. In each sets, the chunks were shuffled, normalized, and recombined into waveforms representing 8 bits. These data were saved to train_set_shuffled.pt and test_set_shuffled.pt. 

The non-shuffled waveforms in the original order of chunks were saved to test_set.pt. 

In all .pt files, for each chunk, time, quantized waveform, the waveform's discrete derivative, and corresponding 8 bit labels were saved in order. 

The reading from ADC output and the saving/reading for .pt files were documented in build_ch1_dataset notebook. 
