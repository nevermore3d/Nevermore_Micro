<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <https://github.com/0ndsk4/VoronUsers/tree/0ndsk4/printer_mods/0ndsk4/Nevermore_Air_Filter/Nevermore_Micro/">
    <img src="images/logo.png" alt="Logo" width="1000" height="500">
  </a>

  <h3 align="center">Nevermore Micro Air Filter</h3>

  <p align="left">
    Welcome to the Nevermore Micro repo! Intended as a carbon fume filter for Voron V2, it has found its way into a multitude of other machines. Let yours be the next!<BR><BR>
	The current NM Micro versions are V4 and V5 Duo. V4 utilizes a single dissected 5015 fan that is glued in place to spread the airflow over the entire filter surface (something nigh impossible to do with an intact scroll, which focuses the air too much). 
	V5 Duo uses two blowers in paralell to achieve a more even spread of airflow while keeping the pressure-generating scrolls intact, but still needs some slight modifications to the scroll exhaust. Since you are commiting fan dissection, be aware a 5015 used for a NM Micro will most likely never find a different purpose!<br><BR>
	WHATS NEW IN V5?<br>
	* Exhausts upwards; 1) better heat spread in the chamber, and 2) less air leaks through v2 split doors.<BR>
    * BOM 6x3 magnets are standard<br>
	* Blower fans are seated by bolts again, with less modification needed.<br>
	* Check out assembly images (**take note at how the fans are cut!**) here: [Nevermore V5 Plenum Assembly Album](https://ibb.co/album/0BN405?sort=name_asc&page=1&params_hidden%5Blist%5D=images&params_hidden%5Bfrom%5D=album&params_hidden%5Balbumid%5D=0BN405)
	
	WHY USE A SINGLE FAN VERSION, IF DUAL IS BETTER?
	Dual is not better. The area per blower is halved, so what is gained in air flow is lost in increased restriction per blower. There should be some improvements though, from linear air flow and intact scroll.
	
	WHAT FANS SHOULD i USE?
	Aim for any 5015 blower with a rating above 200Pa / 20mmH2O / 1 inH2O. Since the fan (probably) cant be reused for other projects and will function in a high temp environment affecting its lifetime, go for budget. Two good fans for this is the $6-8 Sunon Maglev MF5015VX (high speed version, 6000 rpm. The 5000 rpm might be okay also) and the $4-6 GDStime 6000rpm Dual Ball bearing on Aliexpress.
 
 <img src="images/DUO_COMBINED_render.png" alt="NevermoreV5">
	<BR></BR>
    <https://github.com/0ndsk4/VoronUsers/tree/0ndsk4/printer_mods/0ndsk4/Nevermore_Air_Filter/Nevermore_Micro"><strong>Explore the Nevermore »</strong></a>
    <br />
    <br />
    <a href="https://github.com/0ndsk4/VoronUsers/tree/0ndsk4/printer_mods/0ndsk4/Nevermore_Air_Filter/Nevermore_Micro">Nevermore Air Filter</a>
    ·
    <a href="https://github.com/0ndsk4/VoronUsers/tree/0ndsk4/printer_mods/0ndsk4/Nevermore_Air_Filter/Nevermore_Micro/issues">Report Bug</a>
    ·
    <a href="https://github.com/0ndsk4/VoronUsers/tree/0ndsk4/printer_mods/0ndsk4/Nevermore_Air_Filter/Nevermore_Micro/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#About-The-Nevermore">About The Nevermore</a>
      <ul>
        <li><a href="#Why">Why Nevermore?</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#BOM">BOM</a></li>
        <li><a href="#installation">Installation</a></li>
		<li><a href="#Built-with">Built with</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Nevermore Micro

 <img src="images/print_example2.png" alt="NevermoreV2">

<B>NEVERMORE V4</B><br>
Nevermore V4 is a refinement of the V3. V4 adds a air guides, as the previous versions had the majority of air flow on just one side of the filter (most recent version has all supports removed yet again!). The cartridge lid also mounts a bit sturdier, and V4 now has separate base pieces for use with vorons other than 2.4.


<B>NEVERMORE BACKGROUND</B><br>
There are many options for 3d printing air filters. Here’s a short list, and why I eventually settled on creating Nevermore:<br>
<B>1.	Home air purifiers</B><br>
a.	PRO: Plug and play! High air flow (mostly). Will filter most particles a 3d printer produces.<br>
b.	CON: ABS headaches are not from particles, but Volatile Organic Compounds (VOCs), that are two orders of magnitude smaller than any particles a HEPA or ULPA could trap - they’re essentially gasses. <br>
While home purifiers typically also contains carbon filtration and/or photocatlytic UV filtration stages, they will still not be suitable for 3d printing. Why? Efficient carbon adsorbtion in sufficient amount and stages is an absolute airflow killer, so most purifiers contain only a thin layer of carbon mesh/pellets that will be fully adsorbed within days or weeks at full power. And even if the filter is not used, contact with air saturates the carbon in 1-2 months. Yet they’re advertised as lasting for 6 months – that's only true for the hepa component, not the VOC adsorbant carbon we're after. <br>And replacement filters typically run 20-60 US a pop. Quite alot for changing every few weeks when the carbon component depletes.<br>
UV photocatalyst activity can last though, but breakdown is slow and inefficient, with voc halflives of several hours. The TiO2 layer reacting to the UV will also easily get irreversably blocked by silicates (of which there are alot in peoples homes, in everything from sink and bathroom sealants to plaster walls). And breakdown will many times be incomplete. Styrene passing a PCO filter might get turned to even more dangerous benzene, for instance.<br><br>
<B>2.	Carbon/HEPA filter combinations</B> like the zortax (https://spool3d.ca/zortrax-m-series-hepa-filter-3-pack/)<br>
a.	Same as above. The HEPA component will keep working, but the carbon is just a few pebbles per hex. It could provide partial VOC clearance when fresh, but will quickly deplete with air flow. Then you need to replace it for 36 US after a week of printing.<br>
<B>3.	Wet scrubber</B><br>
a.	Awesome for both particles and VOCs, but its an industrial solution with any smaller home versions plagued by loud noise, water leakage and mechanical issues. Its not a solution for the masses.<br>
So, how about Nevermore? Well, the carbon in those filters mentioned above, costing alot for little duration is actually dirt cheap. Whereas you get 20 grams for 36 US with a zortax filter, you can get 5000 grams for 36 US in bulk. And with an enclosed chamber, you dont need the air flow of a room-size air purifier. Even a 350mm V2 Voron only holds about 5cf, meaning even a partial flow from a 5015 fan of 0.5-2cfm is enough to filter the fumes efficiently at the source.<br>
So what are we waiting for? We got lots of cheap carbon. We can replace is easily. We dont need high airflow to clean a small chamber. We deal with poor efficiency of one-pass carbon filters by multiplying the amount and recirculate the air. <br>Enter Nevermore.<br><br>

### Why

At the end of the day, a fresh single-pass filtered exhaust (at brand new) has perhaps 70% VOC removal efficiency while still exhausting 30% of the nasty. A recirculation filter achieving four passes at worn-in 50% efficiency would still remove 94% of the bas stuff. Or 99% at six passes! <BR>
The number of passes you get all depends on how well you can seal your build chamber.<br><BR>
Some will have a hard time achieving a good chamber seal, which creates the biggest drawback of recirculation filters - they're air flow neutral. Meaning, as nothing pulls air into the chamber, air can diffuse freely to the outside through any remaining gaps. And that air could be <i>zero per cent</I> cleaned... If you plan on using only a Nevermore Micro - be sure to seal your chamber as good as possible.<BR><BR>



<!-- GETTING STARTED -->
## Getting Started

You're ready to build a Nevermore Micro? Cool!

### BOM (V4)

<B>MADE FOR ABS/PC/PETG - USE A DECENTLY HEAT RESISTANT FILAMENT!</b> <br>


<B>FANS</b><br>
* ONE 5015 BLOWER FAN, CUT UP SO JUST THE CENTER REMAINS (take off the top half, cut the bottom piece circular along the fan blades). We aim for removing the focused air stream and instead achieve an even pressure across all of the filter medium.

<B>PRINTED PARTS:</b><br>
Nevermore Micro has Three main parts: <B>Base, Plenum</b>, and <B>Cartridge</B> (plus lids for the plenum/cartridge. <BR>

* <b>Base</B> is mounted in the 130mm space between the bottom extrusions found on many vorons (designed for v2 originally). It’s seated with one m3 on each side, that screws into to a receiving 2020 M3 T-nut.<BR> 

*<b>Plenum</B> holds the cut up 5015 fan, and is seated with two m3 screws into the base (base has two recieving m3 4mm heat inserts) on each side<BR>

*<b>Cartridge</B> holds the filter medium of your choice (made for 4mm air filter active carbon pellets, but feel free to filter with what you think works best!). It snaps onto the Plenum piece for easy and quick removal.

<B>BOLTS/INSERTS/MAGNETS for v4:</b><br>
* **4 X** Heat inserts (M3,5x4mm, standard voron issue). <BR>
-2 for seating plenum to base.<BR>
-2 for seating plenum lid to plenum.<BR>
-**2 x** m3 2020 T-Nuts<br>
* **8 x** 4x6 mm OR 6x3 cylindrical magnets.<br>
* M3 SHCS/BHCS (6-10mm, use what works/looks best!)<BR><br>

<B>Filter medium:</b><br>
4mm Active carbon Air Filter Pellets (see Nevermore BOM for useful/important carbon info!)

### Installation

~~1. Place 4 inserts (2 plenum, 2 on base).<br>
2. <s>Remove support material from PLENUM</s> <br>
3. Disassemble a 5015 fan (200+ Pa static pressure recommended), bu cutting it flat/circular (optionally use cutting guide stl). Seat it absolutely centered on the PLENUM HEX piece with a bit of glue or VHB tape (there should be 1.6-2mm of clearance to the plenum lid to work with) and with the wires along the markings. <br>
4. Lead fan wire along to the cutout on the back, and then glue the hex piece to the plenum. It only fits one way.<br>
5. Glue 8 magnets (cylindrical 4x6mm) to the corresponding holes on the plenum and cartridge, so the pieces can snap together. 
6. Add LID Piece to Plenum with 4x m3 x 6mm (BHSC, back two with inserts, front two are just threaded). NOTE: The lid have to bent slightly while installing as the intake hole extends down and have to pass over the plenum vanes to get in place - dont't worry, it will fit fine, just dont break the vanes! <br><I>Optionally add a strip of 1.75mm soft TPU filament for additional sealing in the corresponding slot between cartridge/plenum (due to the printing orientation of the lid, the fit is not optimal, do at your own risk).</i><BR>
7. Remove/lift you v2.4 bed so you can reach about 5-10cm underneath the front of the hot bed.<br>
8. Find a good location for the filter base. When everything is installed, you should be able to remove the cartridge without burning yourself on the bed, and the filter cartridge should not reach all the way to the printer doors.<br>
9. Seat the Base with 2 m3 bolts into two recieving extrusion T Nuts.<br>
10. Seat Plenum to Base with two m3 shcs bolts (6-10mm).<br>
11. Test cartride/plenum/base. The base should not move when snapping on/off cartridge. Tighten as necessary!<br>
12. Re-install your heated bed.<br>
13. Fill cartridge with filter medium, snap on, connect fan wire to mcu and activate in klipper - <br>
14. Enjoy active carbon recirculation. Keep your carbon stash air tight, and change cartridge every 30-40 hrs (tip: print two or more cartridge pieces for fast/quick filter swaps. Keep any unused fresh cartridges in an air tight bag.<br>~~


### Built with
The Voron nevermore Air Filter was modelled in Fusion 360.
* [Fusion 360](http://autodesk.com)

<!-- USAGE EXAMPLES -->


<!-- CONTRIBUTING -->
## Contributing

Please contribute! I'd like to incorporate VOC sensors, making the filter smart (running on low-noise mode at an acceptable VOC level, then ramp up at the end to clean more thoroughly before doors open).


<!-- LICENSE -->
## License

Distributed under GNU General Public License version 3.0 (GPLv3)



<!-- CONTACT -->
## Contact

0ndsk4#5933  - (http://discord.com/user/0ndsk4#5933) <BR>
Nevermore: [https://github.com/0ndsk4/VoronUsers/tree/0ndsk4/printer_mods/0ndsk4/Nevermore_Air_Filter](https://github.com/0ndsk4/VoronUsers/tree/0ndsk4/printer_mods/0ndsk4/Nevermore_Air_Filter)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [The Voron Dev Team](https://vorondesign.com/)






<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[product-screenshot]: images/screenshot.png
