# RSP1Adump1090
ADS-B receiver <b>dump1090</b> progam for SDRPLay RSP1A SDR boards<br/>
<br/>
I own a SDRPlay RSP1A SDR board, and I wanted to use it to receive ADS-B planes signals <br/>
and report planes positions to <b>FlightAware</b> and </b>FlightRadar24</b> websites.<br/>
<br/>
I also don't want to use a dedicated PC to do this job, and planned to use my Raspberry Pi4 instead.<br/>
<br/>
So I started by installing on the Raspberry the PiAware software from FlighAware.<br/>
They provide a Raspberry Pi image that you can download from :<br/>
<br/>
<ul>
  <li><a href='https://fr.flightaware.com/adsb/piaware/build'>fr.flightaware.com/adsb/piaware/build</a></li>
</ul>
<br/>
Once installed on your Raspberry, the PiAware software manage the SDR board using a program named <b>dump1090</b> who is dedicated for <b>RTL2832U</b> SDR boards, but not for the RSP1A that I own.<br/>
<br/>
Fortunately, the SDRPlay company have adapted this <b>dump1090</b> program for they boards, <br/>
and you can download the source code from their Github at address : <br/>
<br/>
<ul>
 <li><a href='https://github.com/SDRplay/dump1090'>github.com/SDRplay/dump1090</a></li>
</ul>
<br/>
This project is a fork that I made from their Github, and contains the adaptations that I had to do <br/>
in order to be able to compile their source code on my Raspberry Pi running the PiAware image.<br/>
It also contains the result of this compilation which is the <b>dump1090</b> executable for RSP1A boards.<br/>
<br/>
Normally, all you have to do is to clone my project, <br/>
copy the <b>runDump</b> shell and the <b>dump1090</b> directory into your home directory on your Raspberry.<br/>
<br/>
Then, you can start the dump1090 in interactive mode using the "<b>./runDump</b>" bash command.<br/>
<br/>
For more information on this project, you can have a look at my website <b>www.f4laa.fr</b> where i wrote an article on this ADS-B subject.<br/>
<br/>
<ul>
 <li><a href='https://www.f4laa.fr/index.php/2024/02/28/ads-b-decodage-des-avions-avec-sdrplay-rsp1-a/'>www.f4laa.fr/index.php/2024/02/28/ads-b-decodage-des-avions-avec-sdrplay-rsp1-a/</a></li>
</ul>



