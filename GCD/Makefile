
all: result.vcd

result.vcd: gcd.vhdl gcdTb.vhdl
	ghdl -a gcd.vhdl
	ghdl -a gcdTb.vhdl
	ghdl -e fsmgcd_tb
	ghdl -r fsmgcd_tb --vcd=result.vcd --stop-time=5us

clean:
	rm -rf result.vcd
