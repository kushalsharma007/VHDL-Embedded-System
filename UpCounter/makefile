
all:	result.vcd
result.vcd:	counter.vhdl	counterTest.vhdl
	ghdl	-a	-fsynopsys	counter.vhdl
	ghdl	-a	-fsynopsys counterTest.vhdl
	ghdl	-e	-fsynopsys counterTest
	ghdl	-r	-fsynopsys counterTest	--vcd=result.vcd	--stop-time=2ms
clean:
	rm	-rf	result.vcd
