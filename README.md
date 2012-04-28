NORM Praat Script README
========================

Praat script for measuring vowel formants for NORM processing.

Instructions
------------

Before you use this script, you must edit the settings in the next section.

The script will not function at all if you do not specify a speaker.
Avoid using spaces in the name of the speaker, as that has not been tested.

If you would like the output file to be put somewhere other than the current
directory, specify that in the filepath, relative to this file.

### How To Use This Script ###

1. In Praat, load the script into "Log script 3" or "Log script 4" by
   entering the full path of the script into the menu accessed by executing
   [ Query > Log settings... ].

2. To measure monophthongs, put the cursor at the desired point or select an
   entire segment to get the mean measurements over that range.

3. To measure diphthongs, you will have to run the script twice. For the
   first run, select the initial steady-state position as if it were a
   monophthong. For the second run, select the glide position.

4. To run the script, execute [ Query > Log script 3 ] or [ Query > Log
   script 4 ], depending on what you did in Step 1.

5. In the first menu, specify the word you are measuring and a unique way to
   refer to the vowel you are measuring. (The same vowel should always have
   the same name.) You can use any system you want, as long as you are
   consistent. Click OK when you are done.

6. The next menu will ask whether you are measuring a monophthong or a
   diphthong. Give an honest answer.

7. On the second run of a diphthong measurement, the information you enter
   in the first menu is discarded, so you can leave it blank.

8. If you have measured the initial position of a diphthong, but not its
   glide position, Step 6 above will be different. Instead, it will ask you
   whether you want to measure that glide position or pretend that you had
   measured a monophthong and just move on to a new measurement. Again, be
   honest.

9. Once you have completed these steps once, a file will appear with the
   name of your speaker and the file extension '.tsv' (for tab-separated
   file). When you have completed your measurements, you can feed this file
   into NORM and have it plot all your vowels.

Settings
--------

* **`speaker$`:**  
  Add speaker name between quotation marks.

* **`filepath$`:**  
  Specify which directory to put the log files in.  
  Put path between quotation marks. (Do not include file name.)  
  Be sure to include trailing slash.  
  (Leave empty for current directory.)
