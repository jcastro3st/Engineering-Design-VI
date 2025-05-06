# Lab 1 - GTKWave and GHDL
## Engineering-Design-VI CPE-322
## Written by Jacqueline Castro

In this lab, we will be utilizing GTKWave, GHDL, and Notepad++. GTKWave is used to be able to visualize data, 
both analog and digital, as well as facilitate various search operations and allow users to save certain signals 
that are extracted from a complete simulation dump. GHDL is described as an open-source simulator for the VHDL 
language. It also compiles and executes VHDL code in a computer.  Notepad++ is a free source code editor that allows 
a user to use various languages. The goal of this lab is to explore the capabilities of GTKWave, GHDL, and Notepad++ 
by creating and testing a simple half adder code.

**Notepad++ ha.vhdl**

<img width="624" alt="Image" src="https://github.com/user-attachments/assets/639b67ef-aa2d-4d37-9189-8e771fa42381" />


**Notepad++ Test Block for Half-Adder ha_tb.vhdl**

<img width="500" alt="Image" src="https://github.com/user-attachments/assets/d3407fe2-a925-416c-86f3-ce000b948328" />


**Command Prompt GHDL scans for errors, analyze, and execute the files**

`ghdl -a ha_vhdl`

`ghdl -a ha_tb.vhdl`

`ghdl -e ha_tb`

`ghdl -r ha_tb`

`ghdl -r ha_tb --vcd=ha.vcd`

<img width="498" alt="Image" src="https://github.com/user-attachments/assets/c0dd4fef-2d26-4379-a25b-79c80e8566e3" />


**Command Prompt GTKWave runs simulation and displays signals**

`gtkwave ha.vcd`

<img width="497" alt="Image" src="https://github.com/user-attachments/assets/29d15f51-6cc8-49bc-95fb-ef9540fbce84" />


**Signal produced at different values**

<img width="501" alt="Image" src="https://github.com/user-attachments/assets/9d464cfb-8735-4dc1-a6c4-7a0c93687eab" />

<img width="502" alt="Image" src="https://github.com/user-attachments/assets/efc67df5-d112-494d-aa79-0e8480a1db36" />

<img width="497" alt="Image" src="https://github.com/user-attachments/assets/a2976bfb-ec1e-452d-b2ea-67a5d9eff3ca" />

<img width="498" alt="Image" src="https://github.com/user-attachments/assets/fabdaa85-b551-4297-b2d5-8a8aa77665e4" />

---

### D Flip-Flop
We will be performing the same process, but with a D flip-flop instead. We began by creating the vhdl file with 
inputs clock, reset, en, and d as well as output q. We also set the behavior for the process of q according to clock, 
reset, en, and d.

**Notepad++ dff.vhdl**

<img width="497" alt="Image" src="https://github.com/user-attachments/assets/ef476b97-f051-4f44-a2ce-c69e4c22b161" />


**Notepad++ dff_tb.vhdl**

<img width="501" alt="Image" src="https://github.com/user-attachments/assets/742e22b1-72e3-4c7f-a7e7-d41509435a61" />


**Command Prompt for ghdl/gtkwave**

`ghdl -r dff_tb`

`ghdl -s dff.vhdl`

`ghdl -s dff_tb.vhdl`

`ghdl -a dff.vhdl`

`ghdl -a dff_tb.vhdl`

`ghdl -e dff_tb`

`ghdl -r dff_tb`

`ghdl -r dff_tb --vcd=dff.vcd`

`gtkwave dff.vcd`

<img width="497" alt="Image" src="https://github.com/user-attachments/assets/5dfdfecd-da8b-4561-bfad-19d948e8c283" />

<img width="499" alt="Image" src="https://github.com/user-attachments/assets/39c31d89-1a1f-42dd-a573-75f5d4c28f28" />

**Signal produced**

<img width="498" alt="Image" src="https://github.com/user-attachments/assets/98adce77-07a2-4d20-af22-3f17a954a5df" />
