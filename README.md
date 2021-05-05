# CrossPromo

## Functions:

**PlayVideo()**  - Play the current video in the loop

**Next()** - Set the current video to play to the next video in the loop

**Previous()** - Set the current video to play to the previous video in the loop

**Pause()** - If the video is playing, pause the video

**Resume()** - If the video is paused, continue the video

## Variables:

**playerID()** - The player id used for tracking the click on the video

**isLooping()** - Default set to true, if false only one video will appear in each time we activate the PlayVideo function

#

### Sample code to run a simple video one time:

```
  public class MyScript : MonoBehaviour
  {
    //The CrossPromo prefab
    public GameObject CrossPromo;

    private void Start()
    {
      CrossPromo.GetComponent<CrossPromoScript>().isLooping = false;
      CrossPromo.GetComponent<CrossPromoScript>().playerID = "myPlayerID";
      CrossPromo.GetComponent<CrossPromoScript>().PlayVideo();
    }
  }
```
