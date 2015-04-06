PINGPONG - Tennisspiel
------------------------------------------------------------------
* Programmerstellung, Programmdokumenation + (C) Copyright, 
  Programmbearbeitung, diese README-Datei

  Rolf Hemmerling
  Erderstr.31
  D30451 Hannover          
  Tel. 0511-2102352
  
* Stand: 1988-01-30, 1995-04-29

------------------------------------------------------------------

Die Bedeutung der D-Schnittstelle war mir damals nicht klar, sie
ist wohl auch erst mit der damals ganz frischen Version 2.1 ins 
RTOS-System gekommen. Das Spiel wurde noch mit Version 2.0 
entwickelt. 

Fuer Ausgaben wird jetzt die D-Schnittstelle verwendet.

Die serielle Schnittstelle ist vor Programmstart auf 19200 Baud
zu stellen mit

<<<<<<<<<<<<<<
SB A2. 19200
>>>>>>>>>>>>>>
 
Das erwaehnte Terminal-Programm PROCOMM liegt mir in seiner letzten
Shareware-Version 2.43 vor, daneben gibt es noch PROCOMM PLUS 1.1.
PROCOMM beansprucht keinen Platz auf dem Bildschirm fuer 
Televideo-Bildschirmattribute, PROCOMM PLUS emuliert das leider
nicht. Daher ist nur PROCOMM kompatibel zum ATARI-Hauptbildschirm.

PROCOMM funktioniert auf meinem 486-DX100 Board auch mit 16550
Schnittstellen-Chips, auf einem aelteren 386-SX16 Board nur mit 
8250/16450 Schnittstellen-Chips.

Das Programm wurde auch mit einem WYSE-60 Terminal mit 
TELEVIDEO-Emulation getestet.

Die Start-Task heisst nun STRT_PING aus Kompatibilitaet zu 
WERUM-PEARL, Abbruch des Spiels mit TERM_PING.

Die Einbaufunktion CON,COFF wurden anstelle eines Aufrufs der
RTOS-Shell verwendet.

Das Programm wurde zum PEARL-Programmierwettbewerb des PEARL-Vereins
mit Einsendeschluss 31.01.88 eingesandt, womit der Autor (ich !) auf 
die Rechte an seinem Programm verzichtete. Nach der Aufloesung des
PEARL-Vereins wurden die eingesandten Beitraege von Professor
Frevert an den mich, den PEARL-Pool Verwalter, weitergegeben. 
