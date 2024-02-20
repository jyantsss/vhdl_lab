
all: result.vcd

result.vcd: gcd.vhdl gcdTB.vhdl
	ghdl -a gcd.vhdl
	ghdl -a gcdTB.vhdl
	ghdl -e fsmgcd_tb
	ghdl -r fsmgcd_tb --vcd=result.vcd --stop-time=5us

clean:
	rm -rf result.vcd
