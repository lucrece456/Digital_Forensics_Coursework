
# Digital Forensics Coursework

## Module: Principles of Digital Forensics (7CSEF007W)
**University**: University of Westminster  
**Module Leader**: [Your Module Leader's Name]

### **Coursework Overview**
This repository contains all the files, documentation, and resources related to my Digital Forensics coursework. The assignment focuses on researching and analyzing modern partition tables (GPT) versus legacy methods (MBR). It includes practical implementations and comparisons to demonstrate proficiency in digital forensic analysis techniques.

---

### **Key Features**
1. **Partition Analysis**:
   - Creation and analysis of Master Boot Record (MBR) and GUID Partition Table (GPT).
   - Detailed comparisons of partition size, sector size, file system, and volume name.

2. **Hex Dump Analysis**:
   - Observations and screenshots of hex dump outputs for MBR and GPT partition types.
   - Endian representation analysis for both partitioning methods.

3. **Technical Comparisons**:
   - In-depth comparison of modern versus legacy partitioning methods.
   - Observations on partitioning schemes used in forensic investigations.

4. **Tools Used**:
   - `fdisk`, `parted`, and other Linux utilities for partition creation and analysis.
   - Hex editors for byte-level analysis.

---

### **Repository Structure**

Digital_Forensics_Coursework/
├── src/                     # Source files (commands, scripts, and code used in the coursework)
├── docs/                    # Documentation and reports
│   ├── Digital_Forensics_Report.pdf
│   ├── MBR_vs_GPT_Analysis.docx
│   └── References.bib       # Bibliography used in the coursework
├── assets/                  # Images and screenshots (e.g., hex dumps, partition tables)
├── README.md                # This file
└── LICENSE                  # Repository license (optional)

---

### **Commands and Instructions**
#### Partition Creation
- Create an MBR partition:
  ```bash
  sudo fdisk /dev/sdX

	•	Create a GPT partition:

sudo parted /dev/sdX mklabel gpt



Hex Dump Output

	•	Hex dump of an MBR partition:

xxd -g 1 /dev/sdX | head


	•	Hex dump of a GPT partition:

xxd -g 1 /dev/sdX | head

How to Use This Repository

	1.	Clone the repository:

git clone https://github.com/lucrece456/Digital_Forensics_Coursework.git


	2.	Explore the documentation in the docs/ directory for detailed reports.
	3.	Check out the src/ folder for command scripts and partition configurations.

Key Observations

	•	The structure and organization of partition tables impact forensic recovery and analysis.
	•	Hexadecimal analysis reveals critical differences in the representation of partition tables.
	•	Properly understanding MBR and GPT is essential for modern forensic investigations.

References

	1.	Digital Forensics Guide by NIST
	2.	Linux Partitioning and File Systems

Acknowledgments

This coursework was developed as part of my studies at the University of Westminster. Special thanks to the module leader for their guidance.

License

This project is licensed under the MIT License - see the LICENSE file for details.

Feel free to customize the details, such as the references or structure, based on your coursework specifics! Let me know if you need help further refining it.
