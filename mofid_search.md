# Searching Tips

## MOFid
Consider this scenario: you know you want to find MOF-5 (also known as IRMOF-1) in the QMOF Database but don't know which entry it corresponds to. One way to find the MOF that you're looking for is to take advantage of our tool called [MOFid](https://github.com/snurr-group/mofid). The MOFid code can generate a unique identifier for a given MOF structure, and this information is made publicly available with each structure in the QMOF Database. I outline the steps below:

1. Download the CIF of the desired MOF from the internet (e.g. from the original source publication). An example CIF for MOF-5 is [here](https://github.com/iRASPA/RASPA2/blob/master/structures/mofs/cif/IRMOF-1.cif).
2. Calculate its unique MOFid/MOFkey using the [ID Tool](https://snurr-group.github.io/web-mofid/) by simply uploading the structure and hitting submit.
3. Copy down the MOFid and/or MOFkey information. The MOFkey for MOF-5 is Zn.KKEYFWRCBNTPAC.MOFkey-v1.pcu.
4. Search the `qmof.json` file provided with the QMOF Database for any entries with the obtained MOFkey or MOFid components. The hits returned for MOF-5 are: LISBIZ_FSR, MIBQAR_FSR, SAHYIK_FSR, SAHYOQ_FSR , XOKHAH_FSR, and so on (this is a very popular MOF).
5. If there are multiple options, take the one you like. I would generally recommend the structure with the lowest energy (per atom), if there are any appreciable differences. 