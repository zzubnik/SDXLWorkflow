# SDXLWorkflows
Basic SDXL workflows for ComfyUI. I prefer things to be lined up.


## SDXL Refiner
[SDXL_Refiner.json]([url](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_Refiner.json)) - Requires RGThree nodes, but only for the seed node. Setup layout assumes Preview method: Auto is set.

![WorkflowPreview](https://github.com/zzubnik/SDXLWorkflow/assets/24965799/9a1eb0bf-3c3e-4d0c-afe8-3654918c356e)


## SDXL Refiner with upscale node
[SDXL_RefinerUpscaler.json]([url](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_RefinerUpscaler.json)) - The same, but with an upscale node added. Mute to ignore upscale.


## SDXL Refiner with LORA and upscaler
[SDXL_RefinerUpscalerLora.json]([url](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_RefinerUpscalerLora.json)) - The same as above, but with a Lora node.

![WorkflowPreviewlora](https://github.com/zzubnik/SDXLWorkflow/assets/24965799/d274f364-c0cf-4633-bc3b-64f850d0e053)


## SDXL CLIP image combiner
[SDXL_CLIPVisionCombiner.json]([url](https://github.com/zzubnik/SDXLWorkflow/blob/main/SDXL_CLIPVisionCombiner.json)) - Loads two images, looks at them, then combines the results. Your milage may vary. I Need to add refiner node. Ther results can be pretty bad.
![WorkflowPreviewCLIPCombiner](https://github.com/zzubnik/SDXLWorkflow/assets/24965799/0b4a4fe0-88b7-4017-9b7e-57276d19f5d1)
