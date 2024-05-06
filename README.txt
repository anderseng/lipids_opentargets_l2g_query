
# These two files can be joined on study_id and lead_variant_id 

# Credible Set File Columns

tag_variant_id: Description not available.
postprob: Posterior probability of the tag variant being causal.
is95_credset: Indicator if the tag_variant_id is in the 95% credible set for the locus.
cred_set_min_pos: Minimum position of variants within the credible set for this locus.
cred_set_max_pos: Maximum position of variants within the credible set for this locus.
cred_set_size_bp: Size of the credible set in base pairs.
credset_n_variants: Number of variants within the credible set for this locus.
gene_id: Ensmbl gene ID
fpred_max_label: Most severe VEP consequence of the tag_variant_id on the gene_id
v2g_fpred_max_score: Score based on VEP functional prediction as described at https://github.com/opentargets/v2g_data/blob/master/configs/vep_consequences.tsv
v2g_qtl_score_q: Maximum quantile of OpenTargets V2G based on -log10(QTL p-value)
v2g_interval_score_q: Maximum quantile of OpenTargets V2G based on PCHi-C from Javierre et al. (Cell, 2016), Enhancer-TSS correlation from Andersson et al. (Nature, 2014) or DHS-promoter correlation from Thurman et al. (Nature,  2012)
v2g_distance_score_q: Maximum quantile of OpenTargets V2G based on 1/distance to tss
v2g: Weighted mean across the v2g quantiles, as described in https://genetics-docs.opentargets.org/our-approach/data-pipeline
distance_to_tss: distance to gene transcription start site (TSS) in bp

# Other File Columns

L2G: OpenTargets Locus-to-gene score associated with the locus and the gene.
coloc_h0: Colocalization hypothesis H0.
coloc_h1: Colocalization hypothesis H1.
coloc_h2: Colocalization hypothesis H2.
coloc_h3: Colocalization hypothesis H3.
coloc_h4: Colocalization hypothesis H4.
coloc_h4_h3: Ratio of colocalization hypotheses H4 to H3.
coloc_log2_h4_h3: Log2 ratio of colocalization hypotheses H4 to H3.
coloc_probe_transcript_id: Transcript ID of the probe used in colocalization study.
coloc_study: Colocalization study associated with the variant. Note that colocalization was only attempted if there were overlaps in the credible sets.
coloc_tissue: Tissue type used in colocalization study.
coloc_type: Type of colocalization study (eQTL or pQTL)
gene_name: Gene Name wtihin 500Kb of lead_variant
lead_variant_id: ID of the lead variant for each independent locus.
lead_variant_pval: P-value of the lead variant in the study.
n_cases: Number of cases in the study.
num_assoc_loci: Number of independent associated loci in the study.
pmid: PubMed ID of the study.
pub_date: Publication date of the study.
source: Source of the study data. Could be SAIGE (UKB) or GCST (GWAS Catalog)
study_id: ID of the study. There are 39 GWAS catalog studies of lipid traits from the last 10 years + 2 studies from UKB conducted with SAIGE
trait_efos: EFO Trait/Disase Codes. In this study, only lipid-related codes EFO_0003774, EFO_0004530, EFO_0004611, EFO_0004612, and HP_0003124 are included.
trait_reported: Reported trait for the GWAS (e.g. Hyperlipidemia)
