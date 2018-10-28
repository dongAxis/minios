all:
	nasm boot.asm -o boot.bin

boot:
	dd if=boot.bin of=../boot.img bs=512 count=1 conv=notrunc
	bochs -f bochsrc

clean:
	rm -rf *.bin
