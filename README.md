# GameDev
Game development repository
<br>
Use 
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
