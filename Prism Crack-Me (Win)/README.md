# Reversing (+ patching) a Windows "Crack-Me" Style Program

## YOU NEED A WINDOWS MACHINE (physical or vm) IN ORDER TO COMPLETE THIS

- Start by downloading the 'PrismCrackMe.exe' in this folder

![loadingFile](loadingFile.JPG)

1. First drop your file into IDA PRO, and make sure that the filetype selected is 'Microsoft.Net assembly [pe64.l64]' and that the processor type is 'MetaPC', then press OK.

![selectProximityView](selectProximityView.JPG)

2. If available select 'Yes' to view with proximity view.

![clickHere](clickHere.JPG)

3. Now under 'Function name' in the top left double-click button1_Click

![andHere](andHere.JPG)

4. Double click on byte_2

![scrollDown](scrollDown.JPG)

5. Scroll down and bit and you should see 'ldstr "$f47da</"'. There it is, the password for the program. 