# Codecs
https://vimeo.com/104554788

- Compressor and decompressor
- there are proprietary and open codecs
- H.264, ProRez, DWxHD

# Containers
- a bucket that hold stuff like audio, codecs, subtitles
- .mov, ,wmv, .avi, .mkv, .mp4

# Types of codecs
- There is no "best" codec. Just best codec for a specific purpose
- Capture codec, edit codec, delivery codec, archival codec

# Bit Depth
- number of values between dark and light
- Given a gradient from left to right, deep depth means you don't see vertical lines. Shallow depth you see vertical lines
- 8-bit codec means there's 2^8 or 256 different values for RGB

# Chroma Sampling
- Throwing away color data, but not luminance.
- 4:4:4
	- don't throw anything away
	- this is good for chroma key because the edges of the color are more crisp and thus better for keying
- 4:2:2
	- given a set of 4 pixels, keep color for two of them and replicate it for the others.
	- since luminance is not thrown, they would have different shades (light green, green, dark green)
- 4:2:0
	-  given 4 pixels, only use color for one of them

# Spatial Compression
- cut up the image into blocks of similar color
- a completely black screen does not need to waste color values for all pixels
- down-side. If compression is too agressive, you see blocks of same color (not necessarily square). Like army stripes

# Temporal Compression
- Find the difference from one frame to the other. If the background does not change then no need to spend extra space on replicating it, just reference previous frame.
- AKA Long-GOP AKA Long-group-of-pictures
- works along side spatial compression
- Down-sides
	- out of 30 frames. Frame 0 is original frames and frames `0<n<30` keep the diff of previous frames. Now, if you're editing and you go to frame 28, the computer has to claculate the diff of each previous frames to render frame 28. At frame 30 (zero-based) you get the frame right away. This means going backwards will show stutter.

# Bit Rate
- how much data the codec uses
- Measured in bits per second (kbps or kb/s)
- Effect on the image depends on the codec. Some codecs have "sweet spot" like 5-20 Mbps.
	- The best way to find out is to just try it out and see if it looks good
	- A lower bitrate means more compression (which is dependent on the scene and codec)
- generally, the higher the bitrate the better the image (but is dependent on codec)
	- H.264 @ 8 Mbps > MPEG-2 @ 20 Mbps

# RAW
- This is still compressed in reality
- Benefits are similar to uncompressed video (no banding, don't see blocks)
	- Uncompressed
		- 	data from sensor is still mannipulated. Camera manipulates image
	- RAW
		- no processing in the camera. The

