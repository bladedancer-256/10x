# 10X Dumping Ground

Keep 10X notes, reports, results, (small) datasets etc. as you wish.
Basically instead of dumping everything in the
[Google doc](https://docs.google.com/document/d/1EhqPusGRCDKdK5tx5RpEhgwj_LCAi7plb2B62VvbaG4/edit),
feel free to dump it in here.

## Data Paths

| Description                            | Path                                                                             | Cluster   |
| ----------------------                 | -----------------------------------------------------------------------          | --------- |
| NA12878 WGS from [10X-wfu][wfu]        | `/data/cephfs/punim0010/data/External/Reference/NA12878-10x-2018/wfu`            | Spartan   |
| NA12878 WGS from [10X-wg1][wg1] re-run | `/data/cephfs/punim0010/data/External/Reference/NA12878-10x-2018/NA12878_WGS_v2` | Spartan   |
| NA12878 WGS from [10X-wfu][wfu] re-run | `/g/data3/gx8/projects/Hsu_10X_WGS/NA12878-10X-WFU`                              | Raijin    |
| NA12878 WES from [10X-wes][wes]        | `/data/cephfs/punim0010/data/External/Reference/NA12878-10x-2018/WES`            | Spartan   |
| LongRanger + References                | `/data/projects/punim0010/opt/`                                                  | Spartan   |
| GRCh37 non-decoy Reference             | `/data/cephfs/punim0010/extras/10x/refdata-GRCh37`                               | Spartan   |


[wfu]: https://support.10xgenomics.com/de-novo-assembly/datasets/2.0.0/wfu
[wg1]: https://support.10xgenomics.com/genome-exome/datasets/2.1.4/NA12878_WGS_v2
[wes]: https://support.10xgenomics.com/genome-exome/datasets/2.1.4/NA12878_WES_v2

## Tools

| Name               | Description                                                                          | Notes               |
| ------------------ | ------------------------------------------------------------------------------------ | ------------------- |
| [bxtools][bxt]     | light-weight tools for 10X data                                                      | has conda package   |
| [longranger][lr]   | 10X official pipeline for WGS/WES read alignment, SNP/Indel/SV calling and phasing   | has [docker](https://hub.docker.com/r/umccr/longranger/)                   |
| [HapCut2][hc2]     | haplotype assembly                                                                   | -                   |
| [EMA][ema]         | align 10X reads                                                                      | has conda package                   |
| [ZoomX][zoomx]     | somatic SV calling                                                                   | on bitbucket        |
| [bazam][bazam]     | extract paired reads in FASTQ format from coordinate sorted BAM files                | Simon Sadedin at 10X symposium |
| [gemtools][gemtools] | phase SVs in 10X reads                                                             | Hanlee Ji at 10X symposium |


[bxt]: https://github.com/walaj/bxtools
[lr]: https://support.10xgenomics.com/genome-exome/software/pipelines/latest/what-is-long-ranger
[hc2]: https://github.com/vibansal/HapCUT2
[ema]: https://github.com/arshajii/ema
[zoomx]: https://bitbucket.org/charade/zoomx
[bazam]: https://github.com/ssadedin/bazam
[gemtools]: https://github.com/sgreer77/gemtools
