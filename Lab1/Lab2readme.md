# Half Adder
```console
ghdl -a ha.vhdl
ghdl -a ha_tb.vhdl
ghdl -e ha_tb
ghdl -r ha_tb --vcd=ha.vcd
gtkwave ha.vcd
```
![ha gtkwave](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab1/halfadderSS.PNG?raw=true)

# Full Adder
```console
ghdl -a adder.vhdl
ghdl -a adder_tb.vhdl
ghdl -e adder_tb
ghdl -r adder_tb --vcd=adder.vcd
adder_tb.vhdl:54:5:@8ns(assertion note): end of test
gtkwave adder.vcd
```
![adder gktwave](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab1/adderSS%20(1).PNG?raw=true)
