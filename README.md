By Roker2

## libfp_client.so

Need to change B.NE loc_XXXXX to NOP

NOP = 1F 20 03 D5 in HEX

Based on comparing Xiaomi Redmi 4X blobs

Maybe need to patch Aliplay functions

| Function                                 | Patch place | Patch status (patched or not) |
| :--------------------------------------- | :---------- | :---------------------------- |
| BpFingerPrint::gfCmdM                    | 150E0       | yes                           |
| BpFingerPrint::delFpTemplates            | 15D70       | yes                           |
| BpFingerPrint::cancelRecognize           | 15E48       | yes                           |
| BpFingerPrint::recognize                 | 162F0       | yes                           |
| BpFingerPrint::saveRegist                | 163DC       | yes                           |
| BpFingerPrint::unRegist                  | 164C8       | yes                           |
| BpFingerPrint::cancelRegist              | 16748       | yes                           |
| BpFingerPrint::regist                    | 1681C       | yes                           |
| BpFingerPrint::load_all_fpdata           | 16A24       | yes                           |
| BpFingerPrint::set_user_id               | 16FB4       | yes                           |
| BpFingerPrintService::connect            | 1A72C       | yes                           |