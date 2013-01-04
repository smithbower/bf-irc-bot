# IRC-BF

An IRC bot written in brainfuck.

## Usage

I've included a simple brainfuck interpreter that uses a TCP connection for input and output.

You can probably run this through a regular old brainfuck interpreter and do some crazy shit to wire it
up to a TCP connection, but I didn't feel like it. You can probably make something work with socat.

You can use the custom bf interpreter like this:

    netfuck hostname:port path/to/code.bf

For example, to connect the bot to freenode, use this:

    netfuck irc.freenode.net:6667 irc-bot.bf

Then, to get it into your favorite channel, use this from IRC:

    /msg bfbot join #channelname

## Included Programs

A couple of simple C# programs are included.

* bf.exe: A simple brainfuck interpreter.
* netfuck.exe: A brainfuck interpreter that uses TCP for input/output.
* asciitodec.exe: Converts an ASCII string to decimal to make my life easier

## Status

Current capabilities of the bot:

* Connect to IRC. Ignore all responses from the server. Time out and die.