### This is a bash script to more easily use [signal-cli](https://github.com/AsamK/signal-cli) from the command line.

Note: You can use signal-say and signal-cli with ANY phone, including an older flip phone, or even a land line.

***

**Requirements:**
   * GNU/Linux
   * [signal-cli](https://github.com/AsamK/signal-cli)
   * A terminal window
   * Any telephone

**Installation and usage:** `say --help`, (or read the well commented source code [here](https://github.com/TopView/signal-say/blob/master/say)).

**Important:** You must first register and verity your phone number.  Refer to [signal-cli man page](https://github.com/AsamK/signal-cli/blob/master/man/signal-cli.1.adoc).  Basically you need to first run this:

    signal-cli -u +1234567890 register [--voice]

where the number is your phone number.  Add the --voice option if you can't receive txt messages, e.g. your phone is a plain old land line.

And then run this to verify and finalize that registration:

    signal-cli verify <the 6 digit verification code you were texted or called back with>

Once verified you can use signal-say as described in the help (mentioned above).  

**Using signal-say is simple.**  You'll be using two commands: `say` and `?`.  `say` to send a message, and `?` to poll for any return receipts or replies.  (Just to make typing easier the default command is named `say` rather than `signal-say`, but you can rename it if you want to avoid any conflicts.)
