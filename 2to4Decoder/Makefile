all:	result.vcd

result.vcd:	2to4Decoder.vhdl	2to4DecoderTest.vhdl
	ghdl	-a	-fsynopsys	2to4Decoder.vhdl
	ghdl	-a	-fsynopsys	2to4DecoderTest.vhdl
	ghdl	-e	-fsynopsys	bench
	ghdl	-r	-fsynopsys	bench	--vcd=result.vcd
clean:
	rm	-rf	result.vcd
