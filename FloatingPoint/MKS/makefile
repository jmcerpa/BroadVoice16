BV16DIR     = ../bv16
BVCOMMONDIR = ../bvcommon
OBJDIR      = obj

CC=cl
CFLAGS= -DWIN32 -DG192BITSTREAM=1 -I $(BV16DIR) -I $(BVCOMMONDIR) -O -c -W3 -Fo$@

OBJS = 	$(OBJDIR)/a2lsp.o \
	$(OBJDIR)/allpole.o \
	$(OBJDIR)/allzero.o \
	$(OBJDIR)/autocor.o \
	$(OBJDIR)/cmtables.o \
	$(OBJDIR)/levdur.o \
	$(OBJDIR)/lsp2a.o \
	$(OBJDIR)/ptdec.o \
	$(OBJDIR)/stblchck.o \
	$(OBJDIR)/stblzlsp.o \
	$(OBJDIR)/utility.o \
	$(OBJDIR)/bitpack.o \
	$(OBJDIR)/bv.o \
	$(OBJDIR)/coarptch.o \
	$(OBJDIR)/decoder.o \
	$(OBJDIR)/encoder.o \
	$(OBJDIR)/excdec.o \
	$(OBJDIR)/excquan.o \
	$(OBJDIR)/fineptch.o \
	$(OBJDIR)/g192.o \
	$(OBJDIR)/gaindec.o \
	$(OBJDIR)/gainquan.o \
	$(OBJDIR)/levelest.o \
	$(OBJDIR)/lspdec.o \
	$(OBJDIR)/lspquan.o \
	$(OBJDIR)/plc.o \
	$(OBJDIR)/postfilt.o \
	$(OBJDIR)/ptquan.o \
	$(OBJDIR)/tables.o \

BroadVoice16.exe: $(OBJS)
	link -out:../process/BroadVoice16.exe $(OBJS)

clean:
	rm -f ${OBJS}
	@echo "all .o files removed"

$(OBJDIR)/bitpack.o: $(BV16DIR)/bitpack.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16strct.h $(BV16DIR)/bv16.h
	$(CC) $(CFLAGS) $(BV16DIR)/bitpack.c

$(OBJDIR)/bv.o: $(BV16DIR)/bv.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16strct.h $(BV16DIR)/bv16.h $(BVCOMMONDIR)/utility.h $(BV16DIR)/g192.h $(BV16DIR)/bitpack.h
	$(CC) $(CFLAGS) $(BV16DIR)/bv.c

$(OBJDIR)/coarptch.o: $(BV16DIR)/coarptch.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/utility.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16externs.h
	$(CC) $(CFLAGS) $(BV16DIR)/coarptch.c

$(OBJDIR)/decoder.o: $(BV16DIR)/decoder.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16externs.h $(BV16DIR)/bv16strct.h $(BVCOMMONDIR)/utility.h $(BV16DIR)/postfilt.h
	$(CC) $(CFLAGS) $(BV16DIR)/decoder.c

$(OBJDIR)/encoder.o: $(BV16DIR)/encoder.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16externs.h $(BV16DIR)/bv16strct.h $(BVCOMMONDIR)/utility.h
	$(CC) $(CFLAGS) $(BV16DIR)/encoder.c

$(OBJDIR)/excdec.o: $(BV16DIR)/excdec.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h
	$(CC) $(CFLAGS) $(BV16DIR)/excdec.c

$(OBJDIR)/excquan.o: $(BV16DIR)/excquan.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h
	$(CC) $(CFLAGS) $(BV16DIR)/excquan.c

$(OBJDIR)/fineptch.o: $(BV16DIR)/fineptch.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h
	$(CC) $(CFLAGS) $(BV16DIR)/fineptch.c

$(OBJDIR)/g192.o: $(BV16DIR)/g192.c $(BVCOMMONDIR)/typedef.h  $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16cnst.h $(BV16DIR)/bv16strct.h
	$(CC) $(CFLAGS) $(BV16DIR)/g192.c

$(OBJDIR)/gaindec.o: $(BV16DIR)/gaindec.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16externs.h
	$(CC) $(CFLAGS) $(BV16DIR)/gaindec.c

