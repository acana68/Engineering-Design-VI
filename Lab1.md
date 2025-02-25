# Half Adder
```console
ghdl -a ha.vhdl
ghdl -a ha_tb.vhdl
ghdl -e ha_tb
ghdl -r ha_tb --vcd=ha.vcd
gtkwave ha.vcd
```
![ha gtkwave](https://drive.google.com/file/d/1-vFuhCmrOQsaHQrwuSbyPeApStaXz7da/view?usp=drive_link)

# Full Adder
```console
ghdl -a adder.vhdl
ghdl -a adder_tb.vhdl
ghdl -e adder_tb
ghdl -r adder_tb --vcd=adder.vcd
adder_tb.vhdl:54:5:@8ns(assertion note): end of test
gtkwave adder.vcd
```
![adder gktwave](https://drive.google.com/file/d/1ZYGQpb95am506X9qGBMir9gFQkwyVpTr/view?usp=drive_link)
