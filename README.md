# ~ scribe ~ Entware syslog-ng and logrotate installer for Asuswrt-Merlin

scribe is a syslog-ng and logrotate installer for ASUS routers running Asuswrt-Merlin

## Getting Started

### Prerequisites

1. Asuswrt-Merlin running on a supported ASUS router
2. Entware installed, preferably using [amtm](https://github.com/decoderman/amtm "amtm")
3. jffs scripts enabled in the firmware; installing Entware should have taken care of this part

* scribe includes handlers for the logs created by [skynet](https://github.com/Adamm00/IPSet_ASUS "skynet"); if you wish to use these handlers, it is advised to install skynet first.  If skynet is installed after scribe, you will have to re-run the installation and force installation.

### Installing

SSH into the router and run:
```bash
/usr/sbin/curl --retry 3 "https://raw.githubusercontent.com/cynicastic/scribe/master/scribe" -o "/jffs/scripts/scribe" && chmod 0755 /jffs/scripts/scribe && /jffs/scripts/scribe install
```

## WARNING

This software was written by someone who very likely didn't know what they were doing.  There is a non-zero chance this software will not fucntion as intended, cause irreparable data loss or hardware damage, or accidentally trigger the annihilation of the earth.  End user accepts all these potential outcomes as the unavoidable consequences of existing.

## ToDo:

- [ ] Expand the README
- [ ] Add a menu
- [ ] Add md5 checksum when checking for new versions
- [ ] Provide and ask to install a simplified syslog-ng.conf file
- [ ] ...
- [ ] ?????
- [ ] Profit!

## Built With

* [vim](https://www.vim.org/ "definitely NOT emacs") - because vi is always there, so I'm not lost on a clean install.

## Contributing

#### Code:
This has been a learning project for me, so I'm probably more married to my way of doing things than I should be.  Not to say suggestions aren't appreciated - they are and will be considered; but they are likely to be altered to my way of thinking about things if I add them, even if your way is clearly better.

#### Money:
Even if you think this is the best thing since sliced bread, please do not enquire about sending me money.  If I accepted money, I'll feel obligated to keep improving this, and I've got more than enough obligations in life at this point.  

## Authors

"Success has many fathers, but failure is a bastard child."

This isn't high school, it's all open book and copying from your neighbor is encouraged.  All the good bits I stole from someone else, all the crap bits and errors are mine.

## Acknowledgments

* RMerlin, for enduring an endless stream of people who will not read the release notes (out of his control), yet is still dedicated to producing the awesomeness that is AsusWRT-Merlin in what used to be known as his "free time".
* The great coders of SNB Forums, in alphabetical order, for lack of a better system:
    * Adamm
    * Jack Yaz
    * kvic
    * Odkrys
    * thelonelycoder
    * Xentrk

* Template used for thie README shamelessly stolen from [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2 "don't reinvent the wheel")

Are you really still reading this?  I'd have probably lost interest about halfway through.