$(OBJDIR)/gainquan.o: $(BV16DIR)/gainquan.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16externs.h
	$(CC) $(CFLAGS) $(BV16DIR)/gainquan.c

$(OBJDIR)/levelest.o: $(BV16DIR)/levelest.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h
	$(CC) $(CFLAGS) $(BV16DIR)/levelest.c

$(OBJDIR)/lspdec.o: $(BV16DIR)/lspdec.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16externs.h
	$(CC) $(CFLAGS) $(BV16DIR)/lspdec.c

$(OBJDIR)/lspquan.o: $(BV16DIR)/lspquan.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16externs.h
	$(CC) $(CFLAGS) $(BV16DIR)/lspquan.c

$(OBJDIR)/plc.o: $(BV16DIR)/plc.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BV16DIR)/bv16externs.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16strct.h $(BVCOMMONDIR)/utility.h $(BV16DIR)/postfilt.h
	$(CC) $(CFLAGS) $(BV16DIR)/plc.c

$(OBJDIR)/postfilt.o: $(BV16DIR)/postfilt.c $(BVCOMMONDIR)/typedef.h $(BVCOMMONDIR)/bvcommon.h $(BV16DIR)/bv16strct.h $(BV16DIR)/bv16cnst.h
	$(CC) $(CFLAGS) $(BV16DIR)/postfilt.c

$(OBJDIR)/ptquan.o: $(BV16DIR)/ptquan.c $(BVCOMMONDIR)/typedef.h $(BV16DIR)/bv16cnst.h $(BVCOMMONDIR)/bvcommon.h
	$(CC) $(CFLAGS) $(BV16DIR)/ptquan.c

$(OBJDIR)/tables.o: $(BV16DIR)/tables.c $(BVCOMMONDIR)/typedef.h
	$(CC) $(CFLAGS) $(BV16DIR)/tables.c

$(OBJDIR)/a2lsp.o: $(BVCOMMONDIR)/a2lsp.c $(BVCOMMONDIR)/typedef.h $(BVCOMMONDIR)/bvcommon.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/a2lsp.c

$(OBJDIR)/allpole.o: $(BVCOMMONDIR)/allpole.c $(BVCOMMONDIR)/typedef.h $(BVCOMMONDIR)/bvcommon.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/allpole.c

$(OBJDIR)/allzero.o: $(BVCOMMONDIR)/allzero.c $(BVCOMMONDIR)/typedef.h $(BVCOMMONDIR)/bvcommon.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/allzero.c

$(OBJDIR)/autocor.o: $(BVCOMMONDIR)/autocor.c $(BVCOMMONDIR)/typedef.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/autocor.c

$(OBJDIR)/cmtables.o: $(BVCOMMONDIR)/cmtables.c $(BVCOMMONDIR)/typedef.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/cmtables.c

$(OBJDIR)/levdur.o: $(BVCOMMONDIR)/levdur.c $(BVCOMMONDIR)/typedef.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/levdur.c

$(OBJDIR)/lsp2a.o: $(BVCOMMONDIR)/lsp2a.c $(BVCOMMONDIR)/typedef.h $(BVCOMMONDIR)/bvcommon.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/lsp2a.c

$(OBJDIR)/ptdec.o: $(BVCOMMONDIR)/ptdec.c $(BVCOMMONDIR)/typedef.h $(BVCOMMONDIR)/bvcommon.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/ptdec.c

$(OBJDIR)/stblchck.o: $(BVCOMMONDIR)/stblchck.c $(BVCOMMONDIR)/typedef.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/stblchck.c

$(OBJDIR)/stblzlsp.o: $(BVCOMMONDIR)/stblzlsp.c $(BVCOMMONDIR)/typedef.h $(BVCOMMONDIR)/bvcommon.h 
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/stblzlsp.c

$(OBJDIR)/utility.o: $(BVCOMMONDIR)/utility.c $(BVCOMMONDIR)/typedef.h
	$(CC) $(CFLAGS) $(BVCOMMONDIR)/utility.c
