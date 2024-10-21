# **NGS Data Analysis Workshop: From FASTQ to Annotated VCF**

## **Workshop Overview**

This workshop introduces participants to the complete next-generation sequencing (NGS) data analysis pipeline, from quality control of raw sequencing data to variant calling and annotation. The focus will be on using web-based tools to simplify the workflow for beginners. By the end of the workshop, participants will be able to:
- Perform quality control on FASTQ files.
- Align sequencing reads to a reference genome.
- Call variants (SNPs and INDELs) using aligned reads.
- Annotate variants to predict their functional impact.
- Explore genomic variants using the IGV Web App.

### **Tools Used:**
- **Galaxy** (for FASTQ QC, alignment, and variant calling)
- **IGV Web App** (for visualization of aligned reads and variants)
- **VEP (Variant Effect Predictor)** (for variant annotation)

---

## **Workshop Contents**

### 1. **Quality Control of FASTQ Files Using Galaxy**
   - Tool: [Galaxy](https://usegalaxy.org/)
   - Task: Upload FASTQ files and perform quality control using FastQC.
   - Files Generated: 
     - FastQC Report (HTML): A visual summary of read quality.
   
### 2. **Alignment of Reads Using Galaxy**
   - Tool: [Galaxy](https://usegalaxy.org/)
   - Task: Align reads to the reference genome using BWA.
   - Files Generated:
     - SAM/BAM File: Aligned sequencing reads.

### 3. **Visualization of Aligned Reads Using IGV Web App**
   - Tool: [IGV Web App](https://igv.org/app/)
   - Task: Visualize BAM files and inspect sequencing alignments.
   - No new files are generated, but students can save session URLs for review.

### 4. **Variant Calling Using Galaxy**
   - Tool: [Galaxy](https://usegalaxy.org/)
   - Task: Call SNPs and INDELs using FreeBayes or GATK.
   - Files Generated:
     - VCF File: Contains identified variants.

### 5. **Variant Annotation Using VEP**
   - Tool: [VEP](https://www.ensembl.org/Tools/VEP)
   - Task: Annotate variants using the VCF file and predict their effects.
   - Files Generated:
     - Annotated VCF File: Contains functional annotations for each variant.

### 6. **In-depth Exploration of Variants Using IGV Web App**
   - Tool: [IGV Web App](https://igv.org/app/)
   - Task: Use IGV to visualize specific variants and their alignments.
   - Students will save session URLs for submission or review.

---

## **Setup Instructions**

### 1. **Tools Access**

You will need access to the following web-based tools:

- [Galaxy](https://usegalaxy.org/): For quality control, alignment, and variant calling.
- [IGV Web App](https://igv.org/app/): For visualizing sequencing data and variants.
- [VEP](https://www.ensembl.org/Tools/VEP): For variant annotation.

### 2. **Sample Data**

Download the following files for the workshop:
- **Sample FASTQ files:** `short_file.fastq` (https://github.com/czhang0701/KCLModule2_2024_NGS_workshop/blob/main/short_fastq_files.zip)

---

## **Detailed Steps**

### **1. Quality Control Using Galaxy**
1. Log into Galaxy [here](https://usegalaxy.org/).
2. Upload the FASTQ file (`short_file.fastq`).
3. Search for the **FastQC** tool and run it on both FASTQ files.
4. View the generated reports and check for any quality issues, such as low-quality bases or adapter contamination.

### **2. Read Alignment Using Galaxy**
1. In Galaxy, search for the **BWA-MEM** tool.
2. Input your FASTQ files and the reference genome.
3. Run the alignment and generate a BAM file.
4. Once the job completes, inspect the BAM file by viewing it in the Galaxy interface.

### **3. BAM File Visualization Using IGV Web**
1. Go to the [IGV Web App](https://igv.org/app/).
2. Upload the BAM file and the reference genome.
3. Explore the alignment, zoom in on specific regions, and inspect the coverage and read alignment patterns.

### **4. Variant Calling Using Galaxy**
1. In Galaxy, search for **FreeBayes** or **GATK HaplotypeCaller**.
2. Input the aligned BAM file and reference genome.
3. Run the variant calling process and generate a VCF file.

### **5. Variant Annotation Using VEP**
1. Go to [VEP](https://www.ensembl.org/Tools/VEP).
2. Upload the VCF file generated from the variant calling step.
3. Run the annotation process and download the annotated VCF file.

### **6. Explore Variants Using IGV**
1. Load both the BAM file and the annotated VCF file into the [IGV Web App](https://igv.org/app/).
2. Use IGV to visualize specific variants and explore their context in the read alignments.

---

## **Submission (for Workshop Participants)**

After completing the steps, save your session in IGV Web by following these instructions:
1. In the IGV Web App, save your session by selecting **File > Save Session**.
2. Copy the session URL and email it to **cheng.5.zhang@kcl.ac.uk** for review.

---

## **Additional Resources**

- **Galaxy Help:** [Galaxy Training Materials](https://training.galaxyproject.org/training-material/)
- **IGV Web App Tutorials:**
  - [Introduction to IGV Web](https://www.youtube.com/watch?v=sFeK-25K5PE&t=210s)
  - [Advanced IGV Web Features](https://www.youtube.com/watch?v=HwvTcG2SEOs)
- **VEP Documentation:** [VEP User Guide](https://www.ensembl.org/info/docs/tools/vep/index.html)

---

## **Contact**

For any questions or assistance during the workshop, feel free to reach out to **Cheng Zhang** at **cheng.5.zhang@kcl.ac.uk**.
