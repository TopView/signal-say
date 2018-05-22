![say](https://github.com/TopView/signal-say/blob/master/icon.png)

### This is a bash script to more easily use [signal-cli](https://github.com/AsamK/signal-cli) from the command line. 

Note: You can use this with signal-cli with ANY phone, including an older flip phone, or even a land line.

The file you care about is 'say' above.  It has further instructions inside it or when you run: `say --help`  (Note: `args` is a helper utility needed with the -V or --verbose option.)

***

**Requirements:**
   * GNU/Linux
   * [signal-cli](https://github.com/AsamK/signal-cli)
   * A terminal window
   * Any telephone

**Installation and usage:** `say --help`, (or read the well commented source code [here](https://github.com/TopView/signal-say/blob/master/say)).

**Important:** You must first *register* and *verity* your phone number (with a leading country code).  Refer to [signal-cli man page](https://github.com/AsamK/signal-cli/blob/master/man/signal-cli.1.adoc).  

1) Basically you need to first run this:

    signal-cli -u +1234567890 register [--voice]

where the number is your phone number.  Add the --voice option if you can't receive txt messages, e.g. your phone is a plain old land line.

2) And then run this to verify and finalize that registration:

    signal-cli verify <the 6 digit verification code you were texted or called back with>

Once verified you can use signal-say as described in the help (mentioned above).  

**Using signal-say is simple.**  You'll be using two commands: `say` and `?`.  `say` to send a message, and `?` to poll for any return receipts or replies.  (Just to make typing easier the default command is named `say` rather than `signal-say`, but you can rename it if you want to avoid any conflicts.)

**Program files**

    say             - THE MAIN PROGRAM HERE  
    args            - Helper utility used with -V / --verbose command line option to show effect of word splitting

**Misc. files**

    .editorconfig   - Sets github editing options (like tabs set to 4 wide)

    README.md       - This introduction  
    icon.png        - A little graphic for this introduction

    LICENSE         - Legal verbage
