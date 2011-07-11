                           _ 
                          | |
     _ __ ___   __ _ _   _| |
    | '_ ` _ \ / _` | | | | |
    | | | | | | (_| | |_| | |
    |_| |_| |_|\__,_|\__,_|_|
    
    a mail workalike that works with Apple Mail


## Introduction

Like using mail from the commandline? Don't want to set up sendmail on your
laptop? Maul is for you.

Maul attempts to be as similar as possible to the standard mail utility, but
uses the accounts you already have set up in the standard Apple Mail client.

## Installation

    curl -O https://raw.github.com/oldpatricka/maul/master/maul && mv maul /usr/local/bin/ && chmod +x /usr/local/bin/maul

## Usage

    $ maul user@example.com
    Subject: I'm using maul!
    Hey bud,

    I'm sending this mail from the command line. But I didn't set up sendmail
    or any of that noise.

    Rad, huh?

    .
    EOT
    $

You can also pipe stuff to maul:

    $ tail -n40 /var/log/app/everything.log | maul -s "Messed up log" user@example.com

## License

Copyright (c) 2011, Patrick Armstrong
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

Redistributions of source code must retain the above copyright notice, this
list of conditions and the following disclaimer.  Redistributions in binary
form must reproduce the above copyright notice, this list of conditions and the
following disclaimer in the documentation and/or other materials provided with
the distribution.  THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND
CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
OF SUCH DAMAGE.
