# RSP1Adump1090
ADS-B receiver dump1090 progam for SDRPLay RSP1A SDR boards<br/>
<br/>
I own an SDRPlay RSP1A SDR board, <br>
and I wanted to use it to receive ADS-B planes signals and report planes positions to FlightAware and FligtRadar24 websites.<br/>
<br/>
I also don't want to use a dedicated PC to do this job, and wanted to use my Raspberry Pi4 instead.<br/>
<br/>
So I started by installing on the Raspberry the PiAware software from FlighAware.<br/>
They provide a Raspberry Pi image that you can download from :<br/>
<ul>
  <li><a href='https://fr.flightaware.com/adsb/piaware/build'>fr.flightaware.com/adsb/piaware/build</a></li>
</ul><br/>
<br/>
Once installed on your Raspberry, the PiAware software manage the SDR board using a program named <b>dump1090</b> who is dedicated for <b>RTL2832U</b> SDR boards, but not for the RSP1A that I own.<br/>
<br/>
Fortunately, the SDRPlay company have adapted this <b>dump1090</b> program for they boards, <br/>
and you can download the source code from their Github at address : <br/>
<ul>
 <li><a href='https://github.com/SDRplay/dump1090'>github.com/SDRplay/dump1090</a></li>
</ul><br/>
<br/>
This project is a fork that I made from their Github, <br/>
and contains all the adaptations that I had to do in order to be able to compile their source code on my Raspberry Pi running the PiAware image.<br/>
It also contains the result of this compilation which is the dump1090 executable for RSP1A boards.<br/>
<br/>
Normally, all you have to do is to clone my project, <br/>
and copy the <b>runDump</b> shell and the <b>dump1090</b> directory into your home directory on your Raspberry.<br/>
<br/>
Then, you can start the dump1090 in interactive mode using the "<b>./runDump</b>" bash command.<br/>
<br/>
You can have a look at my website <b>www.f4laa.fr</b> where i wrote an article on this ADS-B subject.<br/>
<ul>
 <li><a href='https://www.f4laa.fr/index.php/2024/02/28/ads-b-decodage-des-avions-avec-sdrplay-rsp1-a/'>www.f4laa.fr/index.php/2024/02/28/ads-b-decodage-des-avions-avec-sdrplay-rsp1-a/</a></li>
</ul><br/>



