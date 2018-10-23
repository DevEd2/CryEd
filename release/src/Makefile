ROMNAME=CryEd

ASM=rgbasm
LNK=rgblink
FIX=rgbfix

ASMFLAGS=-o $(ROMNAME).obj -p 255 main.asm
LNKFLAGS=-p 255 -o $(ROMNAME).gb -n $(ROMNAME).sym $(ROMNAME).obj
FIXFLAGS=-v -p 255 $(ROMNAME).gb

make: Main.asm
	$(ASM) $(ASMFLAGS)
	$(LNK) $(LNKFLAGS)
	$(FIX) $(FIXFLAGS)