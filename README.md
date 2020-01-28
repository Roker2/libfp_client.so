By Roker2

## libfp_client.so

Need to change B.NE loc_XXXXX to NOP

NOP = 1F 20 03 D5 in HEX

Based on comparing Xiaomi Redmi 4X blobs

Maybe need to patch Aliplay functions

| Function                                 | Patch place | Patch status (patched or not) |
| :--------------------------------------- | :---------- | :---------------------------- |
| BpFingerPrint::gfCmdM                    | 150E0       | no                            |
| BpFingerPrint::delFpTemplates            | 15D70       | no                            |
| BpFingerPrint::cancelRecognize           | 15E48       | no                            |
| BpFingerPrint::recognize                 | 162F0       | no                            |
| BpFingerPrint::saveRegist                | 163DC       | no                            |
| BpFingerPrint::unRegist                  | 164C8       | no                            |
| BpFingerPrint::cancelRegist              | 16748       | no                            |
| BpFingerPrint::regist                    | 1681C       | no                            |
| BpFingerPrint::load_all_fpdata           | 16A24       | no                            |
| BpFingerPrint::set_user_id               | 16FB4       | no                            |
| BpFingerPrintService::connect            | 1A72C       | no                            |