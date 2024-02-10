all: result.vcd

result.vcd: bcd7.vhdl bcd7Test.vhdl
	ghdl -a bcd7.vhdl
	ghdl -a bcd7Test.vhdl
	ghdl -e bcd7Test
	ghdl -r bcd7Test --vcd=result.vcd --stop-time=5us

clean:
	rm -rf result.vcd
