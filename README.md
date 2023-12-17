# SDXLWorkflows
Basic SDXL workflows for ComfyUI. I prefer things to be lined up.

## Current general setup.
[SDXL_V2_0.json](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_V2_0.json) -  Refiner, face fixer, one LoRA,  FreeUV2 (which I don't like and bypass), Style selectors, Latent upscale (weird), and basic image adjustment controls. Bypass things you don't need. I usually have the face and hand fixer bypassed as well as the latent upscale, which really is pretty useless. I think I'll remove it for the next version.
![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_V2_0.JPG)

## Older general setup.
[SDXLworkflow_11_11.json](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXLworkflow_11_11.json) -  Includes refiner, face fixer, one LoRA,  FreeUV2 (which I don't like and bypass), and basic image adjustment controls
![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/general_sdxl_11_11.JPG)

## Current IMG2IMG version of general setup.
[SDXL_img2Imgworkflow_15_11.json](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_img2Imgworkflow_15_11.json) -  Includes refiner, face fixer, one LoRA,  FreeUV2 (which I don't like and bypass), and basic image adjustment controls
![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_img2Imgworkflow_15_11.JPG)


## An older general setup Includes 2x loRA and upscaling.
workflow_SDXL_2LORA_Upscale.json - Requires RGThree nodes, and JPS Nodes. Setup layout assumes Preview method: Auto is set and link render mode is set to hidden.
![![WorkflowPreview]](https://github.com/zzubnik/SDXLWorkflow/blob/main/workflow_SDXL_2LORA_Upscale.JPG)

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
