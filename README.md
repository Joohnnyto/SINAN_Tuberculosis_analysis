# SINAN_Tuberculosis_analysis

This dataset and codes are related to project: SOCIAL INEQUITIES OF TUBERCOLOSIS IN BRAZIL: A REAL WORLD ANAYSIS
We will use SQLite to conduct all dataset analysis. 

The main objectives are: 
- Demonstrate the difference between race, sex and brazilian regions in incidence, prevalence and mortality
- Explore the difference between diagnosis and initiantion of treatment
- Explore the distance between treatment site and patient residency

The analysis include SINAN database for tuberculosis = https://datasus.saude.gov.br/transferencia-de-arquivos/ -> database download in February 2024

Complete SINAN Database include the columns (98 columns originaly): 
TP_NOT
ID_AGRAVO
DT_NOTIFIC
NU_ANO
SG_UF_NOT
ID_MUNICIP
ID_REGIONA
DT_DIAG
ANO_NASC
NU_IDADE_N
CS_SEXO
CS_GESTANT
CS_RACA
CS_ESCOL_N
SG_UF
SG_UF_AJ -- created by study authors to enrich the UF data -> Import UF data when is emprty from SG_UF_NOT
ID_MN_RESI 
ID_MN_RESI_AJ -- created by study authors to enrich the city data -> Import city data when is emprty from ID_MUNICIP
ID_RG_RESI
ID_PAIS
NDUPLIC_N
IN_VINCULA
DT_DIGITA
DT_TRANSUS
DT_TRANSDM
DT_TRANSSM
DT_TRANSRM
DT_TRANSRS
DT_TRANSSE
CS_FLXRET
FLXRECEBI
MIGRADO_W
ID_OCUPA_N
TRATAMENTO
INSTITUCIO
RAIOX_TORA
TESTE_TUBE
FORMA
EXTRAPU1_N
EXTRAPU2_N
EXTRAPUL_O
AGRAVAIDS
AGRAVALCOO
AGRAVDIABE
AGRAVDOENC
AGRAVOUTRA
AGRAVOUTDE
BACILOSC_E
BACILOS_E2
BACILOSC_O
CULTURA_ES
CULTURA_OU
HIV
HISTOPATOL
DT_INIC_TR
RIFAMPICIN
ISONIAZIDA
ETAMBUTOL
ESTREPTOMI
PIRAZINAMI
ETIONAMIDA
OUTRAS
OUTRAS_DES
TRAT_SUPER
NU_CONTATO
DOENCA_TRA
SG_UF_AT
ID_MUNIC_A
DT_NOTI_AT
SG_UF_2
ID_MUNIC_2
BACILOSC_1
BACILOSC_2
BACILOSC_3
BACILOSC_4
BACILOSC_5
BACILOSC_6
TRATSUP_AT
DT_MUDANCA
NU_COMU_EX
SITUA_9_M
SITUA_12_M
SITUA_ENCE
DT_ENCERRA
TPUNINOT
POP_LIBER
POP_RUA
POP_SAUDE
POP_IMIG
BENEF_GOV
AGRAVDROGA
AGRAVTABAC
TEST_MOLEC
TEST_SENSI
ANT_RETRO
BAC_APOS_6
TRANSF
UF_TRANSF
MUN_TRANSF
CONCATENATE1 -- created by study authors to enrich unique patient identification -> concatenate DT_DIAG || ANO_NASC || NU_IDADE_N || CS_SEXO
CONCATENATE2 -- created by study authors to enrich unique patient identification -> concatenate DT_DIAG || ANO_NASC || CS_SEXO || ID_MN_RESI_AJ
DURATION_TT -- number of days between diagnosis and the end of treatment -> needs refinement 

**STUDY UNDER CONSTRUCTION**
