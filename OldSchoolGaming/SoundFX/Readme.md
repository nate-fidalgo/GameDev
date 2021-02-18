
<br>
Use OLDSCHOOLGAMINGSOUND.dll on your 64bit machine to emulate the old  8254 programable interval timer chip with onboard speaker that old computer gaming sound of
the 80 and 90's generations used. Remember them days where sound was 1bit but with PWM in the right way with the speaker not having time to fully go from on to off
one could achieve 8bit sound quality which was the threshold of being able to do ok sound for games :)
<br>
<bold> Please Note that this dll is only meant for 64 bit machines aka a 64 bit JVM some day i might upload a 32 bit dill version to work with 32bit JVMs. Please raise a issue comment if you would like the 32 bit dll version someday.</bold>
<br>
Below is sample code on how to uses this aka a sample test class using the native BEEP speaker method!
<pre>
<code>

public class SoundBeep {

	
    static {
        System.loadLibrary("OLDSCHOOLGAMINGSOUND");  //Load the OLDSCHOOLGAMINGSOUND.dll
    }

public static void main(String args[] )
{
System.out.println("Beeppping" ) ;
BEEP( 233 , 3221 ) ;
System.exit(0) ;

}

  //freq     ---> (The frequency of the sound, in hertz. This parameter must be in the range 37 through 32,767 (0x25 through 0x7FFF).)
  //duration ---> The duration of the sound, in milliseconds.
  public static native void BEEP( int freq , int duration ) ;
	
}

</code>
</pre>


<br>
<br>
To Run above example copy the code above with the OLDSCHOOLGAMINGSOUND.dll and make sure you have the path to the OLDSCHOOLGAMINGSOUND.dll set 
Like below enjoy :) and most importantly make some cool soundfx the old school way like old games did!!!
<pre>
<code>
javac SoundBeep.java
java -Djava.library.path="C:\xxxxx\xxxx\xxx\OLDSCHOOLGAMINGSOUND_DIRECTORY" SoundBeep

</pre>
</code>

<br>
O another use is to test your ears as a hearing test i can only get to 15khz ish the human hearing range i believe is 20hz to 20khz so i am lacking 15khz to 20khz range now.
See if you can here 16khz or even create a dog whistle like application.
I cool toy application. To create multiply frequencies mixed together like in the old school gaming consoles or computers you have to create multiple threads that each invoke 
SoundBeep.Beep(...) with different frequencies
<br>
definitely not sure on the ramification of this as new hardware is drastically different then old hardware so different machines may not beable to emulator or even use the BEEP function in which case for you guys this is all for nothing ignore all this talk.
