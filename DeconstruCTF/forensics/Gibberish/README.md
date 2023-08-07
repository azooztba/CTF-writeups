## Deconstruct CTF 2023
Category: forensics<br>
Name: Gibberish<br>
Points: 50<br>
Description: `NASA receive a weird transmission yesterday but they were't able to decode it. I mean, it's just a bunch of gibberish. The only thing they have cracked was one word "goodbye". They have no clue what that means though. Can you help them?`<br>

I downloaded the attached file [flag.txt](https://github.com/azooztba/CTF-writeups/blob/main/DeconstruCTF/forensics/Gibberish/resourses/flag.txt). after looking at the contents of the file it looked like it was Base64 encoded.<br>
So i went to [cyberchef](https://cyberchef.org/) and used the <b>From Base64</b> on the file as in this img:<br>
<img src="https://github.com/azooztba/CTF-writeups/blob/main/DeconstruCTF/forensics/Gibberish/resources/cyberchef_screenshot.png"><br>
press on save output to file.<br>
I examined the [download.elf](https://github.com/azooztba/CTF-writeups/blob/main/DeconstruCTF/forensics/Gibberish/resources/download.elf) file in a text editor and i found this interesting text:<br>
<img src="https://github.com/azooztba/CTF-writeups/blob/main/DeconstruCTF/forensics/Gibberish/resources/ELF_screenshot.png"><br>
if we put it in the flag format we get: <b>mlh{nc_c4n_4ls0_trnsmit_f1les}</b>
