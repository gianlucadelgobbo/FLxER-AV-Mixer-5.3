///////////////////////////////////////////
/                                         /
/ XXXXX X     X   X xxxxx xxxx            /
/ X     X      X X  x     x   x           /
/ XXX   X       X   xxx   xxxx            /
/ X     X      X X  x     x  x            /
/ X     XXXXX X   X xxxxx x   x     MIDI  /
/                                         /
///////////////////////////////////////////

README

ITALIANO
installazione:
- copia i file libmmj.jnilib e mmj.jar che si trovano nella cartella Extensions4osX nella cartella /Library/Java/Extensions del tuo sistema
se la cartella Extensions non esiste va creata (Attenzione alle maiuscole, OS X è case sensitive)


utilizzo:
- collegare un dispositivo midi al computer
- lanciare l'applicazione midiToFLxER.app
- selezionare dalla lista di dispositivi il dispositivo midi che si intende utilizzare
- scegliere se tracciare tutti i comandi midi (sconsigliato, usare solo durante i test) selezionando il checkbox "trace"
- cliccare sul tasto "START"
- lanciare FLxER ed attivare la funzionalità midi sulla pulsantiera in alto
- enjoy FLxER 

messaggi di errore:

System doesn't have any midi devices installed. Application cant start
Il software non ha rilevato nessun dispositivo midi installato e non è in grado di continuare; l'esecuzione viene interrotta.

soluzione:
configurare correttamente il dispositivo midi o installare eventuali driver disponibili.
Per verificare il corretto funzionamento del dispositivo midi usa MIDI Monitor disponibile qui: http://www.snoize.com/MIDIMonitor/ 


Cant find midi preferences XML file.
Il software non trova il file di preferenze.
viene aperta una finestra per selezionare il percorso del file midiPref.xml

soluzione:
trovare all'interno del proprio computer il file midiPref.xml
il file è contenuto in questo pacchetto e dovrebbe essere stato copiato nella cartella FLxER/preferences/midiPref.xml 
---------------------------------------

ENGLISH
installation:
- copy libmmj.jnilib and mmj.jar from Extensions4osX folder to /Library/Java/Extensions of your system
If Extensions folder doesn't exist create it.(be careful OS X is case sensitive)



USE:
- connect your midi device
- run  midiToFLxER.app application
- select the midi device you want to use from the list
- check the "trace" checkbox if you want to trace all midi command (check this option only for debug)
- click the "START" button
- run FLxER ed activate the midi functionality from top menu
- enjoy FLxER 

error messages:

System doesn't have any midi devices installed.\nApplication cant start
The application doesn't find any midi device. execution will stop

solution:
Configure your midi device or install any available driver.
Download MIDI Monitor from here http://www.snoize.com/MIDIMonitor/ to be sure that your device is correctly setup.


Cant find midi preferences XML file.
The application cant file the midi preference xml file.
Use the file chooser to setup the path of the file

solution:
find in your hard drive the file midiPref.xml
the file comes with this package and is usually located in your FLxER folder  
in preferences/midiPref.xml 
----------------------------------------

- Copy the lines with the functions that you want to use in FLxER in "preferences/midiPref.xml" from the list below and assign the midiID and midiVal (minVal,MaxVal OR 0) values from midiToFLxER.jar trace:

<root>
	<midiCtrl midiID="" fnz="hiQuality" midiVal="0" />
	<midiCtrl midiID="" fnz="fullScreen" midiVal="0" />
	<midiCtrl midiID="" fnz="mouseShowHide" midiVal="0" />
	<midiCtrl midiID="" fnz="topBarShowHide" midiVal="0" />
	<midiCtrl midiID="" fnz="bottomBarShowHide" midiVal="0" />
	<midiCtrl midiID="" fnz="moveDown" ch="auto" midiVal="0" />
	<!--
	<midiCtrl midiID="" fnz="moveDown" ch="1" midiVal="0" />
	<midiCtrl midiID="" fnz="moveDown" ch="2" midiVal="0" />
	<midiCtrl midiID="" fnz="moveDown" ch="3" midiVal="0" />
	<midiCtrl midiID="" fnz="moveDown" ch="4" midiVal="0" />
	<midiCtrl midiID="" fnz="moveDown" ch="5" midiVal="0" />
	<midiCtrl midiID="" fnz="moveDown" ch="6" midiVal="0" />
	<midiCtrl midiID="" fnz="moveDown" ch="7" midiVal="0" />
	>-->
	<midiCtrl midiID="" fnz="moveUp" ch="auto" midiVal="0" />
	
	<midiCtrl midiID="" fnz="live" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="hideShow" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="stopPlay" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="rewind" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="tap" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="eject" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="reset" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="lockWipes" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="libraryScroller" val="1" ch="auto" midiVal="0" />	
	<midiCtrl midiID="" fnz="libraryScroller" val="-1" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="zoomOneByOne" val="1,-1" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="sliderOneByOne" val="1,-1" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="zoom" val="1,1600" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="rotate" val="1,1600" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="scratch" val="0,800" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="slider" val="0,100" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="movieScroller" val="1,-1" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="changeChannel" val="2,7" ch="auto" midiVal="0" />

	<midiCtrl midiID="" fnz="redMovie" val="-255,255" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="greenMovie" val="-255,255" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="bluMovie" val="-255,255" ch="auto" midiVal="0,7F" />

	<midiCtrl midiID="" fnz="bkgOnOff" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="redMovieB" val="-255,255" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="greenMovieB" val="-255,255" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="bluMovieB" val="-255,255" ch="auto" midiVal="0,7F" />

	<midiCtrl midiID="" fnz="blendScroller" val="-1" ch="auto" midiVal="0" />
	<midiCtrl midiID="" fnz="blendScroller" val="1" ch="auto" midiVal="0" />

	<midiCtrl midiID="" fnz="wipeScroller" val="-1" ch="auto" midiVal="0" />	
	<midiCtrl midiID="" fnz="wipeScroller" val="1" ch="auto" midiVal="0" />	

	<midiCtrl midiID="" fnz="quickContent" val="1" ch="auto" />
	<midiCtrl midiID="" fnz="quickContent" val="2" ch="auto" />
	<midiCtrl midiID="" fnz="quickContent" val="3" ch="auto" />

	<midiCtrl midiID="" fnz="rotate" val="1,1600" ch="auto" midiVal="0,7F" />	


	<midiCtrl midiID="" fnz="soloPress" val="127" ch="auto" midiVal="0" />	
	<midiCtrl midiID="" fnz="soloRelease" val="0" ch="auto" midiVal="0" />	

	<midiCtrl midiID="" fnz="hueMovie" val="0,360" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="satMovie" val="-300,300" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="conMovie" val="-200,500" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="briMovie" val="-255,255" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="thrMovie" val="0,255" ch="auto" midiVal="0,7F" />
	<midiCtrl midiID="" fnz="thrOnOff" ch="auto" midiVal="0" />
</root>
</root>

- Close and save the file "preferences/midiPref.xml"

- Unselect "Trace"

- Press start

- Run FLxER

- Activate MIDI from top right

- EnjoyMidi

for any question please contact the authors at info@flxer.net

FLxER
http://www.flxer.net

Used software:
java version "1.5.0_06"
Java(TM) 2 Runtime Environment, Standard Edition (build 1.5.0_06-b05)
Java HotSpot(TM) Client VM (build 1.5.0_06-b05, mixed mode)