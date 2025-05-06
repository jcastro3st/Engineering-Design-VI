# Lab 9 - YANG
## Engineering-Design-VI CPE-322
## Written by Jacqueline Castro

In this lab, we will be using pyang and PlantUML We will be converting YANG modules to YIN, generating visual diagrams, and viewing the diagram using pinta/GIMP.

---

To begin, we will be using the command cat for intrusiondetection.yang, converting to yin, command cat for intrusiondetection.yi, converting to uml, command cat for intrusiondetection.uml, and running intrusiondetection.uml using plantuml.

`cat intrusiondetection.yang`

<img width="467" alt="Image" src="https://github.com/user-attachments/assets/72c79034-7058-4342-a03a-4e110655ba7b" />

<img width="468" alt="Image" src="https://github.com/user-attachments/assets/7f0d18fe-c7c2-4f61-bb7e-677d03a4e237" />

<img width="469" alt="Image" src="https://github.com/user-attachments/assets/9d47fc73-52c1-4320-b452-9bdfa8eb9f12" />

<img width="469" alt="Image" src="https://github.com/user-attachments/assets/ba681307-fec1-4094-9bcd-cf61157513f7" />

<img width="469" alt="Image" src="https://github.com/user-attachments/assets/b3795706-9004-4654-949e-099c8522e56f" />


`pyang -f yin -o intrusiondetection.yin intrusiondetection.yang`

`cat intrusiondetection.yin`

<img width="467" alt="Image" src="https://github.com/user-attachments/assets/1c090f60-4ec9-4f99-a386-d95cbe546413" />

<img width="470" alt="Image" src="https://github.com/user-attachments/assets/6339d74f-f6b4-4230-baf2-100e965a8002" />

<img width="467" alt="Image" src="https://github.com/user-attachments/assets/9c43d5d4-c13b-4320-8135-27fde06b7926" />


`pyang -f uml -o intrusiondetection.uml intrusiondetection.yang-uml-no=stereotypes,annotation,typedef`

`cat intrusiondetection.uml`

<img width="834" alt="Image" src="https://github.com/user-attachments/assets/36455ab6-b749-4526-94a8-3cc6bf737716" />

---

Intrusion Detection Display:

`open -a Pinta intrusiondetection.png`

<img width="464" alt="Image" src="https://github.com/user-attachments/assets/7cb90ed4-4066-4b4b-9736-679b323ea42c" />

`gimp -h`

<img width="405" alt="Image" src="https://github.com/user-attachments/assets/593e3590-f70b-4d31-8ca4-754076f1a879" />

`gimp -a intrusiondetection.png`

<img width="468" alt="Image" src="https://github.com/user-attachments/assets/aef1358c-993e-4256-b61a-76fb8cafb40f" />

