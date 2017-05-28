# Reversing (+ patching) a Windows "Crack-Me" Style Program

## YOU NEED A WINDOWS MACHINE (physical or vm) IN ORDER TO COMPLETE THIS

- Start by downloading the 'PrismCrackMe.exe' in this folder

![openProgram](openProgram.JPG)
1. First open the program, you can see we have a textBox for the password input, and a button that simply checks the contents of the textBox.

![loadingFile](loadingFile.JPG)

2. First drop your file into IDA PRO, and make sure that the filetype selected is 'Microsoft.Net assembly [pe64.l64]' and that the processor type is 'MetaPC', then press OK.

![selectProximityView](selectProximityView.JPG)

3. If available select 'Yes' to view with proximity view.

![clickHere](clickHere.JPG)

4. Now under 'Function name' in the top left double-click button1_Click

![andHere](andHere.JPG)

5. Double click on byte_2

![scrollDown](scrollDown.JPG)

6. Scroll down and bit and you should see 'ldstr "$f47da</"'. There it is, the password for the program. Copy the '$f47da</' string.

![complete](complete.JPG) ![failed](failed.JPG)

7. Now you can paste the password into the textBox and press check! If you got the success message congrats! If you didn't I don't know what to say.
