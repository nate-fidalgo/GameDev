
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
        System.loadLibrary("OLDSCHOOLGAMINGSOUND");
    }

public static void main(String args[] )
{
System.out.println("Beeppping" ) ;
SoundBeep bp = new SoundBeep() ;
BEEP( 233 , 3221 ) ;
System.exit(0) ;

}

  public static native void BEEP( int freq , int duration ) ;
	
}

</code>
</pre>
