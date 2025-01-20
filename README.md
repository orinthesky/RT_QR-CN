# RT_QR-CN
A real time workflow for diffusing generative visuals in ComfyUI/ComfyStream

Created by FungAI - @orinthesky

This is a real time diffusion workflow using any black and white generative source as the input.
Using the QR Monster v2 ControlNet, the black and white input source drives the motion of the diffusion. With a fixed seed and unchanging prompt, the QR allows for continuous change in the output, while maintaining temporal consistency.  The input used for development was the "Equirectangular" source in Synesthesia Live, allowing for realtime midi input to drive the movment pattern.  

This workflow can run very fast as it uses only one ControlNet, so I provided two versions of the API workflow.  The first is a single render pass setup which is very fast, and the other does two render passes, one at full denoise and one at only 40% so as to effectively enhance and smooth the ouput.
