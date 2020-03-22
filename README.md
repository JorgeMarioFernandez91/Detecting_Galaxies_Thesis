# Detecting_Galaxies_Thesis

This system is designed to read in images from the "images_folder" container simulated images with the keyword "sim" and their name and their respective real world counterparts (with just their name). Inverted black and white images should have the keyword "inv" in the name so the system knows how to handle these appropriately. These images can be either png or jpg. The test script looks in the test_image_folder for images.

examples:

simulated image:  m31_sim.jpg, m31_sim.png, etc.
  
real image:       m31.jpg, M31_NED.png, etc.

inverted images:  m31_inv.jpg, M31_NED_inv.png, etc.

When running for the first time you may be prompted to install missing Python libraries. I have not included how to do this but this should be fairly straight forward if you simply type the name of the library into google.
   
The system can be run with the following command:

    python3 -W ignore run.py system-test ./image_folder/
    
If you would like to keep track of the time it takes to run the run.py script pre-append the time command as follows:

    time python3 -W ignore run.py system-test ./image_folder/

The system can be tested with the following command: 
    
    python3 -W ignore test.py -v

Note: "-W ignore" can be ommitted if you wish to see warnings

If you would like to test yourself or another person to see how you compare with the system enter:

    time python3 -W ignore run.py human-test ./image_folder/
