# Docking-Molekul-dengan-Vina-Ver.1.2.5
Tutorial langkah-langkah Docking Molekul Menggunakan Vina Versi 1.2.5 (2023) menggunakan command Prompt di Windows 11


# Required software
1. Vina Versi 1.2.5 https://github.com/ccsb-scripps/AutoDock-Vina/releases atau bisa Pilih Versi Terbaru, di download dan di rename menjadi vina.exe
2. Vina dan Script Vina bisa di download di https://drive.google.com/drive/folders/1nWgguowPkIm4MjWj1DJNkgvvgSz8Hpel?usp=drive_link
3. Vegazz https://www.ddl.unimi.it/cms/index.php?Software_projects:VEGA_ZZ:Download
4. Mgl Tools (Version 1.5.7) https://ccsb.scripps.edu/download/262/
5. Discovery Studio (Version 2021) https://discover.3ds.com/discovery-studio-visualizer-download
6. Marvin Sketch https://chemaxon.com/marvin atau ChemDraw Ultra Versi 12
7. Notepad ++ https://notepad-plus-plus.org/downloads/

# Semua Software yang Dibutuhkan
bisa didownload di https://drive.google.com/drive/folders/1dKsa3nHUQzslO-emkJHd045z9aQAGS4b?usp=drive_link

# Pemisahan Protein dan Ligan (menggunakan Biovia Discovery Studio Visualizer)
1. Protein dapat di download dari situs https://www.rcsb.org/
2. Memisahkan Protein, hapus molekul air (Script > Selection > Select Water Molecules > Delete) dan Ligan (Script > Selection > Select Ligands > Delete) > Save Protein dalam Format .mol2
3. Memisahkan Native_Ligan, hapus molekul air (Script > Selection > Select Water Molecules > Delete) dan Protein (Script > Selection > Select Ligands > Edit > Invert Selection > Delete) > Save Ligan dalam Format .mol2

# Preparasi Protein Menggunakan Autodock Tools
1. Pisahkan Pertama Molekul Air dan native_ligands Biovia Discovery Studio Visualizer
2. Buka File pdb Protein protein.pdb
3. Tambahkan Hydrogen (Edit-Add Hydrogen-All)
4. Edit add gasteiger charge
5. Edit-Hydrogen Merge Non Polar
6. Grid-Macromolecules-Choose
7. Simpan dan beri nama protein.pdbqt > simpan

# Preparasi Native_Ligan Menggunakan Autodock Tools
Select File Read Molecules, look for ligand.pdb
Added Hydrogen with Edit-Add Hydrogen-All
Edit add gasteiger charge
Edit-Hydrogen Merge Non Polar
Ligand-Input-choose
Select ligand.pdb
ligand-Toorsion tree-detect root
Click Ligand-Torsion Tree-Choose Torsions, Select Done
Select Ligand-Torsion Tree-Set Number of Torsions select fewest atom, and Dismiss
Select Ligand-output-save as ligand.pdbqt

# Penentuan Sisi Aktif pada Protein Target
- membaca artikel protein di RCSB
- Online > Website Uniprot https://www.uniprot.org/
- Online server >  Aplikasi Online : ICM-PocketFinder, CASTp, Chimera, Qsite, Scfbio online server
- Offline Software Discovery Studio Visualizer

  

