# Creating a Mask for Agisoft
Created by Jack A. Biggs
<br>*Maintained by [LEADR](http://leadr.msu.edu/) under the direction of Gillian Macdoanld*

*Last Updated: 4/9/2019*

This is a quick guide to creating masks to use in photogrammetry model building.

## Microsoft Paint Instructions
* Choose a photo for which to create the mask
    * To ensure the best quality of the mask, choose a photo out of the set where the majority of the object can be seen – preferably from the eye-level rotation
* Right click on the desired photo
    * On the dropdown menu choose **Open with --> Paint**
* Use eye dropper tool to select the color of the background
    * With this new color in the ‘Color 1’ box, select ‘Edit colors’
        * Click **Add to Custom Colors** then click **Okay**
    * Select ‘Color 2’ then click on the new color you created - this will ensure that both the border and fill of the mask will be this same color
    * Click on the ‘Select’ dropdown menu and choose **Select All --> Delete**
        * This should get rid of the image and replace it with the solid color you selected using the eye dropper tool
    * Saving the mask - **DO NOT HIT ‘CTRL S’ OR CLICK ON THE SAVE BUTTON!!**
        * Doing the above will basically replace the photo of the object with just a black photo which eliminates it from the set
          * This could mean that the model might not build properly since you don’t have that specific angled photo anymore
          * To save properly, click **File --> Save as**
               * Choose the location in which to save the mask - best not to save it into the Images folder, but to the overall folder
               * Rename the photo as the model designation followed by the word ‘mask’
                  * E.g. puma_effigy_mask.jpg

* Check to make sure that the mask is now in the desire location

## Photoshop Instructions
* Choose a photo for which to create the mask
   * To ensure the best quality of the mask, choose a photo out of the set where the majority of the object can be seen
        * Profile photos for skulls, whole-length photos of long bones, etc.
* Open Adobe Photoshop
   * Click **File --> Open -->** Choose the photo that you want to use
   * Once the photo has loaded, choose **Edit** on the taskbar and then **Fill** from the dropdown menu
   * A pop-up box should appear - make sure the following options are correct:
      * **Contents**
         * **Use: Black (or whichever color your background is)**
      * **Blending**
         * **Mode: Normal**
         * **Opacity: 100%**
      * Click **Okay**
   * The picture should automatically be completely filled in black
* Saving the mask - **DO NOT HIT ‘COMMAND S’ OR CLICK ON THE SAVE BUTTON!!**
   * Doing the above will basically replace the photo of the object with just a black photo which eliminates it from the set
      * This could mean that the model might not build properly since you don’t have that specific angled photo anymore
   * To save properly, click **File --> Save** as
      * Choose the location in which to save the mask - best not to save it into the **Images** folder, but to the overall folder
      * Rename the photo as the model designation followed by the word ‘mask’
         * E.g. puma_effigy_mask.jpg
* Check to make sure that the mask is now in the desire location

-----
### Return to [LEADR's Resources list](https://leadr-msu.github.io/)
