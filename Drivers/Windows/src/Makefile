all:	../ACHILLES_DRV.exe ../ACHILLES_D64.exe

../ACHILLES_DRV.exe:	ACHILLES_DRV.7z
	cat 7zSD.sfx config.txt ACHILLES_DRV.7z > ../ACHILLES_DRV.exe

../ACHILLES_D64.exe:	ACHILLES_D64.7z
	cat 7zSD.sfx config.txt ACHILLES_D64.7z > ../ACHILLES_D64.exe

ACHILLES_DRV.7z:
	cd files && 7za a ../$@ *
	cd dpinst && 7za a ../$@ dpinst.exe

ACHILLES_D64.7z:
	cd files && 7za a ../$@ *
	cd dpinst64 && 7za a ../$@ dpinst.exe

clean:
	rm ACHILLES_DRV.7z ACHILLES_D64.7z
