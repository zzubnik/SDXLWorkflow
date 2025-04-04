This is so out of date. I would be highly surprised if it works at all. 

# SDXLWorkflows
Basic SDXL workflows for ComfyUI. I prefer things to be lined up. Images in the middle with the controls around that for quick navigation. This repository is really just to help me keep track of things while I learn and add new developments from the community.

## Current general setup.
[SDXL_V3_2.json](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_V_3_2.json) -  Redesigned to use switching on and off of parts of the process. Refiner, face fixer, one LoRA, FreeUV2, Self-attention Guidance, Style selectors, better basic image adjustment controls. Bypass things you don't need with the switches. Added film grain and chromatic abberation, which really makes some images much more believable.

This new version can replicate IMG2IMG or image feedback. Enable Input Image When you generate an image you like, right-click on it in the Refined Image window and choose Copy (Clipspace). Right-click on the Load Image window and choose Paste (Clipspace). Adjust the Denoise to a value that works. Start with .75 and see how much the image changes. Change the text to change the output. Feed that back in, etc. 
Make sure to set Denoise to 1.0 when not using image input or you will get noise.

Glow replaced with faster and better Bloom filter. Comparison preview image added to the Load Image box.

Time to reorganize. The layout has sprawled.

![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/images/SDXL_V_3_2.JPG)

## Everything below here is older.
[SDXL_V3_0.json](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_3_0.json) -  Redesigned to use switching on and off of parts of the process. Refiner, face fixer, one LoRA,  FreeUV2, Style selectors, and basic image adjustment controls. Bypass things you don't need with the switches.

![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/images/SDXL_3_0.JPG)

[SDXL_V2_0.json](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_V2_0.json) -  Refiner, face fixer, one LoRA,  FreeUV2 (which I don't like and bypass), Style selectors, Latent upscale (weird), and basic image adjustment controls. Bypass things you don't need. I usually have the face and hand fixer bypassed as well as the latent upscale group, which really is pretty useless. I think I'll remove it for the next version. There is a row of collapsed nodes. Just right-click and choose Bypass to turn them off.

![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/images/SDXL_V2_0.JPG)

## Older general setup.
[SDXLworkflow_11_11.json](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXLworkflow_11_11.json) -  Includes refiner, face fixer, one LoRA,  FreeUV2 (which I don't like and bypass), and basic image adjustment controls
![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/images/general_sdxl_11_11.JPG)

## IMG2IMG version of general setup.
[SDXL_img2Imgworkflow_15_11.json](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_img2Imgworkflow_15_11.json) -  Includes refiner, face fixer, one LoRA,  FreeUV2 (which I don't like and bypass), and basic image adjustment controls
![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/images/SDXL_img2Imgworkflow_15_11.JPG)


## An older general setup Includes 2x loRA and upscaling.
workflow_SDXL_2LORA_Upscale.json - Requires RGThree nodes, and JPS Nodes. Setup layout assumes Preview method: Auto is set and link render mode is set to hidden.
![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/images/workflow_SDXL_2LORA_Upscale.JPG)

## general setup Includes LOrA and upscaling.
SDXL_WorkflowCombinedTidy.json - Requires RGThree nodes, but only for the seed node. Setup layout assumes Preview method: Auto is set.
![WorkflowCombinedOrganised](https://github.com/zzubnik/SDXLWorkflow/assets/24965799/86b1161a-3e58-4474-94ec-05ba8073c376)


## SDXL Refiner
[SDXL_Refiner.json]([url](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_Refiner.json)) - Requires RGThree nodes, but only for the seed node. Setup layout assumes Preview method: Auto is set.

![WorkflowPreview](https://github.com/zzubnik/SDXLWorkflow/assets/24965799/9a1eb0bf-3c3e-4d0c-afe8-3654918c356e)


## SDXL Refiner with upscale node
[SDXL_RefinerUpscaler.json]([url](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_RefinerUpscaler.json)) - The same, but with an upscale node added. Mute to ignore upscale.


## SDXL Refiner with LORA and upscaler
[SDXL_RefinerUpscalerLora.json]([url](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_RefinerUpscalerLora.json)) - The same as above, but with a Lora node.

![WorkflowPreviewlora](https://github.com/zzubnik/SDXLWorkflow/assets/24965799/d274f364-c0cf-4633-bc3b-64f850d0e053)


## SDXL CLIP image combiner
[SDXL_CLIPVisionCombiner.json]([url](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_CLIPVisionCombiner.json)) - Loads two images, looks at them, then combines the results (beach, woman). Your milage may vary. The results can be pretty bad.
![WorkflowPreviewCLIPCombiner](https://github.com/zzubnik/SDXLWorkflow/assets/24965799/0b4a4fe0-88b7-4017-9b7e-57276d19f5d1)
