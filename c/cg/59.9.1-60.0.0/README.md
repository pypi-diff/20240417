# Comparing `tmp/cg-59.9.1.tar.gz` & `tmp/cg-60.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg-59.9.1.tar", max compression
+gzip compressed data, was "cg-60.0.0.tar", max compression
```

## Comparing `cg-59.9.1.tar` & `cg-60.0.0.tar`

### file list

```diff
@@ -1,1296 +1,1329 @@
--rw-r--r--   0        0        0     2686 2024-03-04 07:52:11.681385 cg-59.9.1/README.md
--rw-r--r--   0        0        0       40 2024-03-04 07:52:11.685385 cg-59.9.1/cg/__init__.py
--rw-r--r--   0        0        0      315 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/__init__.py
--rw-r--r--   0        0        0       27 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/coverage/__init__.py
--rw-r--r--   0        0        0     2940 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/coverage/api.py
--rw-r--r--   0        0        0       56 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/__init__.py
--rw-r--r--   0        0        0    12783 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/crunchy.py
--rw-r--r--   0        0        0     4502 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/files.py
--rw-r--r--   0        0        0      430 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/models.py
--rw-r--r--   0        0        0      910 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/sbatch.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    12262 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0        0        0     8576 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/api.py
--rw-r--r--   0        0        0     1581 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0        0        0     4227 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0        0        0     7341 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
--rw-r--r--   0        0        0     4166 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0        0        0    10542 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_models.py
--rw-r--r--   0        0        0     9851 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0        0        0     1614 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
--rw-r--r--   0        0        0     9644 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
--rw-r--r--   0        0        0      824 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/validators.py
--rw-r--r--   0        0        0     1943 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/downsample/__init__.py
--rw-r--r--   0        0        0     6160 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/downsample/downsample.py
--rw-r--r--   0        0        0     2125 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/downsample/utils.py
--rw-r--r--   0        0        0      298 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/environ.py
--rw-r--r--   0        0        0     1741 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/gens.py
--rw-r--r--   0        0        0     3419 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/gt.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/hermes/__init__.py
--rw-r--r--   0        0        0     2249 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/hermes/hermes_api.py
--rw-r--r--   0        0        0     1298 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/hermes/models.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/housekeeper/__init__.py
--rw-r--r--   0        0        0    28681 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/housekeeper/hk.py
--rw-r--r--   0        0        0      326 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/housekeeper/models.py
--rw-r--r--   0        0        0       32 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/invoice/__init__.py
--rw-r--r--   0        0        0     4804 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/invoice/render.py
--rw-r--r--   0        0        0   113439 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0        0        0    81032 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0        0        0   113363 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0        0        0    80886 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
--rw-r--r--   0        0        0       25 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/__init__.py
--rw-r--r--   0        0        0    16539 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/api.py
--rw-r--r--   0        0        0     2652 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/batch.py
--rw-r--r--   0        0        0     8129 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/order.py
--rw-r--r--   0        0        0     3302 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/sample_sheet.py
--rw-r--r--   0        0        0     4866 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/loqus.py
--rw-r--r--   0        0        0       35 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/madeline/__init__.py
--rw-r--r--   0        0        0     3213 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/madeline/api.py
--rw-r--r--   0        0        0       23 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/mip/__init__.py
--rw-r--r--   0        0        0     3564 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/mip/confighandler.py
--rw-r--r--   0        0        0     2207 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/mutacc_auto.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/__init__.py
--rw-r--r--   0        0        0     9498 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0        0        0     3051 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0        0        0     6419 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0        0        0      252 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/utils.py
--rw-r--r--   0        0        0     2537 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/osticket.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/scout/__init__.py
--rw-r--r--   0        0        0     3177 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/scout/scout_export.py
--rw-r--r--   0        0        0    11054 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/scout/scoutapi.py
--rw-r--r--   0        0        0      444 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/scout/validators.py
--rw-r--r--   0        0        0       78 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     1854 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/api.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/models/__init__.py
--rw-r--r--   0        0        0     1871 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
--rw-r--r--   0        0        0     1076 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/__init__.py
--rw-r--r--   0        0        0     7312 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
--rw-r--r--   0        0        0     2641 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0        0        0     6806 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
--rw-r--r--   0        0        0     3559 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0        0        0      172 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/utils.py
--rw-r--r--   0        0        0      836 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/slurm/__init__.py
--rw-r--r--   0        0        0     1277 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/slurm/sbatch.py
--rw-r--r--   0        0        0     3559 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/slurm/slurm_api.py
--rw-r--r--   0        0        0       32 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/__init__.py
--rw-r--r--   0        0        0     7501 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/api.py
--rw-r--r--   0        0        0      152 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/dto/create_job_request.py
--rw-r--r--   0        0        0      287 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/dto/summary_response.py
--rw-r--r--   0        0        0     1305 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/models.py
--rw-r--r--   0        0        0      305 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/validators.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/__init__.py
--rw-r--r--   0        0        0    10945 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/add.py
--rw-r--r--   0        0        0     2653 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/archive.py
--rw-r--r--   0        0        0    10118 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/backup.py
--rw-r--r--   0        0        0     3853 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/base.py
--rw-r--r--   0        0        0    10506 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/clean.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/compress/__init__.py
--rw-r--r--   0        0        0     2135 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/compress/base.py
--rw-r--r--   0        0        0     6706 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/compress/fastq.py
--rw-r--r--   0        0        0     8163 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/compress/helpers.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/__init__.py
--rw-r--r--   0        0        0      564 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/base.py
--rw-r--r--   0        0        0     4603 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/case.py
--rw-r--r--   0        0        0     1884 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/cases.py
--rw-r--r--   0        0        0     2633 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/observations.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/deliver/__init__.py
--rw-r--r--   0        0        0     6270 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/deliver/base.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0      829 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/base.py
--rw-r--r--   0        0        0     4905 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
--rw-r--r--   0        0        0     8016 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/demux.py
--rw-r--r--   0        0        0     1619 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/finish.py
--rw-r--r--   0        0        0     2683 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0        0        0     2995 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/downsample.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/__init__.py
--rw-r--r--   0        0        0      356 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/base.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     4636 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/report/base.py
--rw-r--r--   0        0        0      854 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/report/options.py
--rw-r--r--   0        0        0     5107 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/report/utils.py
--rw-r--r--   0        0        0     8326 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/get.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/set/__init__.py
--rw-r--r--   0        0        0     9856 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/set/base.py
--rw-r--r--   0        0        0     4384 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/set/case.py
--rw-r--r--   0        0        0     2595 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/set/cases.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/store/__init__.py
--rw-r--r--   0        0        0     5340 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/store/fastq.py
--rw-r--r--   0        0        0     1049 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/store/store.py
--rw-r--r--   0        0        0     1761 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/transfer.py
--rw-r--r--   0        0        0        1 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/__init__.py
--rw-r--r--   0        0        0     5652 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/base.py
--rw-r--r--   0        0        0     5238 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0        0        0     1175 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/coverage.py
--rw-r--r--   0        0        0     1528 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/delivery_report.py
--rw-r--r--   0        0        0     4022 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/fohm.py
--rw-r--r--   0        0        0     1463 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/genotype.py
--rw-r--r--   0        0        0     1885 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/gens.py
--rw-r--r--   0        0        0      584 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/gisaid.py
--rw-r--r--   0        0        0     2645 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/mutacc.py
--rw-r--r--   0        0        0       23 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0        0        0     3006 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/nipt/base.py
--rw-r--r--   0        0        0     2275 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0        0        0     1596 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/nipt/statina.py
--rw-r--r--   0        0        0      112 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/observations/__init__.py
--rw-r--r--   0        0        0     2672 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/observations/observations.py
--rw-r--r--   0        0        0     2904 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/observations/utils.py
--rw-r--r--   0        0        0     9970 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/scout.py
--rw-r--r--   0        0        0      650 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/utils.py
--rw-r--r--   0        0        0     1667 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/validate.py
--rw-r--r--   0        0        0      105 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/utils.py
--rw-r--r--   0        0        0       18 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/__init__.py
--rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0        0        0     8925 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0        0        0     1980 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0        0        0      881 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0        0        0     1162 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0        0        0     1177 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0        0        0     1196 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/base.py
--rw-r--r--   0        0        0    12379 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/commands.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     1367 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fastq/base.py
--rw-r--r--   0        0        0     1787 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fastq/fastq_service.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     4177 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fluffy/base.py
--rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0     7810 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/microsalt/base.py
--rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0        0        0     6596 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip/base.py
--rw-r--r--   0        0        0     1268 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip/options.py
--rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0        0        0     1013 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip_dna/base.py
--rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0        0        0      916 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip_rna/base.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0        0        0     3413 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mutant/base.py
--rw-r--r--   0        0        0     3532 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/nf_analysis.py
--rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     1865 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/raredisease/base.py
--rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0        0        0    10391 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0        0        0      554 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/rnafusion/options.py
--rw-r--r--   0        0        0       22 2024-03-04 07:52:11.697385 cg-59.9.1/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0        0        0     6512 2024-03-04 07:52:11.697385 cg-59.9.1/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0        0        0      531 2024-03-04 07:52:11.697385 cg-59.9.1/cg/cli/workflow/taxprofiler/options.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/__init__.py
--rw-r--r--   0        0        0      147 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/arnold/api.py
--rw-r--r--   0        0        0      125 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/arnold/dto/create_case_request.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/__init__.py
--rw-r--r--   0        0        0     1078 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/api.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/dto/__init__.py
--rw-r--r--   0        0        0      503 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/dto/create_qc_metrics_request.py
--rw-r--r--   0        0        0      420 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/exceptions.py
--rw-r--r--   0        0        0      937 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/__init__.py
--rw-r--r--   0        0        0      253 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/archiving.py
--rw-r--r--   0        0        0       35 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/backup.py
--rw-r--r--   0        0        0     1411 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0        0        0      469 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/compression.py
--rw-r--r--   0        0        0     6285 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/constants.py
--rw-r--r--   0        0        0     5615 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/delivery.py
--rw-r--r--   0        0        0     9650 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/demultiplexing.py
--rw-r--r--   0        0        0     1422 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/encryption.py
--rw-r--r--   0        0        0      372 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/extraction.py
--rw-r--r--   0        0        0     2047 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/gene_panel.py
--rw-r--r--   0        0        0     6396 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/housekeeper_tags.py
--rw-r--r--   0        0        0       95 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/invoice.py
--rw-r--r--   0        0        0     5815 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/lims.py
--rw-r--r--   0        0        0      231 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/nanopore_files.py
--rw-r--r--   0        0        0      650 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/nextflow.py
--rw-r--r--   0        0        0      862 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/nf_analysis.py
--rw-r--r--   0        0        0       19 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/nipt.py
--rw-r--r--   0        0        0     2257 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/observations.py
--rw-r--r--   0        0        0     1216 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/orderforms.py
--rw-r--r--   0        0        0       96 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/paths.py
--rw-r--r--   0        0        0      266 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/pdc.py
--rw-r--r--   0        0        0      160 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/pedigree.py
--rw-r--r--   0        0        0     1044 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/priority.py
--rw-r--r--   0        0        0       79 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/process.py
--rw-r--r--   0        0        0     4506 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/report.py
--rw-r--r--   0        0        0      485 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/sample_sources.py
--rw-r--r--   0        0        0     3111 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/scout.py
--rw-r--r--   0        0        0     1669 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/sequencing.py
--rw-r--r--   0        0        0      313 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/slurm.py
--rw-r--r--   0        0        0      529 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/subject.py
--rw-r--r--   0        0        0       55 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/symbols.py
--rw-r--r--   0        0        0      435 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/tb.py
--rw-r--r--   0        0        0      161 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/time.py
--rw-r--r--   0        0        0     6014 2024-03-04 07:52:11.697385 cg-59.9.1/cg/exc.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/__init__.py
--rw-r--r--   0        0        0     1037 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/api.py
--rw-r--r--   0        0        0     2913 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/controller.py
--rw-r--r--   0        0        0     1763 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/csv.py
--rw-r--r--   0        0        0      210 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/gzip.py
--rw-r--r--   0        0        0      616 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/json.py
--rw-r--r--   0        0        0      601 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/txt.py
--rw-r--r--   0        0        0      552 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/validate_path.py
--rw-r--r--   0        0        0     1289 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/xml.py
--rw-r--r--   0        0        0     1153 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/yaml.py
--rw-r--r--   0        0        0      281 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/__init__.py
--rw-r--r--   0        0        0    15193 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/archive.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/__init__.py
--rw-r--r--   0        0        0     1727 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/constants.py
--rw-r--r--   0        0        0    10853 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/ddn_data_flow_client.py
--rw-r--r--   0        0        0     3704 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/models.py
--rw-r--r--   0        0        0     1250 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/utils.py
--rw-r--r--   0        0        0     2024 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/models.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/backup/__init__.py
--rw-r--r--   0        0        0    17530 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/backup/backup.py
--rw-r--r--   0        0        0     5397 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/backup/pdc.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/clean/__init__.py
--rw-r--r--   0        0        0     3901 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/clean/api.py
--rw-r--r--   0        0        0     7744 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/clean/clean_flow_cells.py
--rw-r--r--   0        0        0     1841 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/clean/clean_retrieved_spring_files.py
--rw-r--r--   0        0        0       34 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/compress/__init__.py
--rw-r--r--   0        0        0    14557 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/compress/compress.py
--rw-r--r--   0        0        0     4947 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/compress/files.py
--rw-r--r--   0        0        0    14247 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/deliver.py
--rw-r--r--   0        0        0     7886 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/deliver_ticket.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/__init__.py
--rw-r--r--   0        0        0     2592 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/combine_sequencing_metrics.py
--rw-r--r--   0        0        0     5915 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0        0        0     4135 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/files.py
--rw-r--r--   0        0        0     7777 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/housekeeper_storage_functions.py
--rw-r--r--   0        0        0     6941 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/status_db_storage_functions.py
--rw-r--r--   0        0        0    11951 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/utils.py
--rw-r--r--   0        0        0     2855 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/validation.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/encryption/__init__.py
--rw-r--r--   0        0        0    19578 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/encryption/encryption.py
--rw-r--r--   0        0        0      464 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/encryption/sbatch.py
--rw-r--r--   0        0        0    10922 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/invoice.py
--rw-r--r--   0        0        0     2249 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/meta.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/observations/__init__.py
--rw-r--r--   0        0        0     6008 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0        0        0     5277 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0        0        0     5364 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/observations/observations_api.py
--rw-r--r--   0        0        0       27 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/__init__.py
--rw-r--r--   0        0        0     3637 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/api.py
--rw-r--r--   0        0        0      121 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0        0        0      107 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0        0        0      122 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0        0        0    15262 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/case_submitter.py
--rw-r--r--   0        0        0     6102 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0        0        0      105 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0        0        0     1254 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/lims.py
--rw-r--r--   0        0        0     5782 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0        0        0     6337 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0        0        0      123 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0        0        0      105 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0        0        0      105 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0        0        0     7761 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/pool_submitter.py
--rw-r--r--   0        0        0      102 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/rml_submitter.py
--rw-r--r--   0        0        0      718 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0        0        0     1268 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0        0        0     1754 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/submitter.py
--rw-r--r--   0        0        0     7880 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/ticket_handler.py
--rw-r--r--   0        0        0     3608 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/qc_metrics/collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/__init__.py
--rw-r--r--   0        0        0    10372 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/balsamic.py
--rw-r--r--   0        0        0      562 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/balsamic_qc.py
--rw-r--r--   0        0        0      717 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/balsamic_umi.py
--rw-r--r--   0        0        0     4171 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/field_validators.py
--rw-r--r--   0        0        0     7160 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/mip_dna.py
--rw-r--r--   0        0        0    19056 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/report_api.py
--rw-r--r--   0        0        0     5403 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/rnafusion.py
--rw-r--r--   0        0        0    80176 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0        0        0   151463 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0        0        0    78094 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/templates/mip-dna_report.html
--rw-r--r--   0        0        0    79169 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/templates/rnafusion_report.html
--rw-r--r--   0        0        0       32 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/rsync/__init__.py
--rw-r--r--   0        0        0    12141 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/rsync/rsync_api.py
--rw-r--r--   0        0        0      387 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/rsync/sbatch.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/tar/__init__.py
--rw-r--r--   0        0        0     1694 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/tar/tar.py
--rw-r--r--   0        0        0       71 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/transfer/__init__.py
--rw-r--r--   0        0        0    10013 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/transfer/external_data.py
--rw-r--r--   0        0        0     5814 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/transfer/lims.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0        0        0     3107 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0        0        0     2224 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/coverage.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0        0        0    12102 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/fohm/fohm.py
--rw-r--r--   0        0        0       30 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0      928 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0        0        0    13521 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0        0        0     3312 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/gisaid/models.py
--rw-r--r--   0        0        0     5310 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/gt.py
--rw-r--r--   0        0        0      898 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/microsalt/microsalt_upload_api.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/mip/__init__.py
--rw-r--r--   0        0        0     2546 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0        0        0     1400 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0        0        0     7294 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/mutacc.py
--rw-r--r--   0        0        0       32 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0        0        0      696 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/nipt/models.py
--rw-r--r--   0        0        0     8106 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/nipt/nipt.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0        0        0     1698 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0     4009 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0        0        0     1491 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0        0        0     3322 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0        0        0     9103 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0        0        0     3495 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0        0        0     7516 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0        0        0    23146 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0        0        0     3197 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/upload_api.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/__init__.py
--rw-r--r--   0        0        0    26334 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/analysis.py
--rw-r--r--   0        0        0    26074 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/balsamic.py
--rw-r--r--   0        0        0     2700 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0        0        0      553 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0        0        0      556 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/downsample/__init__.py
--rw-r--r--   0        0        0     3922 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/downsample/downsample.py
--rw-r--r--   0        0        0      711 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/downsample/sbatch.py
--rw-r--r--   0        0        0     8913 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/fastq.py
--rw-r--r--   0        0        0    10687 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/fluffy.py
--rw-r--r--   0        0        0       70 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0      116 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/constants.py
--rw-r--r--   0        0        0      174 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/metrics_parser/__init__.py
--rw-r--r--   0        0        0      366 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
--rw-r--r--   0        0        0      903 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/metrics_parser/models.py
--rw-r--r--   0        0        0    13171 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/microsalt.py
--rw-r--r--   0        0        0       95 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/__init__.py
--rw-r--r--   0        0        0      712 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/models.py
--rw-r--r--   0        0        0     5688 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
--rw-r--r--   0        0        0     1217 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py
--rw-r--r--   0        0        0     2373 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py
--rw-r--r--   0        0        0     5641 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/utils.py
--rw-r--r--   0        0        0     1220 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/utils.py
--rw-r--r--   0        0        0    13833 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/mip.py
--rw-r--r--   0        0        0     2686 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/mip_dna.py
--rw-r--r--   0        0        0     2167 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/mip_rna.py
--rw-r--r--   0        0        0    10587 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/mutant.py
--rw-r--r--   0        0        0    19362 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/nf_analysis.py
--rw-r--r--   0        0        0     6161 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/nf_handlers.py
--rw-r--r--   0        0        0     6394 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0        0        0     2318 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/raredisease.py
--rw-r--r--   0        0        0     8987 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/rnafusion.py
--rw-r--r--   0        0        0     7652 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0        0        0      113 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/__init__.py
--rw-r--r--   0        0        0      102 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/analysis.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/balsamic/__init__.py
--rw-r--r--   0        0        0      459 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/balsamic/analysis.py
--rw-r--r--   0        0        0     4550 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/balsamic/config.py
--rw-r--r--   0        0        0     1954 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/balsamic/metrics.py
--rw-r--r--   0        0        0    16013 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/cg_config.py
--rw-r--r--   0        0        0     4302 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/compression_data.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/deliverables/__init__.py
--rw-r--r--   0        0        0     5170 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/deliverables/metric_deliverables.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/demultiplex/__init__.py
--rw-r--r--   0        0        0    12040 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0        0        0      539 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/demultiplex/sbatch.py
--rw-r--r--   0        0        0     6823 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/downsample/downsample_data.py
--rw-r--r--   0        0        0      255 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/email.py
--rw-r--r--   0        0        0     1046 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/fastq.py
--rw-r--r--   0        0        0     2157 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/file_data.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/flow_cell/__init__.py
--rw-r--r--   0        0        0    10976 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/flow_cell/flow_cell.py
--rw-r--r--   0        0        0      317 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/flow_cell/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/invoice/__init__.py
--rw-r--r--   0        0        0     1254 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/invoice/invoice.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/lims/__init__.py
--rw-r--r--   0        0        0     2019 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/lims/sample.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/__init__.py
--rw-r--r--   0        0        0      337 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/mip_analysis.py
--rw-r--r--   0        0        0     1564 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/mip_config.py
--rw-r--r--   0        0        0     4696 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0        0        0     2550 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/mip_sample_info.py
--rw-r--r--   0        0        0     2076 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/nf_analysis.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/observations/__init__.py
--rw-r--r--   0        0        0      688 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/observations/input_files.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/__init__.py
--rw-r--r--   0        0        0     2659 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/constants.py
--rw-r--r--   0        0        0     5604 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/excel_sample.py
--rw-r--r--   0        0        0      898 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/json_sample.py
--rw-r--r--   0        0        0     1449 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/order.py
--rw-r--r--   0        0        0      811 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/orderform_schema.py
--rw-r--r--   0        0        0     4212 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/sample_base.py
--rw-r--r--   0        0        0     9549 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/samples.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/validators/__init__.py
--rw-r--r--   0        0        0     2300 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/validators/excel_sample_validators.py
--rw-r--r--   0        0        0      576 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/validators/json_sample_validators.py
--rw-r--r--   0        0        0       71 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/validators/sample_base_validators.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/raredisease/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/__init__.py
--rw-r--r--   0        0        0     6785 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/metadata.py
--rw-r--r--   0        0        0     5951 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/report.py
--rw-r--r--   0        0        0     4724 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/sample.py
--rw-r--r--   0        0        0     2669 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/validators.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/rnafusion/__init__.py
--rw-r--r--   0        0        0     2633 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/scout/__init__.py
--rw-r--r--   0        0        0     4783 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/scout/scout_load_config.py
--rw-r--r--   0        0        0      116 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/scout/validators.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/slurm/__init__.py
--rw-r--r--   0        0        0      617 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/slurm/sbatch.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/taxprofiler/__init__.py
--rw-r--r--   0        0        0     2433 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/taxprofiler/taxprofiler.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/workflow/__init__.py
--rw-r--r--   0        0        0      685 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/workflow/mutant.py
--rw-r--r--   0        0        0       70 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/workflow/validators.py
--rw-r--r--   0        0        0    25590 2024-03-04 07:52:11.709385 cg-59.9.1/cg/resources/20181012_Indices.csv
--rw-r--r--   0        0        0      661 2024-03-04 07:52:11.709385 cg-59.9.1/cg/resources/__init__.py
--rw-r--r--   0        0        0     2590 2024-03-04 07:52:11.709385 cg-59.9.1/cg/resources/rnafusion_bundle_filenames.csv
--rw-r--r--   0        0        0     2583 2024-03-04 07:52:11.709385 cg-59.9.1/cg/resources/taxprofiler_bundle_filenames.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/__init__.py
--rw-r--r--   0        0        0    20077 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/admin.py
--rw-r--r--   0        0        0    19972 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/api.py
--rw-r--r--   0        0        0     4813 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/app.py
--rw-r--r--   0        0        0       48 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/auto.py
--rw-r--r--   0        0        0     1184 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/config.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/__init__.py
--rw-r--r--   0        0        0       92 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/delivery_message_response.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/orders/__init__.py
--rw-r--r--   0        0        0      598 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/orders/orders_request.py
--rw-r--r--   0        0        0      397 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/orders/orders_response.py
--rw-r--r--   0        0        0     2404 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/ext.py
--rw-r--r--   0        0        0       29 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/__init__.py
--rw-r--r--   0        0        0     4793 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0        0        0     8171 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0        0        0     2838 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0        0        0     4956 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0        0        0     7715 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/views.py
--rw-r--r--   0        0        0      354 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/templates/admin/index.html
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/__init__.py
--rw-r--r--   0        0        0      607 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/delivery_message_service.py
--rw-r--r--   0        0        0      792 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/__init__.py
--rw-r--r--   0        0        0      706 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/analysis_scout_message.py
--rw-r--r--   0        0        0      777 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/covid_message.py
--rw-r--r--   0        0        0      182 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/delivery_message.py
--rw-r--r--   0        0        0      721 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
--rw-r--r--   0        0        0      525 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/fastq_message.py
--rw-r--r--   0        0        0      701 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/fastq_scout_message.py
--rw-r--r--   0        0        0      594 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/microsalt_mwr_message.py
--rw-r--r--   0        0        0      582 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/microsalt_mwx_message.py
--rw-r--r--   0        0        0      415 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/scout_message.py
--rw-r--r--   0        0        0      408 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/statina_message.py
--rw-r--r--   0        0        0      737 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/utils.py
--rw-r--r--   0        0        0     2346 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/fastq_file_service/__init__.py
--rw-r--r--   0        0        0      101 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/fastq_file_service/exceptions.py
--rw-r--r--   0        0        0      868 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/fastq_file_service/fastq_file_service.py
--rw-r--r--   0        0        0     2780 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/fastq_file_service/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_service/__init__.py
--rw-r--r--   0        0        0      101 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_service/exceptions.py
--rw-r--r--   0        0        0     2020 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_service/order_service.py
--rw-r--r--   0        0        0     1053 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_service/utils.py
--rw-r--r--   0        0        0       92 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/dto/__init__.py
--rw-r--r--   0        0        0      275 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/dto/order_status_summary.py
--rw-r--r--   0        0        0      972 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/order_status_service.py
--rw-r--r--   0        0        0     2316 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_service/__init__.py
--rw-r--r--   0        0        0      703 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_service/slurm_cli_service.py
--rw-r--r--   0        0        0      242 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_service/slurm_service.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_upload_service/__init__.py
--rw-r--r--   0        0        0      175 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_upload_service/slurm_upload_config.py
--rw-r--r--   0        0        0     2074 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_upload_service/slurm_upload_service.py
--rw-r--r--   0        0        0      203 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_upload_service/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/__init__.py
--rw-r--r--   0        0        0     7245 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/base.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/__init__.py
--rw-r--r--   0        0        0    12932 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/create.py
--rw-r--r--   0        0        0     2144 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/delete.py
--rw-r--r--   0        0        0    77317 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/read.py
--rw-r--r--   0        0        0      837 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/update.py
--rw-r--r--   0        0        0     1662 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/database.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/__init__.py
--rw-r--r--   0        0        0     5371 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0        0        0     1712 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_application_filters.py
--rw-r--r--   0        0        0     1440 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_application_limitations_filters.py
--rw-r--r--   0        0        0     2523 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0        0        0     1390 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_bed_filters.py
--rw-r--r--   0        0        0     1317 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0        0        0    10384 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_case_filters.py
--rw-r--r--   0        0        0     1461 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0        0        0      903 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0        0        0     1412 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_customer_filters.py
--rw-r--r--   0        0        0     1880 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0        0        0     1255 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0        0        0     2792 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0        0        0     2304 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_order_filters.py
--rw-r--r--   0        0        0      851 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_organism_filters.py
--rw-r--r--   0        0        0      783 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_panel_filters.py
--rw-r--r--   0        0        0     3923 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_pool_filters.py
--rw-r--r--   0        0        0     8660 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_sample_filters.py
--rw-r--r--   0        0        0      731 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_user_filters.py
--rw-r--r--   0        0        0    37068 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/models.py
--rw-r--r--   0        0        0      593 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/store.py
--rw-r--r--   0        0        0       30 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/__init__.py
--rw-r--r--   0        0        0      187 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/calculations.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/checksum/__init__.py
--rw-r--r--   0        0        0     1579 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/checksum/checksum.py
--rw-r--r--   0        0        0     1655 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/click/EnumChoice.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/click/__init__.py
--rw-r--r--   0        0        0     4910 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/commands.py
--rw-r--r--   0        0        0     1811 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/date.py
--rw-r--r--   0        0        0      635 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/dict.py
--rw-r--r--   0        0        0     2111 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/dispatcher.py
--rw-r--r--   0        0        0     1251 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/email.py
--rw-r--r--   0        0        0      134 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/enums.py
--rw-r--r--   0        0        0     3178 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/files.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/flask/__init__.py
--rw-r--r--   0        0        0     1052 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/flask/enum.py
--rw-r--r--   0        0        0      834 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/time.py
--rw-r--r--   0        0        0     1224 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/utils.py
--rw-r--r--   0        0        0     1678 2024-03-04 07:52:11.717385 cg-59.9.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.717385 cg-59.9.1/tests/__init__.py
--rw-r--r--   0        0        0     1158 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/conftest.py
--rw-r--r--   0        0        0      231 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/coverage/conftest.py
--rw-r--r--   0        0        0     6188 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/coverage/test_coverage.py
--rw-r--r--   0        0        0     1693 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/conftest.py
--rw-r--r--   0        0        0     5438 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0        0        0     2283 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/test_config.py
--rw-r--r--   0        0        0    14032 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0        0        0     9109 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/test_spring_decompression.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    10776 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/conftest.py
--rw-r--r--   0        0        0     8944 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0        0        0     6098 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_index.py
--rw-r--r--   0        0        0     9468 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_override_cycles_validator.py
--rw-r--r--   0        0        0     6074 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0        0        0    15738 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_models.py
--rw-r--r--   0        0        0     4516 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0        0        0     2244 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_creator_factory.py
--rw-r--r--   0        0        0     3271 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_models.py
--rw-r--r--   0        0        0    11331 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_validator.py
--rw-r--r--   0        0        0     1495 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_validate.py
--rw-r--r--   0        0        0     5094 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/downsample/test_downsample.py
--rw-r--r--   0        0        0     1419 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/downsample/test_downsample_utils.py
--rw-r--r--   0        0        0     1716 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/gens/test_gens_api.py
--rw-r--r--   0        0        0     1950 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/gt/conftest.py
--rw-r--r--   0        0        0     4276 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/gt/test_gt_api.py
--rw-r--r--   0        0        0     1453 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/conftest.py
--rw-r--r--   0        0        0      684 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test__getattr__.py
--rw-r--r--   0        0        0     1593 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_add_file.py
--rw-r--r--   0        0        0     3523 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_bundles.py
--rw-r--r--   0        0        0      871 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_core.py
--rw-r--r--   0        0        0    24975 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_file.py
--rw-r--r--   0        0        0     5080 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_version.py
--rw-r--r--   0        0        0     1840 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/lims/conftest.py
--rw-r--r--   0        0        0     3197 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/lims/test_api.py
--rw-r--r--   0        0        0     1451 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/lims/test_sample_sheet.py
--rw-r--r--   0        0        0     9223 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/loqus/conftest.py
--rw-r--r--   0        0        0     8994 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/loqus/test_loqusdb_api.py
--rw-r--r--   0        0        0     2439 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/madeline/conftest.py
--rw-r--r--   0        0        0     4653 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/madeline/test_madeline.py
--rw-r--r--   0        0        0     3328 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/mip/conftest.py
--rw-r--r--   0        0        0     2487 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/mip/test_config_mip.py
--rw-r--r--   0        0        0      883 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0        0        0     2473 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/mutacc_auto/test_mutacc_auto.py
--rw-r--r--   0        0        0    11930 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/conftest.py
--rw-r--r--   0        0        0     9484 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0        0        0     4351 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0        0        0     1032 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0        0        0     2474 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/test_orderform_parser.py
--rw-r--r--   0        0        0    16002 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/validators/test_excel_sample_validators.py
--rw-r--r--   0        0        0     3670 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/conftest.py
--rw-r--r--   0        0        0     2269 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0        0        0     1376 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0        0        0     1840 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0        0        0     7047 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/test_scout_models.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     2861 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/conftest.py
--rw-r--r--   0        0        0     2010 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0        0        0     1820 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
--rw-r--r--   0        0        0     1908 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0        0        0     2997 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0        0        0     7322 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0        0        0     1458 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
--rw-r--r--   0        0        0     1131 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/slurm/conftest.py
--rw-r--r--   0        0        0     4412 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0        0        0      831 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/test_apps_environ.py
--rw-r--r--   0        0        0      957 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/test_osticket.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/__init__.py
--rw-r--r--   0        0        0     1174 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add.py
--rw-r--r--   0        0        0     2471 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0        0        0     6747 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0        0        0     7588 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0        0        0     7694 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add_sample.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/backup/__init__.py
--rw-r--r--   0        0        0      705 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/backup/conftest.py
--rw-r--r--   0        0        0    11101 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/backup/test_backup_command.py
--rw-r--r--   0        0        0     6865 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/conftest.py
--rw-r--r--   0        0        0     5536 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0        0        0     2557 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_clean_flow_cell.py
--rw-r--r--   0        0        0     1830 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0        0        0     2098 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0        0        0     4610 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0        0        0     3585 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0        0        0     1881 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_rsync_past_run_dirs.py
--rw-r--r--   0        0        0     9707 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/conftest.py
--rw-r--r--   0        0        0     7709 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0        0        0     1416 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0        0        0     5205 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0        0        0     1239 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0        0        0     7558 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/conftest.py
--rw-r--r--   0        0        0    12747 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0        0        0     1873 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/delete/test_cli_delete_cases.py
--rw-r--r--   0        0        0     3794 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/deliver/conftest.py
--rw-r--r--   0        0        0     4630 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0        0        0     1166 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0        0        0     8569 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/deliver/test_run_deliver_cmd.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0     9244 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     8683 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0        0        0     1607 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0        0        0     3704 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_validate_sample_sheet.py
--rw-r--r--   0        0        0     4423 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_verify_syncing.py
--rw-r--r--   0        0        0     1585 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/downsample/test_cli_downsample.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     1622 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/report/conftest.py
--rw-r--r--   0        0        0     2477 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0        0        0     2760 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/report/test_utils.py
--rw-r--r--   0        0        0      563 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/test_cli_base.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/__init__.py
--rw-r--r--   0        0        0      863 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get.py
--rw-r--r--   0        0        0     1526 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0        0        0     1242 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0        0        0     6208 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0        0        0     8835 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get_sample.py
--rw-r--r--   0        0        0     1364 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/conftest.py
--rw-r--r--   0        0        0     7311 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0        0        0     1460 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0        0        0     2016 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0        0        0     1685 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0        0        0    12450 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0        0        0     6124 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/set/test_cli_set_samples.py
--rw-r--r--   0        0        0     6934 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/store/test_fastq.py
--rw-r--r--   0        0        0     2332 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/test_base.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/__init__.py
--rw-r--r--   0        0        0    10003 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/conftest.py
--rw-r--r--   0        0        0     2295 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0        0        0     1789 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0        0        0      971 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0        0        0     1669 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0        0        0      895 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0        0        0     1199 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0        0        0      694 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0        0        0     9965 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0        0        0     4684 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0        0        0     1839 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0        0        0     6177 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/__init__.py
--rw-r--r--   0        0        0    30612 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0        0        0    13938 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0        0        0     7957 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0        0        0     2336 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0        0        0     3554 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0        0        0     6209 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0        0        0     6934 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0        0        0     8458 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/conftest.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     2298 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fastq/test_fastq_base.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     5291 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0        0        0     5687 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0        0        0     3302 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0        0        0     1896 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0        0        0     2968 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0        0        0     7815 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_store.py
--rw-r--r--   0        0        0     2775 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0     6926 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0        0        0     1000 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/microsalt/test_microsalt_run.py
--rw-r--r--   0        0        0     6544 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0        0        0     7011 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0        0        0     1542 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0        0        0      431 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0        0        0     2108 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
--rw-r--r--   0        0        0     1273 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0        0        0     3595 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0        0        0     3884 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0        0        0     1004 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0        0        0      527 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0        0        0      716 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0        0        0     8559 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_store.py
--rw-r--r--   0        0        0     1864 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py
--rw-r--r--   0        0        0     1927 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
--rw-r--r--   0        0        0     5075 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
--rw-r--r--   0        0        0     4498 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
--rw-r--r--   0        0        0     9843 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0        0        0     5887 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0        0        0     1602 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0        0        0     7899 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0        0        0     8710 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
--rw-r--r--   0        0        0     2409 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0        0        0     3302 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
--rw-r--r--   0        0        0     1521 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_metrics_deliver.py
--rw-r--r--   0        0        0     3933 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_run.py
--rw-r--r--   0        0        0      837 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0        0        0     4310 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0        0        0     2346 2024-03-04 07:52:11.725385 cg-59.9.1/tests/clients/conftest.py
--rw-r--r--   0        0        0     1812 2024-03-04 07:52:11.725385 cg-59.9.1/tests/clients/janus/test_janus_api_client.py
--rw-r--r--   0        0        0   100013 2024-03-04 07:52:11.725385 cg-59.9.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/fixture_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/__init__.py
--rw-r--r--   0        0        0     4867 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
--rw-r--r--   0        0        0     3686 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
--rw-r--r--   0        0        0    21233 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
--rw-r--r--   0        0        0     3699 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
--rw-r--r--   0        0        0     4385 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
--rw-r--r--   0        0        0     5824 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
--rw-r--r--   0        0        0     1304 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/timestamp_fixtures.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
--rw-r--r--   0        0        0    14644 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
--rw-r--r--   0        0        0    15921 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0        0        0     5497 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0        0        0    11711 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     2873 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/sample_coverage.bed
--rw-r--r--   0        0        0     6506 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json
--rw-r--r--   0        0        0    10513 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    10961 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0        0        0     3465 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0        0        0       63 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0        0        0      165 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0        0        0     2705 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
--rw-r--r--   0        0        0      692 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/crunchy/spring_metadata.json
--rw-r--r--   0        0        0      156 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/demuxcomplete.txt
--rw-r--r--   0        0        0     1781 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json
--rw-r--r--   0        0        0     2532 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json
--rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0        7 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     6034 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        7 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
--rw-r--r--   0        0        0        7 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      602 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/demuxcomplete.txt
--rw-r--r--   0        0        0      315 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      434 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0     8624 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0        0        0      568 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      220 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      463 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      622 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      619 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     4439 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0       43 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338370 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338349 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
--rw-r--r--   0        0        0     2126 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1827 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
--rw-r--r--   0        0        0       90 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
--rw-r--r--   0        0        0     6895 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
--rw-r--r--   0        0        0       37 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
--rw-r--r--   0        0        0    24755 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
--rw-r--r--   0        0        0      692 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0      724 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
--rw-r--r--   0        0        0     5775 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
--rw-r--r--   0        0        0     2282 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1632 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
--rw-r--r--   0        0        0       75 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
--rw-r--r--   0        0        0     6912 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
--rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
--rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
--rw-r--r--   0        0        0    24814 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
--rw-r--r--   0        0        0      814 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
--rw-r--r--   0        0        0      660 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
--rw-r--r--   0        0        0     5853 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    21848 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    15512 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       79 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      756 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     4118 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0     1408 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5326 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    15041 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    10649 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       80 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      755 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     2878 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0      928 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5359 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
--rw-r--r--   0        0        0    27887 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
--rw-r--r--   0        0        0   141870 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
--rwxr-xr-x   0        0        0   122682 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
--rw-r--r--   0        0        0      243 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0    28230 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
--rw-r--r--   0        0        0    94426 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
--rw-r--r--   0        0        0     5819 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
--rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     5945 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
--rw-r--r--   0        0        0      260 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
--rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0    47522 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
--rw-r--r--   0        0        0       12 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0        0        0     6666 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0        0        0      254 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
--rwxr-xr-x   0        0        0    47434 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
--rw-r--r--   0        0        0    10950 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
--rw-r--r--   0        0        0      225 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
--rw-r--r--   0        0        0       55 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2493 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
--rwxr-xr-x   0        0        0        1 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
--rwxr-xr-x   0        0        0        2 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
--rwxr-xr-x   0        0        0      730 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
--rwxr-xr-x   0        0        0    79277 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
--rwxr-xr-x   0        0        0     2694 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      619 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
--rw-r--r--   0        0        0     4941 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
--rwxr-xr-x   0        0        0    20050 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
--rw-r--r--   0        0        0      244 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6391 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
--rw-r--r--   0        0        0    16428 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
--rw-r--r--   0        0        0     6728 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0     5127 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
--rw-r--r--   0        0        0      124 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0      310 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0     5819 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0      122 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2694 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0      311 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6728 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
--rw-r--r--   0        0        0   111989 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0        0        0     5319 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
--rw-r--r--   0        0        0     5944 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2481 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2474 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
--rw-r--r--   0        0        0     5899 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
--rw-r--r--   0        0        0     4941 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
--rw-r--r--   0        0        0    10950 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0        0        0     5554 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0        0        0      901 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/summary.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/gt/yellowhog.bcf
--rw-r--r--   0        0        0     5114 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/madeline/madeline.xml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0        0        0     3241 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    21811 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0        0        0    23364 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    37367 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0       16 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0        0        0       16 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0       16 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0        0        0      123 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0        0        0    62741 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
--rw-r--r--   0        0        0    11242 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0        0        0    12164 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
--rw-r--r--   0        0        0     5231 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0        0        0     9774 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0        0        0     4624 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    13666 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/sample_file.txt
--rw-r--r--   0        0        0     1885 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0        0        0     6027 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0        0        0     9349 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0        0        0     1315 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0        0        0     3518 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0        0        0     8874 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0        0        0     4169 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/panel_export.csv
--rw-r--r--   0        0        0    63569 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0    42478 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0    69708 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      582 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
--rw-r--r--   0        0        0       42 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/shipping/scout-deploy.yaml
--rw-r--r--   0        0        0     1036 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0        0        0     1104 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0        0        0     1313 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0        0        0     3038 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0        0        0     3705 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0        0        0     1364 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0        0        0     2125 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0        0        0     1368 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0        0        0     4684 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/sarscov2.json
--rw-r--r--   0        0        0     5609 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0        0        0      511 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/bcl_convert_sample_sheet.csv
--rw-r--r--   0        0        0   258048 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/cgfixture.db
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0        0        0    49152 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/hkstore.db
--rw-r--r--   0        0        0       73 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/yellowhog/pedigree.yaml
--rw-r--r--   0        0        0       76 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/casava_five_parts.fastq.gz
--rw-r--r--   0        0        0       90 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/casava_seven_parts.fastq.gz
--rw-r--r--   0        0        0       96 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/casava_ten_parts.fastq.gz
--rw-r--r--   0        0        0      153 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/example.csv
--rw-r--r--   0        0        0       46 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/example.gz
--rw-r--r--   0        0        0      147 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/example.tsv
--rw-r--r--   0        0        0       20 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/io/example.txt
--rw-r--r--   0        0        0      582 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/io/example_json.json
--rw-r--r--   0        0        0      103 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/io/example_xml.xml
--rw-r--r--   0        0        0       20 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
--rw-r--r--   0        0        0       20 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
--rw-r--r--   0        0        0   156910 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx
--rw-r--r--   0        0        0   156770 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
--rw-r--r--   0        0        0   156737 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
--rw-r--r--   0        0        0   156582 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.fastq.xlsx
--rw-r--r--   0        0        0   155627 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx
--rw-r--r--   0        0        0   156850 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.mip.xlsx
--rw-r--r--   0        0        0   258580 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
--rw-r--r--   0        0        0   258342 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
--rw-r--r--   0        0        0    82677 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0        0        0   149394 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0        0        0   227887 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/2184.8.sarscov2.xlsx
--rw-r--r--   0        0        0    18639 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0        0        0     6052 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0        0        0     6611 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
--rw-r--r--   0        0        0     1417 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/report/case_data.json
--rw-r--r--   0        0        0     1109 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0        0        0     1562 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/report/lims_family.json
--rw-r--r--   0        0        0     2948 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/conftest.py
--rw-r--r--   0        0        0     8639 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_controller.py
--rw-r--r--   0        0        0     3877 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_csv.py
--rw-r--r--   0        0        0      482 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_gzip.py
--rw-r--r--   0        0        0     1779 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_json.py
--rw-r--r--   0        0        0     1828 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_txt.py
--rw-r--r--   0        0        0     1027 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_xml.py
--rw-r--r--   0        0        0     2131 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_yaml.py
--rw-r--r--   0        0        0     1233 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_validate_path.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/__init__.py
--rw-r--r--   0        0        0    13131 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/conftest.py
--rw-r--r--   0        0        0    16858 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/test_archive_api.py
--rw-r--r--   0        0        0    10246 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/test_archive_cli.py
--rw-r--r--   0        0        0    15766 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/test_archiving.py
--rw-r--r--   0        0        0     3807 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/backup/conftest.py
--rw-r--r--   0        0        0    26536 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0        0        0    10055 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/backup/test_meta_pdc.py
--rw-r--r--   0        0        0    12654 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/clean/conftest.py
--rw-r--r--   0        0        0    16961 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/clean/test_clean_flow_cells_api.py
--rw-r--r--   0        0        0     2286 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/clean/test_clean_retrieved_spring_files.py
--rw-r--r--   0        0        0     7691 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/conftest.py
--rw-r--r--   0        0        0     7961 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0        0        0     1778 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_compress_files.py
--rw-r--r--   0        0        0     3644 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0        0        0     1180 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0        0        0     6902 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0        0        0     8207 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/conftest.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/deliver/__init__.py
--rw-r--r--   0        0        0     3471 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/deliver/conftest.py
--rw-r--r--   0        0        0     8874 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0        0        0    10277 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/deliver/test_delivery_api.py
--rw-r--r--   0        0        0    13489 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/conftest.py
--rw-r--r--   0        0        0     5382 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py
--rw-r--r--   0        0        0    10786 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0        0        0    12330 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py
--rw-r--r--   0        0        0     5219 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_status_db_storage_functions.py
--rw-r--r--   0        0        0    22708 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0        0        0     6193 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_validation.py
--rw-r--r--   0        0        0     4943 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/encryption/conftest.py
--rw-r--r--   0        0        0    18133 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/encryption/test_encryption.py
--rw-r--r--   0        0        0     3122 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/observations/conftest.py
--rw-r--r--   0        0        0    16164 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/observations/test_meta_upload_observations.py
--rw-r--r--   0        0        0     4974 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/conftest.py
--rw-r--r--   0        0        0     1749 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0        0        0     1470 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0        0        0     1768 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0        0        0     2032 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0        0        0    19783 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0        0        0     7083 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0        0        0    29515 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0        0        0     1677 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0        0        0     1068 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_ticket_handler.py
--rw-r--r--   0        0        0     3907 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/qc_metrics/conftest.py
--rw-r--r--   0        0        0     1247 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/qc_metrics/test_collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/__init__.py
--rw-r--r--   0        0        0     5354 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/conftest.py
--rw-r--r--   0        0        0      434 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/helper.py
--rw-r--r--   0        0        0     4106 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0        0        0     4056 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_field_validators.py
--rw-r--r--   0        0        0     2834 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0        0        0    16698 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_report_api.py
--rw-r--r--   0        0        0     2546 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_rnafusion_api.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/rsync/__init__.py
--rw-r--r--   0        0        0      916 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/rsync/conftest.py
--rw-r--r--   0        0        0     9442 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/rsync/test_rsync.py
--rw-r--r--   0        0        0     3147 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/test_invoice.py
--rw-r--r--   0        0        0     1787 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/transfer/conftest.py
--rw-r--r--   0        0        0     9995 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/transfer/test_external_data.py
--rw-r--r--   0        0        0     4395 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/transfer/test_meta_transfer_lims.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/__init__.py
--rw-r--r--   0        0        0     2210 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0        0        0     4002 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/conftest.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0     2557 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0        0        0      211 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0        0        0      371 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0        0        0     3684 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0        0        0     4188 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
--rw-r--r--   0        0        0     1149 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0        0        0     1683 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/nipt/test_models.py
--rw-r--r--   0        0        0     1242 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/nipt/test_nipt_upload_api.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0    24071 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/conftest.py
--rw-r--r--   0        0        0     4734 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0        0        0     4182 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0        0        0    33260 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0        0        0     7372 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0        0        0     2511 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0        0        0     1473 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/test_upload_api.py
--rw-r--r--   0        0        0     2547 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/test_upload_genotypes_api.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/__init__.py
--rw-r--r--   0        0        0    10066 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/conftest.py
--rw-r--r--   0        0        0     3652 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0      318 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/test_parsing_metrics.py
--rw-r--r--   0        0        0     3714 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/test_quality_controller.py
--rw-r--r--   0        0        0    14367 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py
--rw-r--r--   0        0        0      825 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/test_report_generation.py
--rw-r--r--   0        0        0    20886 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_analysis.py
--rw-r--r--   0        0        0     6190 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0        0        0     3034 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_fastq.py
--rw-r--r--   0        0        0     1532 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0        0        0     3123 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_nf_analysis.py
--rw-r--r--   0        0        0     7741 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0        0        0     1688 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_rnafusion.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1161 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0        0        0     3500 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/crunchy.py
--rw-r--r--   0        0        0    21569 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/hk_mock.py
--rw-r--r--   0        0        0     3802 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/limsmock.py
--rw-r--r--   0        0        0      572 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/madeline.py
--rw-r--r--   0        0        0     1297 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0        0        0     1525 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/osticket.py
--rw-r--r--   0        0        0     3239 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/process_mock.py
--rw-r--r--   0        0        0     3718 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/report.py
--rw-r--r--   0        0        0     3915 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/scout.py
--rw-r--r--   0        0        0      750 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/store_model.py
--rw-r--r--   0        0        0     1532 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/tb_mock.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/balsamic/__init__.py
--rw-r--r--   0        0        0     1194 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/balsamic/conftest.py
--rw-r--r--   0        0        0     1030 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0        0        0     1050 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/conftest.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/demultiplexing/__init__.py
--rw-r--r--   0        0        0      284 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/demultiplexing/conftest.py
--rw-r--r--   0        0        0    11446 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/demultiplexing/test_run_parameters.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/downsample/__init__.py
--rw-r--r--   0        0        0     2096 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/downsample/test_down_sample_meta_data.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     8715 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/flow_cell/test_flowcell_model.py
--rw-r--r--   0        0        0     6637 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/conftest.py
--rw-r--r--   0        0        0     1239 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0        0        0     2348 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/test_mip_config.py
--rw-r--r--   0        0        0     6392 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0        0        0     3959 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/test_mip_sample_info.py
--rw-r--r--   0        0        0     3314 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/nextflow/test_nextflow_deliver.py
--rw-r--r--   0        0        0     1602 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/observations/conftest.py
--rw-r--r--   0        0        0     2579 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/observations/test_observations_input_files.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/report/__init__.py
--rw-r--r--   0        0        0     6722 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/report/test_validators.py
--rw-r--r--   0        0        0     3855 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0        0        0     1374 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/test_cg_models.py
--rw-r--r--   0        0        0      990 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/test_compression_data.py
--rw-r--r--   0        0        0      729 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/test_fastq.py
--rw-r--r--   0        0        0     2860 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/test_file_data.py
--rw-r--r--   0        0        0     3114 2024-03-04 07:52:11.761385 cg-59.9.1/tests/server/conftest.py
--rw-r--r--   0        0        0      509 2024-03-04 07:52:11.761385 cg-59.9.1/tests/server/endpoints/test_delivery_message_endpoint.py
--rw-r--r--   0        0        0     3047 2024-03-04 07:52:11.761385 cg-59.9.1/tests/server/endpoints/test_orders_endpoint.py
--rw-r--r--   0        0        0      271 2024-03-04 07:52:11.761385 cg-59.9.1/tests/server/test_server_auto.py
--rw-r--r--   0        0        0     1047 2024-03-04 07:52:11.761385 cg-59.9.1/tests/services/fastq_file_service/conftest.py
--rw-r--r--   0        0        0     3435 2024-03-04 07:52:11.761385 cg-59.9.1/tests/services/fastq_file_service/test_fastq_file_service.py
--rw-r--r--   0        0        0     1055 2024-03-04 07:52:11.761385 cg-59.9.1/tests/services/orders/order_status_service/conftest.py
--rw-r--r--   0        0        0      872 2024-03-04 07:52:11.761385 cg-59.9.1/tests/services/orders/order_status_service/test_order_status_service.py
--rw-r--r--   0        0        0      318 2024-03-04 07:52:11.761385 cg-59.9.1/tests/small_helpers.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/api/__init__.py
--rw-r--r--   0        0        0     2981 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/api/conftest.py
--rw-r--r--   0        0        0     1557 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/api/test_base.py
--rw-r--r--   0        0        0    20311 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/conftest.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/__init__.py
--rw-r--r--   0        0        0     1497 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/test_store_add_application_version.py
--rw-r--r--   0        0        0     3958 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/test_store_add_base.py
--rw-r--r--   0        0        0     2502 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/test_store_add_customer.py
--rw-r--r--   0        0        0     1640 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/test_store_add_flow_celll.py
--rw-r--r--   0        0        0    12209 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/conftest.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/delete/__init__.py
--rw-r--r--   0        0        0     5541 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/delete/test_delete.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/__init__.py
--rw-r--r--   0        0        0    57211 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read.py
--rw-r--r--   0        0        0     5461 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_analyses_to_clean.py
--rw-r--r--   0        0        0     3553 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py
--rw-r--r--   0        0        0    18463 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_analysis.py
--rw-r--r--   0        0        0     2743 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_application_version.py
--rw-r--r--   0        0        0    59704 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_case.py
--rw-r--r--   0        0        0     1105 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_customer.py
--rw-r--r--   0        0        0     1530 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_pool.py
--rw-r--r--   0        0        0    21602 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_sample.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/update/__init__.py
--rw-r--r--   0        0        0      737 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/update/test_update.py
--rw-r--r--   0        0        0    11693 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0        0        0     3397 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0        0        0     2073 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_application_limitations_filters.py
--rw-r--r--   0        0        0    10452 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0        0        0     2804 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0        0        0     2362 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0        0        0     3495 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0        0        0    39100 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0        0        0     1345 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0        0        0     2482 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0        0        0     4907 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0        0        0     2226 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0        0        0     5970 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0        0        0     2404 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0        0        0     1804 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0        0        0     8720 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0        0        0    22967 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0        0        0     1576 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0        0        0     2147 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/test_delivery.py
--rw-r--r--   0        0        0     4127 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/test_store_models.py
--rw-r--r--   0        0        0    35256 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store_helpers.py
--rw-r--r--   0        0        0     4930 2024-03-04 07:52:11.765385 cg-59.9.1/tests/test_copy_novaseqx_flow_cell.py
--rw-r--r--   0        0        0      911 2024-03-04 07:52:11.765385 cg-59.9.1/tests/test_store_helpers.py
--rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     1754 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/conftest.py
--rw-r--r--   0        0        0      371 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_calculations.py
--rw-r--r--   0        0        0     2920 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_commands.py
--rw-r--r--   0        0        0      953 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_date.py
--rw-r--r--   0        0        0     1508 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_dict.py
--rw-r--r--   0        0        0     7154 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_dispatcher.py
--rw-r--r--   0        0        0     4100 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_files.py
--rw-r--r--   0        0        0     1170 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_time.py
--rw-r--r--   0        0        0     2366 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_utils.py
--rw-r--r--   0        0        0     4341 1970-01-01 00:00:00.000000 cg-59.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2686 2024-04-16 14:26:30.528189 cg-60.0.0/README.md
+-rw-r--r--   0        0        0       40 2024-04-16 14:26:30.528189 cg-60.0.0/cg/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/coverage/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/coverage/api.py
+-rw-r--r--   0        0        0       56 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/crunchy/__init__.py
+-rw-r--r--   0        0        0    12783 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0        0        0     4502 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/crunchy/files.py
+-rw-r--r--   0        0        0      430 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/crunchy/models.py
+-rw-r--r--   0        0        0      910 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/crunchy/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    11321 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0        0        0    12920 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/api.py
+-rw-r--r--   0        0        0     3442 2024-04-16 14:26:30.528189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0        0        0     7341 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
+-rw-r--r--   0        0        0     4305 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0        0        0    10542 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/sample_models.py
+-rw-r--r--   0        0        0     6180 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0        0        0     1614 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
+-rw-r--r--   0        0        0     8346 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
+-rw-r--r--   0        0        0      824 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/demultiplex/sample_sheet/validators.py
+-rw-r--r--   0        0        0      677 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/downsample/__init__.py
+-rw-r--r--   0        0        0     6160 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/downsample/downsample.py
+-rw-r--r--   0        0        0     2125 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/downsample/utils.py
+-rw-r--r--   0        0        0      298 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/environ.py
+-rw-r--r--   0        0        0     1741 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/gens.py
+-rw-r--r--   0        0        0     3419 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/gt.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/hermes/__init__.py
+-rw-r--r--   0        0        0     2249 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0        0        0     1298 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/hermes/models.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0        0        0    30395 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/housekeeper/hk.py
+-rw-r--r--   0        0        0      326 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/housekeeper/models.py
+-rw-r--r--   0        0        0       32 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/invoice/__init__.py
+-rw-r--r--   0        0        0     4804 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/invoice/render.py
+-rw-r--r--   0        0        0   113439 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0        0        0    81032 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0        0        0   113363 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0        0        0    80886 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+-rw-r--r--   0        0        0       25 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/lims/__init__.py
+-rw-r--r--   0        0        0    16539 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/lims/api.py
+-rw-r--r--   0        0        0     2652 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/lims/batch.py
+-rw-r--r--   0        0        0     8129 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/lims/order.py
+-rw-r--r--   0        0        0     3332 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0        0        0     4866 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/loqus.py
+-rw-r--r--   0        0        0       35 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/madeline/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/madeline/api.py
+-rw-r--r--   0        0        0       23 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/mip/__init__.py
+-rw-r--r--   0        0        0     3564 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/mip/confighandler.py
+-rw-r--r--   0        0        0     2207 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/mutacc_auto.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/orderform/__init__.py
+-rw-r--r--   0        0        0     9498 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0        0        0     3051 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0        0        0     6419 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0        0        0      252 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/orderform/utils.py
+-rw-r--r--   0        0        0     2537 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/osticket.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/scout/__init__.py
+-rw-r--r--   0        0        0     3177 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/scout/scout_export.py
+-rw-r--r--   0        0        0    11054 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/scout/scoutapi.py
+-rw-r--r--   0        0        0      444 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/scout/validators.py
+-rw-r--r--   0        0        0       78 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     1854 2024-04-16 14:26:30.532189 cg-60.0.0/cg/apps/sequencing_metrics_parser/api.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/models/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
+-rw-r--r--   0        0        0     1076 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/__init__.py
+-rw-r--r--   0        0        0     7312 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
+-rw-r--r--   0        0        0     2641 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0        0        0     6806 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
+-rw-r--r--   0        0        0     3559 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0        0        0      172 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/utils.py
+-rw-r--r--   0        0        0      836 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/slurm/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/slurm/sbatch.py
+-rw-r--r--   0        0        0     3559 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/slurm/slurm_api.py
+-rw-r--r--   0        0        0       32 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/tb/__init__.py
+-rw-r--r--   0        0        0     7995 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/tb/api.py
+-rw-r--r--   0        0        0      152 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/tb/dto/create_job_request.py
+-rw-r--r--   0        0        0      250 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/tb/dto/summary_response.py
+-rw-r--r--   0        0        0     1305 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/tb/models.py
+-rw-r--r--   0        0        0      305 2024-04-16 14:26:30.536189 cg-60.0.0/cg/apps/tb/validators.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/__init__.py
+-rw-r--r--   0        0        0    11558 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/add.py
+-rw-r--r--   0        0        0     2653 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/archive.py
+-rw-r--r--   0        0        0    10118 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/backup.py
+-rw-r--r--   0        0        0     3852 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/base.py
+-rw-r--r--   0        0        0    10506 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/clean.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/compress/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/compress/base.py
+-rw-r--r--   0        0        0     6706 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/compress/fastq.py
+-rw-r--r--   0        0        0     8163 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/compress/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/delete/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/delete/base.py
+-rw-r--r--   0        0        0     4603 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/delete/case.py
+-rw-r--r--   0        0        0     1884 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/delete/cases.py
+-rw-r--r--   0        0        0     2633 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/delete/observations.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/deliver/__init__.py
+-rw-r--r--   0        0        0     6030 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/deliver/base.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/demultiplex/base.py
+-rw-r--r--   0        0        0     4905 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
+-rw-r--r--   0        0        0     7804 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/demultiplex/demux.py
+-rw-r--r--   0        0        0     1473 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/demultiplex/finish.py
+-rw-r--r--   0        0        0     3119 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0        0        0     2995 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/downsample.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/generate/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/generate/base.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/generate/report/base.py
+-rw-r--r--   0        0        0      854 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/generate/report/options.py
+-rw-r--r--   0        0        0     5107 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/generate/report/utils.py
+-rw-r--r--   0        0        0     8327 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/get.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/set/__init__.py
+-rw-r--r--   0        0        0     9856 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/set/base.py
+-rw-r--r--   0        0        0     4384 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/set/case.py
+-rw-r--r--   0        0        0     2595 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/set/cases.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/store/__init__.py
+-rw-r--r--   0        0        0     1093 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/store/base.py
+-rw-r--r--   0        0        0     6191 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/store/store.py
+-rw-r--r--   0        0        0     1761 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/transfer.py
+-rw-r--r--   0        0        0        1 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/__init__.py
+-rw-r--r--   0        0        0     5706 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/base.py
+-rw-r--r--   0        0        0     5503 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0        0        0     1175 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/coverage.py
+-rw-r--r--   0        0        0     1528 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/delivery_report.py
+-rw-r--r--   0        0        0     4022 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/fohm.py
+-rw-r--r--   0        0        0     1463 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/genotype.py
+-rw-r--r--   0        0        0     1885 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/gens.py
+-rw-r--r--   0        0        0      584 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/gisaid.py
+-rw-r--r--   0        0        0     2645 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/mutacc.py
+-rw-r--r--   0        0        0       23 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0        0        0     3006 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/nipt/base.py
+-rw-r--r--   0        0        0     2275 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0        0        0     1596 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/nipt/statina.py
+-rw-r--r--   0        0        0      112 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0        0        0     2672 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/observations/observations.py
+-rw-r--r--   0        0        0     2904 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/observations/utils.py
+-rw-r--r--   0        0        0     9970 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/scout.py
+-rw-r--r--   0        0        0      650 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/utils.py
+-rw-r--r--   0        0        0     1667 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/upload/validate.py
+-rw-r--r--   0        0        0      105 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/utils.py
+-rw-r--r--   0        0        0       18 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/workflow/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0        0        0     8925 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0        0        0     1980 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0        0        0      881 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0        0        0     1162 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0        0        0     1177 2024-04-16 14:26:30.536189 cg-60.0.0/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0        0        0     1269 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/base.py
+-rw-r--r--   0        0        0    12379 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/commands.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     1367 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/fastq/base.py
+-rw-r--r--   0        0        0     1787 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/fastq/fastq_service.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     4177 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/fluffy/base.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/microsalt/base.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/mip/base.py
+-rw-r--r--   0        0        0     1268 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/mip/options.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/mip_dna/base.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/mip_rna/base.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0        0        0     3413 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/mutant/base.py
+-rw-r--r--   0        0        0     9002 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/nf_analysis.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     2152 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/raredisease/base.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1179 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0        0        0     1111 2024-04-16 14:26:30.540189 cg-60.0.0/cg/cli/workflow/tomte/base.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.540189 cg-60.0.0/cg/clients/__init__.py
+-rw-r--r--   0        0        0     1363 2024-04-16 14:26:30.540189 cg-60.0.0/cg/clients/arnold/api.py
+-rw-r--r--   0        0        0      160 2024-04-16 14:26:30.540189 cg-60.0.0/cg/clients/arnold/dto/create_case_request.py
+-rw-r--r--   0        0        0      384 2024-04-16 14:26:30.540189 cg-60.0.0/cg/clients/arnold/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.540189 cg-60.0.0/cg/clients/janus/__init__.py
+-rw-r--r--   0        0        0     1246 2024-04-16 14:26:30.540189 cg-60.0.0/cg/clients/janus/api.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.540189 cg-60.0.0/cg/clients/janus/dto/__init__.py
+-rw-r--r--   0        0        0      503 2024-04-16 14:26:30.540189 cg-60.0.0/cg/clients/janus/dto/create_qc_metrics_request.py
+-rw-r--r--   0        0        0      420 2024-04-16 14:26:30.540189 cg-60.0.0/cg/clients/janus/exceptions.py
+-rw-r--r--   0        0        0      937 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/archiving.py
+-rw-r--r--   0        0        0       35 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/backup.py
+-rw-r--r--   0        0        0     1411 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0        0        0      469 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/compression.py
+-rw-r--r--   0        0        0     6545 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/constants.py
+-rw-r--r--   0        0        0     6033 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/delivery.py
+-rw-r--r--   0        0        0     8916 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/demultiplexing.py
+-rw-r--r--   0        0        0     1422 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/encryption.py
+-rw-r--r--   0        0        0      372 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/extraction.py
+-rw-r--r--   0        0        0     2054 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/gene_panel.py
+-rw-r--r--   0        0        0     6704 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/housekeeper_tags.py
+-rw-r--r--   0        0        0       95 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/invoice.py
+-rw-r--r--   0        0        0     5815 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/lims.py
+-rw-r--r--   0        0        0      231 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/nanopore_files.py
+-rw-r--r--   0        0        0      650 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/nextflow.py
+-rw-r--r--   0        0        0     1154 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/nf_analysis.py
+-rw-r--r--   0        0        0       19 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/nipt.py
+-rw-r--r--   0        0        0     2257 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/observations.py
+-rw-r--r--   0        0        0     1216 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/orderforms.py
+-rw-r--r--   0        0        0       96 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/paths.py
+-rw-r--r--   0        0        0      266 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/pdc.py
+-rw-r--r--   0        0        0      160 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/pedigree.py
+-rw-r--r--   0        0        0     1044 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/priority.py
+-rw-r--r--   0        0        0       79 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/process.py
+-rw-r--r--   0        0        0     4620 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/report.py
+-rw-r--r--   0        0        0      485 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/sample_sources.py
+-rw-r--r--   0        0        0     3111 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/scout.py
+-rw-r--r--   0        0        0     1669 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/sequencing.py
+-rw-r--r--   0        0        0      313 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/slurm.py
+-rw-r--r--   0        0        0      529 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/subject.py
+-rw-r--r--   0        0        0       55 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/symbols.py
+-rw-r--r--   0        0        0      435 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/tb.py
+-rw-r--r--   0        0        0      161 2024-04-16 14:26:30.540189 cg-60.0.0/cg/constants/time.py
+-rw-r--r--   0        0        0     6639 2024-04-16 14:26:30.540189 cg-60.0.0/cg/exc.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/api.py
+-rw-r--r--   0        0        0      621 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/config.py
+-rw-r--r--   0        0        0     2913 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/controller.py
+-rw-r--r--   0        0        0     1763 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/csv.py
+-rw-r--r--   0        0        0      210 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/gzip.py
+-rw-r--r--   0        0        0      662 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/json.py
+-rw-r--r--   0        0        0     1094 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/txt.py
+-rw-r--r--   0        0        0      552 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/validate_path.py
+-rw-r--r--   0        0        0     1289 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/xml.py
+-rw-r--r--   0        0        0     1153 2024-04-16 14:26:30.540189 cg-60.0.0/cg/io/yaml.py
+-rw-r--r--   0        0        0      281 2024-04-16 14:26:30.540189 cg-60.0.0/cg/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.540189 cg-60.0.0/cg/meta/archive/__init__.py
+-rw-r--r--   0        0        0    15193 2024-04-16 14:26:30.540189 cg-60.0.0/cg/meta/archive/archive.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.540189 cg-60.0.0/cg/meta/archive/ddn/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-16 14:26:30.540189 cg-60.0.0/cg/meta/archive/ddn/constants.py
+-rw-r--r--   0        0        0    10852 2024-04-16 14:26:30.540189 cg-60.0.0/cg/meta/archive/ddn/ddn_data_flow_client.py
+-rw-r--r--   0        0        0     3704 2024-04-16 14:26:30.540189 cg-60.0.0/cg/meta/archive/ddn/models.py
+-rw-r--r--   0        0        0     1250 2024-04-16 14:26:30.540189 cg-60.0.0/cg/meta/archive/ddn/utils.py
+-rw-r--r--   0        0        0     2024 2024-04-16 14:26:30.540189 cg-60.0.0/cg/meta/archive/models.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/backup/__init__.py
+-rw-r--r--   0        0        0    17426 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/backup/backup.py
+-rw-r--r--   0        0        0     5397 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/backup/pdc.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/clean/__init__.py
+-rw-r--r--   0        0        0     3901 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/clean/api.py
+-rw-r--r--   0        0        0     7738 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/clean/clean_flow_cells.py
+-rw-r--r--   0        0        0     1841 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/clean/clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0       34 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/compress/__init__.py
+-rw-r--r--   0        0        0    14557 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/compress/compress.py
+-rw-r--r--   0        0        0     4947 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/compress/files.py
+-rw-r--r--   0        0        0       77 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/deliver/__init__.py
+-rw-r--r--   0        0        0    14672 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/deliver/deliver.py
+-rw-r--r--   0        0        0     4502 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/deliver/deliver_ticket.py
+-rw-r--r--   0        0        0      904 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/deliver/fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/delivery/__init__.py
+-rw-r--r--   0        0        0     8150 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0        0        0     2592 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/demultiplex/combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     5915 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0        0        0     4135 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/demultiplex/files.py
+-rw-r--r--   0        0        0     7777 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/demultiplex/housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     6209 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/demultiplex/status_db_storage_functions.py
+-rw-r--r--   0        0        0    11951 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/demultiplex/utils.py
+-rw-r--r--   0        0        0     2855 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/demultiplex/validation.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/encryption/__init__.py
+-rw-r--r--   0        0        0    20271 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/encryption/encryption.py
+-rw-r--r--   0        0        0      537 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/encryption/sbatch.py
+-rw-r--r--   0        0        0    10922 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/invoice.py
+-rw-r--r--   0        0        0     2360 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/meta.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/observations/__init__.py
+-rw-r--r--   0        0        0     6008 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0        0        0     5277 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0        0        0     5364 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/observations/observations_api.py
+-rw-r--r--   0        0        0       27 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/__init__.py
+-rw-r--r--   0        0        0     3637 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/api.py
+-rw-r--r--   0        0        0      121 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0        0        0      107 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0        0        0      122 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0        0        0    15262 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/case_submitter.py
+-rw-r--r--   0        0        0     6102 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0        0        0     1254 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/lims.py
+-rw-r--r--   0        0        0     5782 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0        0        0     6337 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0        0        0      123 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0        0        0     7761 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0        0        0      102 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0        0        0      718 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0        0        0     1268 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0        0        0     1754 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/submitter.py
+-rw-r--r--   0        0        0     7880 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/orders/ticket_handler.py
+-rw-r--r--   0        0        0     4105 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/qc_metrics/collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/report/__init__.py
+-rw-r--r--   0        0        0    10310 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/report/balsamic.py
+-rw-r--r--   0        0        0      562 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/report/balsamic_qc.py
+-rw-r--r--   0        0        0      717 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0        0        0     4171 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/report/field_validators.py
+-rw-r--r--   0        0        0     7100 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/report/mip_dna.py
+-rw-r--r--   0        0        0    20025 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/report/report_api.py
+-rw-r--r--   0        0        0     6299 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/report/rnafusion.py
+-rw-r--r--   0        0        0    82540 2024-04-16 14:26:30.544189 cg-60.0.0/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0        0        0   151463 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0        0        0    80462 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/report/templates/mip-dna_report.html
+-rw-r--r--   0        0        0    81533 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/report/templates/rnafusion_report.html
+-rw-r--r--   0        0        0       32 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/rsync/__init__.py
+-rw-r--r--   0        0        0    12291 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0        0        0      387 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/rsync/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/tar/__init__.py
+-rw-r--r--   0        0        0     1694 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/tar/tar.py
+-rw-r--r--   0        0        0       71 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/transfer/__init__.py
+-rw-r--r--   0        0        0    10013 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/transfer/external_data.py
+-rw-r--r--   0        0        0     5814 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/transfer/lims.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0        0        0     3107 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0        0        0     2224 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/coverage.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0        0        0    12102 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/fohm/fohm.py
+-rw-r--r--   0        0        0       30 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0      928 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0        0        0    13521 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0        0        0     3312 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0        0        0     5310 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/gt.py
+-rw-r--r--   0        0        0      898 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/microsalt/microsalt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0        0        0     2546 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0        0        0     1400 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0        0        0     7294 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/mutacc.py
+-rw-r--r--   0        0        0     1853 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/nf_analysis.py
+-rw-r--r--   0        0        0       32 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/nipt/models.py
+-rw-r--r--   0        0        0     8106 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/nipt/nipt.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0        0        0     1491 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0        0        0     3322 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0        0        0     9103 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0        0        0     3495 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0        0        0     7516 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0        0        0    23146 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0        0        0     3197 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/upload/upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    27148 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/analysis.py
+-rw-r--r--   0        0        0    25955 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/balsamic.py
+-rw-r--r--   0        0        0     2700 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0        0        0      553 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0        0        0      556 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/downsample/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/downsample/downsample.py
+-rw-r--r--   0        0        0      711 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/downsample/sbatch.py
+-rw-r--r--   0        0        0     8913 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/fastq.py
+-rw-r--r--   0        0        0    10687 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/fluffy.py
+-rw-r--r--   0        0        0       70 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/constants.py
+-rw-r--r--   0        0        0      174 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/metrics_parser/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
+-rw-r--r--   0        0        0      903 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/metrics_parser/models.py
+-rw-r--r--   0        0        0    13171 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/microsalt.py
+-rw-r--r--   0        0        0       95 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/models.py
+-rw-r--r--   0        0        0     5688 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
+-rw-r--r--   0        0        0     1217 2024-04-16 14:26:30.548189 cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/report_generator.py
+-rw-r--r--   0        0        0     2373 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/result_logger.py
+-rw-r--r--   0        0        0     5641 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/utils.py
+-rw-r--r--   0        0        0     1220 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/microsalt/utils.py
+-rw-r--r--   0        0        0    13833 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/mip.py
+-rw-r--r--   0        0        0     2686 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0        0        0     2167 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0        0        0    10587 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/mutant.py
+-rw-r--r--   0        0        0    34384 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/nf_analysis.py
+-rw-r--r--   0        0        0     6161 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/nf_handlers.py
+-rw-r--r--   0        0        0     6394 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0        0        0     5831 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/raredisease.py
+-rw-r--r--   0        0        0     6023 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0        0        0     4607 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0        0        0     3204 2024-04-16 14:26:30.552189 cg-60.0.0/cg/meta/workflow/tomte.py
+-rw-r--r--   0        0        0      113 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/__init__.py
+-rw-r--r--   0        0        0      102 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/analysis.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/balsamic/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/balsamic/analysis.py
+-rw-r--r--   0        0        0     4550 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/balsamic/config.py
+-rw-r--r--   0        0        0     1954 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/balsamic/metrics.py
+-rw-r--r--   0        0        0    17539 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/cg_config.py
+-rw-r--r--   0        0        0     4302 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/compression_data.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/deliverables/__init__.py
+-rw-r--r--   0        0        0     5170 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/deliverables/metric_deliverables.py
+-rw-r--r--   0        0        0      243 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/demultiplex/__init__.py
+-rw-r--r--   0        0        0    12040 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0        0        0      539 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0        0        0     7006 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/downsample/downsample_data.py
+-rw-r--r--   0        0        0      255 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/email.py
+-rw-r--r--   0        0        0     1046 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/fastq.py
+-rw-r--r--   0        0        0     2157 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/file_data.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0    10942 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/flow_cell/flow_cell.py
+-rw-r--r--   0        0        0      317 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/flow_cell/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/invoice/__init__.py
+-rw-r--r--   0        0        0     1254 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/invoice/invoice.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/lims/__init__.py
+-rw-r--r--   0        0        0     2019 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/lims/sample.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/mip/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/mip/mip_analysis.py
+-rw-r--r--   0        0        0     1564 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/mip/mip_config.py
+-rw-r--r--   0        0        0     4696 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     2550 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/mip/mip_sample_info.py
+-rw-r--r--   0        0        0     2472 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/nf_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/observations/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/observations/input_files.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/__init__.py
+-rw-r--r--   0        0        0     2659 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/constants.py
+-rw-r--r--   0        0        0     5604 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/excel_sample.py
+-rw-r--r--   0        0        0      898 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/json_sample.py
+-rw-r--r--   0        0        0     1449 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/order.py
+-rw-r--r--   0        0        0      811 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/orderform_schema.py
+-rw-r--r--   0        0        0     4212 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/sample_base.py
+-rw-r--r--   0        0        0     9668 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/samples.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/validators/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/validators/excel_sample_validators.py
+-rw-r--r--   0        0        0      576 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/validators/json_sample_validators.py
+-rw-r--r--   0        0        0       71 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/orders/validators/sample_base_validators.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/raredisease/__init__.py
+-rw-r--r--   0        0        0     1549 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/raredisease/raredisease.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/report/__init__.py
+-rw-r--r--   0        0        0     6785 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/report/metadata.py
+-rw-r--r--   0        0        0     6180 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/report/report.py
+-rw-r--r--   0        0        0     5156 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/report/sample.py
+-rw-r--r--   0        0        0     3004 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/report/validators.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/rnafusion/__init__.py
+-rw-r--r--   0        0        0     2188 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/rnafusion/rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/scout/__init__.py
+-rw-r--r--   0        0        0     4783 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/scout/scout_load_config.py
+-rw-r--r--   0        0        0      116 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/slurm/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/slurm/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/taxprofiler/taxprofiler.py
+-rw-r--r--   0        0        0     1203 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/tomte/tomte.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/workflow/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/workflow/mutant.py
+-rw-r--r--   0        0        0       70 2024-04-16 14:26:30.552189 cg-60.0.0/cg/models/workflow/validators.py
+-rw-r--r--   0        0        0      842 2024-04-16 14:26:30.552189 cg-60.0.0/cg/resources/__init__.py
+-rw-r--r--   0        0        0     3493 2024-04-16 14:26:30.552189 cg-60.0.0/cg/resources/rnafusion_bundle_filenames.yaml
+-rw-r--r--   0        0        0     2434 2024-04-16 14:26:30.556189 cg-60.0.0/cg/resources/taxprofiler_bundle_filenames.yaml
+-rw-r--r--   0        0        0     3732 2024-04-16 14:26:30.556189 cg-60.0.0/cg/resources/tomte_bundle_filenames.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/__init__.py
+-rw-r--r--   0        0        0    20241 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/admin.py
+-rw-r--r--   0        0        0    22415 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/api.py
+-rw-r--r--   0        0        0     4887 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/app.py
+-rw-r--r--   0        0        0       48 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/auto.py
+-rw-r--r--   0        0        0     1184 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/config.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/dto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/dto/delivery_message/__init__.py
+-rw-r--r--   0        0        0      300 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/dto/delivery_message/delivery_message_request.py
+-rw-r--r--   0        0        0      183 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/dto/delivery_message/delivery_message_response.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/dto/orders/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/dto/orders/order_delivery_update_request.py
+-rw-r--r--   0        0        0       91 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/dto/orders/order_patch_request.py
+-rw-r--r--   0        0        0      662 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/dto/orders/orders_request.py
+-rw-r--r--   0        0        0      413 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/dto/orders/orders_response.py
+-rw-r--r--   0        0        0     2598 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/ext.py
+-rw-r--r--   0        0        0       29 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/invoices/__init__.py
+-rw-r--r--   0        0        0     4793 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0        0        0     8171 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0        0        0     2838 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0        0        0     4956 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0        0        0     7715 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/invoices/views.py
+-rw-r--r--   0        0        0      354 2024-04-16 14:26:30.556189 cg-60.0.0/cg/server/templates/admin/index.html
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/analysis_service/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/analysis_service/analysis_service.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/__init__.py
+-rw-r--r--   0        0        0     1942 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/delivery_message_service.py
+-rw-r--r--   0        0        0      792 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/__init__.py
+-rw-r--r--   0        0        0     1366 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/analysis_scout_message.py
+-rw-r--r--   0        0        0      791 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/covid_message.py
+-rw-r--r--   0        0        0      189 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/delivery_message.py
+-rw-r--r--   0        0        0     1391 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
+-rw-r--r--   0        0        0      535 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/fastq_message.py
+-rw-r--r--   0        0        0     1358 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/fastq_scout_message.py
+-rw-r--r--   0        0        0      604 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/microsalt_mwr_message.py
+-rw-r--r--   0        0        0      592 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/microsalt_mwx_message.py
+-rw-r--r--   0        0        0      903 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/scout_message.py
+-rw-r--r--   0        0        0      512 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/statina_message.py
+-rw-r--r--   0        0        0      779 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/messages/utils.py
+-rw-r--r--   0        0        0     3300 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/delivery_message/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/fastq_file_service/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/fastq_file_service/exceptions.py
+-rw-r--r--   0        0        0     1092 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/fastq_file_service/fastq_file_service.py
+-rw-r--r--   0        0        0     2991 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/fastq_file_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/order_service/__init__.py
+-rw-r--r--   0        0        0     2598 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/order_service/order_service.py
+-rw-r--r--   0        0        0     1214 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/order_service/utils.py
+-rw-r--r--   0        0        0       94 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/order_status_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/order_status_service/dto/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/order_status_service/dto/case_summary.py
+-rw-r--r--   0        0        0      289 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/order_status_service/dto/order_summary.py
+-rw-r--r--   0        0        0     1768 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/order_status_service/order_summary_service.py
+-rw-r--r--   0        0        0     1737 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/orders/order_status_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/slurm_service/__init__.py
+-rw-r--r--   0        0        0      703 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/slurm_service/slurm_cli_service.py
+-rw-r--r--   0        0        0      242 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/slurm_service/slurm_service.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/slurm_upload_service/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/slurm_upload_service/slurm_upload_config.py
+-rw-r--r--   0        0        0     2074 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/slurm_upload_service/slurm_upload_service.py
+-rw-r--r--   0        0        0      203 2024-04-16 14:26:30.556189 cg-60.0.0/cg/services/slurm_upload_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/base.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/crud/__init__.py
+-rw-r--r--   0        0        0    13100 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/crud/create.py
+-rw-r--r--   0        0        0     2144 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/crud/delete.py
+-rw-r--r--   0        0        0    60195 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/crud/read.py
+-rw-r--r--   0        0        0     1121 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/crud/update.py
+-rw-r--r--   0        0        0     1662 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/database.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/__init__.py
+-rw-r--r--   0        0        0     5371 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0        0        0     1712 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_application_filters.py
+-rw-r--r--   0        0        0     1440 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_application_limitations_filters.py
+-rw-r--r--   0        0        0     2523 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0        0        0     1390 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0        0        0     1317 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0        0        0    10787 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_case_filters.py
+-rw-r--r--   0        0        0     3272 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0        0        0      903 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0        0        0     1412 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0        0        0     1880 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0        0        0     1255 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0        0        0     2792 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0        0        0     3087 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_order_filters.py
+-rw-r--r--   0        0        0      851 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0        0        0      783 2024-04-16 14:26:30.556189 cg-60.0.0/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0        0        0     3923 2024-04-16 14:26:30.560189 cg-60.0.0/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0        0        0     8660 2024-04-16 14:26:30.560189 cg-60.0.0/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0        0        0      731 2024-04-16 14:26:30.560189 cg-60.0.0/cg/store/filters/status_user_filters.py
+-rw-r--r--   0        0        0    36844 2024-04-16 14:26:30.560189 cg-60.0.0/cg/store/models.py
+-rw-r--r--   0        0        0      593 2024-04-16 14:26:30.560189 cg-60.0.0/cg/store/store.py
+-rw-r--r--   0        0        0       30 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/calculations.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/checksum/__init__.py
+-rw-r--r--   0        0        0     1579 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/checksum/checksum.py
+-rw-r--r--   0        0        0     1655 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/click/EnumChoice.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/click/__init__.py
+-rw-r--r--   0        0        0     4910 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/commands.py
+-rw-r--r--   0        0        0     1811 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/date.py
+-rw-r--r--   0        0        0      635 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/dict.py
+-rw-r--r--   0        0        0     2111 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/dispatcher.py
+-rw-r--r--   0        0        0     1251 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/email.py
+-rw-r--r--   0        0        0      134 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/enums.py
+-rw-r--r--   0        0        0     3178 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/files.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/flask/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/flask/enum.py
+-rw-r--r--   0        0        0      834 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/time.py
+-rw-r--r--   0        0        0     1224 2024-04-16 14:26:30.560189 cg-60.0.0/cg/utils/utils.py
+-rw-r--r--   0        0        0     1697 2024-04-16 14:26:30.560189 cg-60.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.560189 cg-60.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-16 14:26:30.560189 cg-60.0.0/tests/apps/conftest.py
+-rw-r--r--   0        0        0      231 2024-04-16 14:26:30.560189 cg-60.0.0/tests/apps/coverage/conftest.py
+-rw-r--r--   0        0        0     6188 2024-04-16 14:26:30.560189 cg-60.0.0/tests/apps/coverage/test_coverage.py
+-rw-r--r--   0        0        0     1693 2024-04-16 14:26:30.560189 cg-60.0.0/tests/apps/crunchy/conftest.py
+-rw-r--r--   0        0        0     5438 2024-04-16 14:26:30.560189 cg-60.0.0/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0        0        0     2283 2024-04-16 14:26:30.560189 cg-60.0.0/tests/apps/crunchy/test_config.py
+-rw-r--r--   0        0        0    14032 2024-04-16 14:26:30.560189 cg-60.0.0/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0        0        0     9109 2024-04-16 14:26:30.560189 cg-60.0.0/tests/apps/crunchy/test_spring_decompression.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.560189 cg-60.0.0/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    11124 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0        0        0     4383 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     7942 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0        0        0     5729 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0        0        0     9468 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_override_cycles_validator.py
+-rw-r--r--   0        0        0     5248 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0        0        0    15738 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_sample_models.py
+-rw-r--r--   0        0        0     1050 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0        0        0     3245 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_sample_sheet_models.py
+-rw-r--r--   0        0        0    10932 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_sample_sheet_validator.py
+-rw-r--r--   0        0        0     7037 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_translate_sample_sheet.py
+-rw-r--r--   0        0        0     1495 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/demultiplex/test_validate.py
+-rw-r--r--   0        0        0     5094 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/downsample/test_downsample.py
+-rw-r--r--   0        0        0     1419 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/downsample/test_downsample_utils.py
+-rw-r--r--   0        0        0     1716 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/gens/test_gens_api.py
+-rw-r--r--   0        0        0     1950 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/gt/conftest.py
+-rw-r--r--   0        0        0     4276 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/gt/test_gt_api.py
+-rw-r--r--   0        0        0     1453 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/hk/conftest.py
+-rw-r--r--   0        0        0      684 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0        0        0     1593 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/hk/test_add_file.py
+-rw-r--r--   0        0        0     3523 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/hk/test_bundles.py
+-rw-r--r--   0        0        0      871 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/hk/test_core.py
+-rw-r--r--   0        0        0    31172 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/hk/test_file.py
+-rw-r--r--   0        0        0     5080 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/hk/test_version.py
+-rw-r--r--   0        0        0     1840 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/lims/conftest.py
+-rw-r--r--   0        0        0     3197 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/lims/test_api.py
+-rw-r--r--   0        0        0     1451 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/lims/test_sample_sheet.py
+-rw-r--r--   0        0        0     9223 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/loqus/conftest.py
+-rw-r--r--   0        0        0     8994 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/loqus/test_loqusdb_api.py
+-rw-r--r--   0        0        0     2439 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/madeline/conftest.py
+-rw-r--r--   0        0        0     4653 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/madeline/test_madeline.py
+-rw-r--r--   0        0        0     3328 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/mip/conftest.py
+-rw-r--r--   0        0        0     2487 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/mip/test_config_mip.py
+-rw-r--r--   0        0        0      883 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0        0        0     2473 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/mutacc_auto/test_mutacc_auto.py
+-rw-r--r--   0        0        0    11930 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/orderform/conftest.py
+-rw-r--r--   0        0        0     9484 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0        0        0     4351 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0        0        0     1032 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0        0        0     2474 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/orderform/test_orderform_parser.py
+-rw-r--r--   0        0        0    16002 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/orderform/validators/test_excel_sample_validators.py
+-rw-r--r--   0        0        0     3670 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/scout/conftest.py
+-rw-r--r--   0        0        0     2269 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0        0        0     1376 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0        0        0     1840 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0        0        0     7047 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/scout/test_scout_models.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     2861 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/sequencing_metrics_parser/conftest.py
+-rw-r--r--   0        0        0     2010 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0        0        0     1820 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
+-rw-r--r--   0        0        0     1908 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0        0        0     2997 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0        0        0     7322 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0        0        0     1458 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
+-rw-r--r--   0        0        0     1131 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/slurm/conftest.py
+-rw-r--r--   0        0        0     4412 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0        0        0      831 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/test_apps_environ.py
+-rw-r--r--   0        0        0      957 2024-04-16 14:26:30.564189 cg-60.0.0/tests/apps/test_osticket.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/add/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/add/test_cli_add.py
+-rw-r--r--   0        0        0     2471 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0        0        0     6841 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0        0        0     7588 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0        0        0     8382 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/add/test_cli_add_sample.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/backup/__init__.py
+-rw-r--r--   0        0        0      705 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/backup/conftest.py
+-rw-r--r--   0        0        0    11101 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/backup/test_backup_command.py
+-rw-r--r--   0        0        0     6865 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/clean/conftest.py
+-rw-r--r--   0        0        0     5536 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0        0        0     2557 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/clean/test_clean_flow_cell.py
+-rw-r--r--   0        0        0     1830 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0        0        0     2098 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0        0        0     4610 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0        0        0     3585 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0        0        0     1881 2024-04-16 14:26:30.564189 cg-60.0.0/tests/cli/clean/test_rsync_past_run_dirs.py
+-rw-r--r--   0        0        0     9707 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/compress/conftest.py
+-rw-r--r--   0        0        0     7709 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0        0        0     1416 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0        0        0     5205 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0        0        0     1239 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0        0        0     7558 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12747 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0        0        0     1873 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/delete/test_cli_delete_cases.py
+-rw-r--r--   0        0        0     3794 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/deliver/conftest.py
+-rw-r--r--   0        0        0     4428 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0        0        0     1166 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0        0        0     8569 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/deliver/test_run_deliver_cmd.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0     5273 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     4880 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0        0        0     1607 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0        0        0     2989 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/demultiplex/test_validate_sample_sheet.py
+-rw-r--r--   0        0        0     4423 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/demultiplex/test_verify_syncing.py
+-rw-r--r--   0        0        0     1585 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/downsample/test_cli_downsample.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/generate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/generate/report/conftest.py
+-rw-r--r--   0        0        0     2477 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0        0        0     2760 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0        0        0      563 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/generate/test_cli_base.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/get/__init__.py
+-rw-r--r--   0        0        0      863 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/get/test_cli_get.py
+-rw-r--r--   0        0        0     1526 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0        0        0     1242 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0        0        0     6208 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0        0        0     8835 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/get/test_cli_get_sample.py
+-rw-r--r--   0        0        0     1364 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/set/conftest.py
+-rw-r--r--   0        0        0     7311 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0        0        0     1460 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0        0        0     2016 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0        0        0     1685 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0        0        0    12450 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0        0        0     6124 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/set/test_cli_set_samples.py
+-rw-r--r--   0        0        0     6934 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/store/test_store.py
+-rw-r--r--   0        0        0     2332 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/test_base.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/__init__.py
+-rw-r--r--   0        0        0    10003 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/conftest.py
+-rw-r--r--   0        0        0     2295 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0        0        0     1789 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0        0        0      971 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0        0        0     1669 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0        0        0      895 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0        0        0     1199 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0        0        0      694 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0        0        0     9965 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0        0        0     4684 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0        0        0     1839 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0        0        0     6177 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/__init__.py
+-rw-r--r--   0        0        0    30612 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0        0        0    13938 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0        0        0     7957 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0        0        0     2336 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0        0        0     3554 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0        0        0     6209 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0        0        0     6934 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0        0        0     8458 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     2298 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/fastq/test_fastq_base.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     5291 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0        0        0     5687 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0        0        0     3302 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0        0        0     1896 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0        0        0     2968 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0        0        0     7815 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/fluffy/test_cli_store.py
+-rw-r--r--   0        0        0     2775 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0     6926 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0        0        0     1000 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/microsalt/test_microsalt_run.py
+-rw-r--r--   0        0        0     6544 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0        0        0     7011 2024-04-16 14:26:30.568189 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0        0        0     1542 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0        0        0      431 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0        0        0     2108 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
+-rw-r--r--   0        0        0     1273 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0        0        0     3595 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0        0        0     3884 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0        0        0     1004 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0        0        0      527 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0        0        0      716 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0        0        0     8559 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_store.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/nf_analysis/__init__.py
+-rw-r--r--   0        0        0     7365 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_config_case.py
+-rw-r--r--   0        0        0     3765 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
+-rw-r--r--   0        0        0     5087 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
+-rw-r--r--   0        0        0     9211 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_run.py
+-rw-r--r--   0        0        0     2994 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_start.py
+-rw-r--r--   0        0        0     9877 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_store.py
+-rw-r--r--   0        0        0    10373 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
+-rw-r--r--   0        0        0      915 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
+-rw-r--r--   0        0        0     3940 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
+-rw-r--r--   0        0        0      921 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0        0        0     4310 2024-04-16 14:26:30.572188 cg-60.0.0/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/clients/arnold/__init__.py
+-rw-r--r--   0        0        0     1080 2024-04-16 14:26:30.572188 cg-60.0.0/tests/clients/arnold/conftest.py
+-rw-r--r--   0        0        0     1503 2024-04-16 14:26:30.572188 cg-60.0.0/tests/clients/arnold/test_arnold_api_client.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/clients/janus/__init__.py
+-rw-r--r--   0        0        0     2381 2024-04-16 14:26:30.572188 cg-60.0.0/tests/clients/janus/conftest.py
+-rw-r--r--   0        0        0     1716 2024-04-16 14:26:30.572188 cg-60.0.0/tests/clients/janus/test_janus_api_client.py
+-rw-r--r--   0        0        0   126958 2024-04-16 14:26:30.572188 cg-60.0.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/delivery_fixtures/__init__.py
+-rw-r--r--   0        0        0     2653 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
+-rw-r--r--   0        0        0     4972 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
+-rw-r--r--   0        0        0     1494 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/__init__.py
+-rw-r--r--   0        0        0     4446 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
+-rw-r--r--   0        0        0     3686 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
+-rw-r--r--   0        0        0    21560 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0     3699 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
+-rw-r--r--   0        0        0     4346 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
+-rw-r--r--   0        0        0     6514 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
+-rw-r--r--   0        0        0     1304 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixture_plugins/timestamp_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+-rw-r--r--   0        0        0    14644 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+-rw-r--r--   0        0        0    15921 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0        0        0       70 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/nf-analysis/pipeline_params.config
+-rw-r--r--   0        0        0      195 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
+-rw-r--r--   0        0        0      195 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/nf-analysis/platform.config
+-rw-r--r--   0        0        0     5497 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0        0        0    12499 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     2873 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/sample_coverage.bed
+-rw-r--r--   0        0        0     6506 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/taxprofiler/multiqc_data.json
+-rw-r--r--   0        0        0    10513 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5771 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/tomte/multiqc_data.json
+-rw-r--r--   0        0        0    14859 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    10961 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0        0        0     3465 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0        0        0       63 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0        0        0      165 2024-04-16 14:26:30.572188 cg-60.0.0/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0        0        0     2705 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+-rw-r--r--   0        0        0      692 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/crunchy/spring_metadata.json
+-rw-r--r--   0        0        0      156 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/demuxcomplete.txt
+-rw-r--r--   0        0        0     1781 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json
+-rw-r--r--   0        0        0     2532 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json
+-rw-r--r--   0        0        0     1757 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0        7 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     6034 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        7 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
+-rw-r--r--   0        0        0        7 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      345 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      650 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      896 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      602 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/demuxcomplete.txt
+-rw-r--r--   0        0        0      315 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      434 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0     8624 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0        0        0      568 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      220 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      463 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      622 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      345 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      650 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      896 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      619 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     4439 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0       43 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338370 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-16 14:26:30.576188 cg-60.0.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338349 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
+-rw-r--r--   0        0        0     2126 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1827 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0       90 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6895 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
+-rw-r--r--   0        0        0       37 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
+-rw-r--r--   0        0        0    24755 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
+-rw-r--r--   0        0        0      692 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0      724 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
+-rw-r--r--   0        0        0     5775 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
+-rw-r--r--   0        0        0     2282 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1632 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
+-rw-r--r--   0        0        0       75 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6912 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
+-rw-r--r--   0        0        0       36 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
+-rw-r--r--   0        0        0    24814 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
+-rw-r--r--   0        0        0      814 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
+-rw-r--r--   0        0        0      660 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
+-rw-r--r--   0        0        0     5853 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    21848 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    15512 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       79 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      756 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     4118 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0     1408 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5326 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    15041 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    10649 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       80 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      755 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     2878 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0      928 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5359 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
+-rw-r--r--   0        0        0    27887 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0   141870 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
+-rwxr-xr-x   0        0        0   122682 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0      243 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0    28230 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
+-rw-r--r--   0        0        0    94426 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
+-rw-r--r--   0        0        0     5819 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     5945 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      260 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.580188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
+-rw-r--r--   0        0        0     1757 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0    47522 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
+-rw-r--r--   0        0        0       12 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6666 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0        0        0      254 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
+-rwxr-xr-x   0        0        0    47434 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
+-rw-r--r--   0        0        0    10950 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0      225 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
+-rw-r--r--   0        0        0       55 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2493 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
+-rwxr-xr-x   0        0        0        1 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
+-rwxr-xr-x   0        0        0        2 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
+-rwxr-xr-x   0        0        0      730 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0        0        0    79277 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
+-rwxr-xr-x   0        0        0     2694 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      619 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
+-rw-r--r--   0        0        0     4941 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
+-rwxr-xr-x   0        0        0    20050 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
+-rw-r--r--   0        0        0      244 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6391 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
+-rw-r--r--   0        0        0    16428 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
+-rw-r--r--   0        0        0     6728 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0     5127 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
+-rw-r--r--   0        0        0      133 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0      724 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0     5775 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0      124 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0      310 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0     5819 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0      122 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2694 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0      311 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6728 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.584188 cg-60.0.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
+-rw-r--r--   0        0        0   111989 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0        0        0     5319 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
+-rw-r--r--   0        0        0     5944 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2481 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2474 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
+-rw-r--r--   0        0        0     5899 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+-rw-r--r--   0        0        0     4941 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
+-rw-r--r--   0        0        0    10950 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0        0        0     5554 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0        0        0      901 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/fluffy/summary.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/gt/yellowhog.bcf
+-rw-r--r--   0        0        0     5114 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/madeline/madeline.xml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0        0        0     3241 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    21811 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0        0        0    23364 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    37367 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0       16 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0        0        0       16 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0       16 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0        0        0      123 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0        0        0    62741 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+-rw-r--r--   0        0        0    11242 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0        0        0    12164 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+-rw-r--r--   0        0        0     5231 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0        0        0     9774 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0        0        0     4624 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    13666 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/mip/sample_file.txt
+-rw-r--r--   0        0        0     1885 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0        0        0     6027 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0        0        0     9349 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0        0        0     1315 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0        0        0     3518 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0        0        0     8874 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0        0        0     4169 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/scout/panel_export.csv
+-rw-r--r--   0        0        0    63569 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0    42478 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0    69708 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      582 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
+-rw-r--r--   0        0        0       42 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/apps/shipping/scout-deploy.yaml
+-rw-r--r--   0        0        0     1036 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0        0        0     1104 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0        0        0     1313 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0        0        0     3038 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0        0        0     3705 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0        0        0     1364 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0        0        0     2125 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0        0        0     1368 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0        0        0     4684 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/cgweb_orders/sarscov2.json
+-rw-r--r--   0        0        0     5609 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0        0        0      511 2024-04-16 14:26:30.588189 cg-60.0.0/tests/fixtures/data/bcl_convert_sample_sheet.csv
+-rw-r--r--   0        0        0   258048 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0        0        0    49152 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/data/hkstore.db
+-rw-r--r--   0        0        0       73 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/data/yellowhog/pedigree.yaml
+-rw-r--r--   0        0        0       76 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/casava_five_parts.fastq.gz
+-rw-r--r--   0        0        0       90 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/casava_seven_parts.fastq.gz
+-rw-r--r--   0        0        0       96 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/casava_ten_parts.fastq.gz
+-rw-r--r--   0        0        0      153 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/example.csv
+-rw-r--r--   0        0        0       46 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/example.gz
+-rw-r--r--   0        0        0      147 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/example.tsv
+-rw-r--r--   0        0        0       20 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/example.txt
+-rw-r--r--   0        0        0       20 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/example2.txt
+-rw-r--r--   0        0        0      582 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/example_json.json
+-rw-r--r--   0        0        0      103 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/io/example_xml.xml
+-rw-r--r--   0        0        0       20 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
+-rw-r--r--   0        0        0       20 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
+-rw-r--r--   0        0        0   156910 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/orderforms/1508.30.balsamic.xlsx
+-rw-r--r--   0        0        0   156770 2024-04-16 14:26:30.592188 cg-60.0.0/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
+-rw-r--r--   0        0        0   156737 2024-04-16 14:26:30.596188 cg-60.0.0/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
+-rw-r--r--   0        0        0   156582 2024-04-16 14:26:30.596188 cg-60.0.0/tests/fixtures/orderforms/1508.30.fastq.xlsx
+-rw-r--r--   0        0        0   155627 2024-04-16 14:26:30.596188 cg-60.0.0/tests/fixtures/orderforms/1508.30.metagenome.xlsx
+-rw-r--r--   0        0        0   156850 2024-04-16 14:26:30.596188 cg-60.0.0/tests/fixtures/orderforms/1508.30.mip.xlsx
+-rw-r--r--   0        0        0   258580 2024-04-16 14:26:30.596188 cg-60.0.0/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
+-rw-r--r--   0        0        0   258342 2024-04-16 14:26:30.596188 cg-60.0.0/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
+-rw-r--r--   0        0        0    82677 2024-04-16 14:26:30.596188 cg-60.0.0/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0        0        0   149394 2024-04-16 14:26:30.600188 cg-60.0.0/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0        0        0   223184 2024-04-16 14:26:30.600188 cg-60.0.0/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
+-rw-r--r--   0        0        0    18639 2024-04-16 14:26:30.600188 cg-60.0.0/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0        0        0     6052 2024-04-16 14:26:30.600188 cg-60.0.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     6611 2024-04-16 14:26:30.600188 cg-60.0.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     1417 2024-04-16 14:26:30.600188 cg-60.0.0/tests/fixtures/report/case_data.json
+-rw-r--r--   0        0        0     1109 2024-04-16 14:26:30.600188 cg-60.0.0/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0        0        0     1562 2024-04-16 14:26:30.600188 cg-60.0.0/tests/fixtures/report/lims_family.json
+-rw-r--r--   0        0        0     3296 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/conftest.py
+-rw-r--r--   0        0        0      431 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/test_io_config.py
+-rw-r--r--   0        0        0     8639 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/test_io_controller.py
+-rw-r--r--   0        0        0     3877 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/test_io_csv.py
+-rw-r--r--   0        0        0      482 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/test_io_gzip.py
+-rw-r--r--   0        0        0     1779 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/test_io_json.py
+-rw-r--r--   0        0        0     2914 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/test_io_txt.py
+-rw-r--r--   0        0        0     1027 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/test_io_xml.py
+-rw-r--r--   0        0        0     2131 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/test_io_yaml.py
+-rw-r--r--   0        0        0     1233 2024-04-16 14:26:30.600188 cg-60.0.0/tests/io/test_validate_path.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/archive/__init__.py
+-rw-r--r--   0        0        0    13131 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/archive/conftest.py
+-rw-r--r--   0        0        0    16858 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/archive/test_archive_api.py
+-rw-r--r--   0        0        0    10246 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/archive/test_archive_cli.py
+-rw-r--r--   0        0        0    15766 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/archive/test_archiving.py
+-rw-r--r--   0        0        0     3807 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/backup/conftest.py
+-rw-r--r--   0        0        0    26368 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0        0        0    10055 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/backup/test_meta_pdc.py
+-rw-r--r--   0        0        0    12546 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/clean/conftest.py
+-rw-r--r--   0        0        0    16944 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/clean/test_clean_flow_cells_api.py
+-rw-r--r--   0        0        0     2286 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/clean/test_clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0     7691 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/compress/conftest.py
+-rw-r--r--   0        0        0     7961 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0        0        0     1778 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0        0        0     3644 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0        0        0     1180 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0        0        0     6902 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0        0        0     8207 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/deliver/__init__.py
+-rw-r--r--   0        0        0     3471 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/deliver/conftest.py
+-rw-r--r--   0        0        0     5533 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0        0        0    10277 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/deliver/test_delivery_api.py
+-rw-r--r--   0        0        0     1057 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/deliver/test_fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/delivery/__init__.py
+-rw-r--r--   0        0        0    14910 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/delivery/test_delivery_api.py
+-rw-r--r--   0        0        0    12490 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0        0        0     5382 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/demultiplex/test_combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     9280 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0        0        0    12330 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/demultiplex/test_housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     4392 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/demultiplex/test_status_db_storage_functions.py
+-rw-r--r--   0        0        0    22708 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0        0        0     6193 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/demultiplex/test_validation.py
+-rw-r--r--   0        0        0     4943 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/encryption/conftest.py
+-rw-r--r--   0        0        0    18133 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/encryption/test_encryption.py
+-rw-r--r--   0        0        0     3122 2024-04-16 14:26:30.600188 cg-60.0.0/tests/meta/observations/conftest.py
+-rw-r--r--   0        0        0    16164 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/observations/test_meta_upload_observations.py
+-rw-r--r--   0        0        0     4974 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/conftest.py
+-rw-r--r--   0        0        0     1749 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0        0        0     1470 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0        0        0     1768 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0        0        0     2032 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0        0        0    19783 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0        0        0     7086 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0        0        0    29515 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0        0        0     1677 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0        0        0     1068 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/orders/test_ticket_handler.py
+-rw-r--r--   0        0        0     4336 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/qc_metrics/conftest.py
+-rw-r--r--   0        0        0     1972 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/qc_metrics/test_collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/report/__init__.py
+-rw-r--r--   0        0        0     5354 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/report/conftest.py
+-rw-r--r--   0        0        0      434 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/report/helper.py
+-rw-r--r--   0        0        0     4106 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0        0        0     4056 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/report/test_field_validators.py
+-rw-r--r--   0        0        0     2834 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0        0        0    16704 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/report/test_report_api.py
+-rw-r--r--   0        0        0     2546 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/report/test_rnafusion_api.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/rsync/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/rsync/conftest.py
+-rw-r--r--   0        0        0     9442 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0        0        0     3147 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/test_invoice.py
+-rw-r--r--   0        0        0     1220 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/transfer/conftest.py
+-rw-r--r--   0        0        0     9892 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0        0        0     4395 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/transfer/test_meta_transfer_lims.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0        0        0     4002 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0     2557 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0        0        0      211 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0        0        0      371 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0        0        0     3684 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0        0        0     4188 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+-rw-r--r--   0        0        0     1149 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0        0        0     1683 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/nipt/test_models.py
+-rw-r--r--   0        0        0     1242 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/nipt/test_nipt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0    23954 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0        0        0     4734 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0        0        0     4182 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0        0        0    33260 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0        0        0     7372 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0        0        0     2511 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0        0        0     1473 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0        0        0     2547 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/upload/test_upload_genotypes_api.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    10003 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/conftest.py
+-rw-r--r--   0        0        0     3652 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0      318 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/microsalt/test_parsing_metrics.py
+-rw-r--r--   0        0        0     3714 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/microsalt/test_quality_controller.py
+-rw-r--r--   0        0        0    14367 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/microsalt/test_quality_controller_utils.py
+-rw-r--r--   0        0        0      825 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/microsalt/test_report_generation.py
+-rw-r--r--   0        0        0    20848 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0        0        0     6238 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0        0        0     3034 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/test_fastq.py
+-rw-r--r--   0        0        0     1532 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0        0        0     2712 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/test_nf_analysis.py
+-rw-r--r--   0        0        0     7741 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0        0        0     1918 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/test_raredisease.py
+-rw-r--r--   0        0        0     1688 2024-04-16 14:26:30.604188 cg-60.0.0/tests/meta/workflow/test_rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.604188 cg-60.0.0/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1161 2024-04-16 14:26:30.604188 cg-60.0.0/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0        0        0     3500 2024-04-16 14:26:30.604188 cg-60.0.0/tests/mocks/crunchy.py
+-rw-r--r--   0        0        0    21778 2024-04-16 14:26:30.604188 cg-60.0.0/tests/mocks/hk_mock.py
+-rw-r--r--   0        0        0     3802 2024-04-16 14:26:30.604188 cg-60.0.0/tests/mocks/limsmock.py
+-rw-r--r--   0        0        0      572 2024-04-16 14:26:30.604188 cg-60.0.0/tests/mocks/madeline.py
+-rw-r--r--   0        0        0     1297 2024-04-16 14:26:30.604188 cg-60.0.0/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0        0        0     1525 2024-04-16 14:26:30.608188 cg-60.0.0/tests/mocks/osticket.py
+-rw-r--r--   0        0        0     3239 2024-04-16 14:26:30.608188 cg-60.0.0/tests/mocks/process_mock.py
+-rw-r--r--   0        0        0     3718 2024-04-16 14:26:30.608188 cg-60.0.0/tests/mocks/report.py
+-rw-r--r--   0        0        0     3915 2024-04-16 14:26:30.608188 cg-60.0.0/tests/mocks/scout.py
+-rw-r--r--   0        0        0      750 2024-04-16 14:26:30.608188 cg-60.0.0/tests/mocks/store_model.py
+-rw-r--r--   0        0        0     1532 2024-04-16 14:26:30.608188 cg-60.0.0/tests/mocks/tb_mock.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/balsamic/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/balsamic/conftest.py
+-rw-r--r--   0        0        0     1030 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0        0        0     1050 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0        0        0    11446 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/demultiplexing/test_run_parameters.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/downsample/__init__.py
+-rw-r--r--   0        0        0     2096 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/downsample/test_down_sample_meta_data.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     8715 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/flow_cell/test_flowcell_model.py
+-rw-r--r--   0        0        0     6637 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/mip/conftest.py
+-rw-r--r--   0        0        0     1239 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0        0        0     2348 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/mip/test_mip_config.py
+-rw-r--r--   0        0        0     6392 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     3959 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/mip/test_mip_sample_info.py
+-rw-r--r--   0        0        0     3314 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/nextflow/test_nextflow_deliver.py
+-rw-r--r--   0        0        0     1602 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/observations/conftest.py
+-rw-r--r--   0        0        0     2579 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/observations/test_observations_input_files.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/report/__init__.py
+-rw-r--r--   0        0        0     7327 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/report/test_validators.py
+-rw-r--r--   0        0        0     3855 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0        0        0     1374 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/test_cg_models.py
+-rw-r--r--   0        0        0      990 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/test_compression_data.py
+-rw-r--r--   0        0        0      729 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/test_fastq.py
+-rw-r--r--   0        0        0     2860 2024-04-16 14:26:30.608188 cg-60.0.0/tests/models/test_file_data.py
+-rw-r--r--   0        0        0     4366 2024-04-16 14:26:30.608188 cg-60.0.0/tests/server/conftest.py
+-rw-r--r--   0        0        0     3135 2024-04-16 14:26:30.608188 cg-60.0.0/tests/server/endpoints/test_delivery_message_endpoint.py
+-rw-r--r--   0        0        0     3239 2024-04-16 14:26:30.608188 cg-60.0.0/tests/server/endpoints/test_orders_endpoint.py
+-rw-r--r--   0        0        0      271 2024-04-16 14:26:30.608188 cg-60.0.0/tests/server/test_server_auto.py
+-rw-r--r--   0        0        0     1047 2024-04-16 14:26:30.608188 cg-60.0.0/tests/services/fastq_file_service/conftest.py
+-rw-r--r--   0        0        0     3634 2024-04-16 14:26:30.608188 cg-60.0.0/tests/services/fastq_file_service/test_fastq_file_service.py
+-rw-r--r--   0        0        0     4861 2024-04-16 14:26:30.608188 cg-60.0.0/tests/services/orders/order_status_service/conftest.py
+-rw-r--r--   0        0        0     2865 2024-04-16 14:26:30.608188 cg-60.0.0/tests/services/orders/order_status_service/test_order_summary_service.py
+-rw-r--r--   0        0        0      318 2024-04-16 14:26:30.608188 cg-60.0.0/tests/small_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/api/__init__.py
+-rw-r--r--   0        0        0     2984 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/api/conftest.py
+-rw-r--r--   0        0        0     1557 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/api/test_base.py
+-rw-r--r--   0        0        0    20096 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/add/__init__.py
+-rw-r--r--   0        0        0     1497 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/add/test_store_add_application_version.py
+-rw-r--r--   0        0        0     3958 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/add/test_store_add_base.py
+-rw-r--r--   0        0        0     2502 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/add/test_store_add_customer.py
+-rw-r--r--   0        0        0     1640 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/add/test_store_add_flow_celll.py
+-rw-r--r--   0        0        0    12212 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/delete/__init__.py
+-rw-r--r--   0        0        0     5541 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/delete/test_delete.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/read/__init__.py
+-rw-r--r--   0        0        0    57211 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/read/test_read.py
+-rw-r--r--   0        0        0     5461 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/read/test_read_analyses_to_clean.py
+-rw-r--r--   0        0        0     3553 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/read/test_read_analyses_to_delivery_report.py
+-rw-r--r--   0        0        0    18463 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/read/test_read_analysis.py
+-rw-r--r--   0        0        0     2743 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/read/test_read_application_version.py
+-rw-r--r--   0        0        0     1105 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/read/test_read_customer.py
+-rw-r--r--   0        0        0     1530 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/read/test_read_pool.py
+-rw-r--r--   0        0        0    21602 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/read/test_read_sample.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/update/__init__.py
+-rw-r--r--   0        0        0      737 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/crud/update/test_update.py
+-rw-r--r--   0        0        0    11693 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0        0        0     3397 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0        0        0     2073 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/filters/test_status_application_limitations_filters.py
+-rw-r--r--   0        0        0    10452 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0        0        0     2804 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0        0        0     2362 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0        0        0     3495 2024-04-16 14:26:30.608188 cg-60.0.0/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0        0        0    39100 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0        0        0     1345 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0        0        0     2482 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0        0        0     4907 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0        0        0     2226 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0        0        0     5970 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0        0        0     2404 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0        0        0     1804 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0        0        0     8720 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0        0        0    22875 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0        0        0     1576 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0        0        0     2147 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/test_delivery.py
+-rw-r--r--   0        0        0     4127 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store/test_store_models.py
+-rw-r--r--   0        0        0    36339 2024-04-16 14:26:30.612188 cg-60.0.0/tests/store_helpers.py
+-rw-r--r--   0        0        0     4930 2024-04-16 14:26:30.612188 cg-60.0.0/tests/test_copy_novaseqx_flow_cell.py
+-rw-r--r--   0        0        0      911 2024-04-16 14:26:30.612188 cg-60.0.0/tests/test_store_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1754 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/conftest.py
+-rw-r--r--   0        0        0      371 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/test_calculations.py
+-rw-r--r--   0        0        0     2920 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      953 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/test_date.py
+-rw-r--r--   0        0        0     1508 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/test_dict.py
+-rw-r--r--   0        0        0     7154 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/test_dispatcher.py
+-rw-r--r--   0        0        0     4100 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1170 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/test_time.py
+-rw-r--r--   0        0        0     2366 2024-04-16 14:26:30.612188 cg-60.0.0/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.0.0/PKG-INFO
```

### Comparing `cg-59.9.1/README.md` & `cg-60.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/coverage/api.py` & `cg-60.0.0/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/crunchy/crunchy.py` & `cg-60.0.0/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/crunchy/files.py` & `cg-60.0.0/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/crunchy/sbatch.py` & `cg-60.0.0/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/demultiplex/demultiplex_api.py` & `cg-60.0.0/cg/apps/demultiplex/demultiplex_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 
     @staticmethod
     def get_sbatch_command(
         run_dir: Path,
         demux_dir: Path,
         sample_sheet: Path,
         demux_completed: Path,
-        flow_cell: FlowCellDirectoryData,
         environment: Literal["production", "stage"] = "stage",
     ) -> str:
         """
         Return sbatch command.
         The unaligned_dir is only used for Bcl2Fastq.
         """
         LOG.debug("Creating the sbatch command string")
@@ -89,17 +88,15 @@
             run_dir=run_dir.as_posix(),
             demux_dir=demux_dir.as_posix(),
             unaligned_dir=unaligned_dir.as_posix(),
             sample_sheet=sample_sheet.as_posix(),
             demux_completed_file=demux_completed.as_posix(),
             environment=environment,
         )
-        return DEMULTIPLEX_COMMAND[flow_cell.bcl_converter].format(
-            **command_parameters.model_dump()
-        )
+        return DEMULTIPLEX_COMMAND.format(**command_parameters.model_dump())
 
     @staticmethod
     def demultiplex_sbatch_path(flow_cell: FlowCellDirectoryData) -> Path:
         """Get the path to where sbatch script file should be kept."""
         return Path(flow_cell.path, "demux-novaseq.sh")
 
     @staticmethod
@@ -220,43 +217,26 @@
             flow_cell=flow_cell, email=self.mail, demux_dir=self.flow_cell_out_dir_path(flow_cell)
         )
         commands: str = self.get_sbatch_command(
             run_dir=flow_cell.path,
             demux_dir=self.flow_cell_out_dir_path(flow_cell=flow_cell),
             sample_sheet=flow_cell.sample_sheet_path,
             demux_completed=self.demultiplexing_completed_path(flow_cell=flow_cell),
-            flow_cell=flow_cell,
             environment=self.environment,
         )
-
-        if flow_cell.bcl_converter == BclConverter.BCL2FASTQ:
-            sbatch_parameters: Sbatch = Sbatch(
-                account=self.slurm_account,
-                commands=commands,
-                email=self.mail,
-                error=error_function,
-                hours=36,
-                job_name=self.get_run_name(flow_cell),
-                log_dir=log_path.parent.as_posix(),
-                memory=125,
-                number_tasks=18,
-                quality_of_service=self.slurm_quality_of_service,
-            )
-        if flow_cell.bcl_converter == BclConverter.BCLCONVERT:
-            sbatch_parameters: SbatchDragen = SbatchDragen(
-                account=self.slurm_account,
-                commands=commands,
-                email=self.mail,
-                error=error_function,
-                hours=36,
-                job_name=self.get_run_name(flow_cell),
-                log_dir=log_path.parent.as_posix(),
-                quality_of_service=self.slurm_quality_of_service,
-            )
-
+        sbatch_parameters: SbatchDragen = SbatchDragen(
+            account=self.slurm_account,
+            commands=commands,
+            email=self.mail,
+            error=error_function,
+            hours=36,
+            job_name=self.get_run_name(flow_cell),
+            log_dir=log_path.parent.as_posix(),
+            quality_of_service=self.slurm_quality_of_service,
+        )
         sbatch_content: str = self.slurm_api.generate_sbatch_content(
             sbatch_parameters=sbatch_parameters
         )
         sbatch_path: Path = self.demultiplex_sbatch_path(flow_cell=flow_cell)
         sbatch_number: int = self.slurm_api.submit_sbatch(
             sbatch_content=sbatch_content, sbatch_path=sbatch_path
         )
@@ -269,13 +249,11 @@
         self.create_demultiplexing_output_dir(flow_cell)
 
     def remove_demultiplexing_output_directory(self, flow_cell: FlowCellDirectoryData) -> None:
         if not self.dry_run and self.flow_cell_out_dir_path(flow_cell=flow_cell).exists():
             shutil.rmtree(self.flow_cell_out_dir_path(flow_cell=flow_cell), ignore_errors=False)
 
     def create_demultiplexing_output_dir(self, flow_cell: FlowCellDirectoryData) -> None:
-        """Creates the demultiplexing output directory and, if necessary, the unaligned directory."""
+        """Creates the demultiplexing output directory for the flow cell."""
         output_directory: Path = self.flow_cell_out_dir_path(flow_cell)
         LOG.debug(f"Creating demultiplexing output directory: {output_directory}")
         output_directory.mkdir(exist_ok=False, parents=True)
-        if flow_cell.bcl_converter == BclConverter.BCL2FASTQ:
-            self.get_flow_cell_unaligned_dir(flow_cell).mkdir(exist_ok=False, parents=False)
```

### Comparing `cg-59.9.1/cg/apps/demultiplex/sample_sheet/api.py` & `cg-60.0.0/cg/apps/demultiplex/sample_sheet/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 import logging
 from pathlib import Path
 
 import click
 
-from cg.apps.demultiplex.sample_sheet.create import create_sample_sheet_content
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
+from cg.apps.demultiplex.sample_sheet.read_sample_sheet import (
+    get_flow_cell_samples_from_content,
+    get_sample_type_from_content,
+)
+from cg.apps.demultiplex.sample_sheet.sample_models import (
+    FlowCellSampleBcl2Fastq,
+    FlowCellSampleBCLConvert,
+)
+from cg.apps.demultiplex.sample_sheet.sample_sheet_creator import SampleSheetCreator
 from cg.apps.demultiplex.sample_sheet.sample_sheet_validator import SampleSheetValidator
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.apps.lims import LimsAPI
 from cg.apps.lims.sample_sheet import get_flow_cell_samples
 from cg.constants.constants import FileFormat
+from cg.constants.demultiplexing import (
+    BclConverter,
+    SampleSheetBcl2FastqSections,
+    SampleSheetBCLConvertSections,
+)
 from cg.exc import FlowCellError, HousekeeperFileMissingError, SampleSheetError
-from cg.io.controller import WriteFile, WriteStream
+from cg.io.controller import ReadFile, WriteFile, WriteStream
 from cg.meta.demultiplex.housekeeper_storage_functions import (
     add_and_include_sample_sheet_path_to_housekeeper,
     delete_sample_sheet_from_housekeeper,
 )
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 from cg.utils.files import get_directories_in_path, link_or_overwrite_file
 
@@ -28,15 +40,14 @@
     def __init__(self, flow_cell_dir: str, hk_api: HousekeeperAPI, lims_api: LimsAPI) -> None:
         self.flow_cell_runs_dir = Path(flow_cell_dir)
         self.hk_api: HousekeeperAPI = hk_api
         self.lims_api: LimsAPI = lims_api
         self.dry_run: bool = False
         self.force: bool = False
         self.validator = SampleSheetValidator()
-        self.bcl_converter: str | None = None
 
     def set_dry_run(self, dry_run: bool) -> None:
         """Set dry run."""
         LOG.debug(f"Set dry run to {dry_run}")
         self.dry_run = dry_run
 
     def set_force(self, force: bool) -> None:
@@ -61,85 +72,168 @@
             flow_cell = FlowCellDirectoryData(
                 flow_cell_path=flow_cell_path, bcl_converter=bcl_converter
             )
         except FlowCellError as error:
             raise SampleSheetError from error
         return flow_cell
 
-    def validate_sample_sheet(
-        self, sample_sheet_path: Path, bcl_converter: str | None = None
-    ) -> None:
+    def validate_sample_sheet(self, sample_sheet_path: Path) -> None:
         """Return the sample sheet path if it exists and if it passes validation.
         Raises:
             SampleSheetError: If the sample sheet does not exist or does not pass validation.
         """
         if not (sample_sheet_path and sample_sheet_path.exists()):
             message: str = f"Sample sheet with path {sample_sheet_path} does not exist"
             LOG.error(message)
             raise SampleSheetError(message)
-        self.validator.validate_sample_sheet_from_file(
-            file_path=sample_sheet_path, bcl_converter=bcl_converter
+        sample_sheet_content: list[list[str]] = ReadFile.get_content_from_file(
+            file_format=FileFormat.CSV, file_path=sample_sheet_path
+        )
+        self.validator.validate_sample_sheet_from_content(sample_sheet_content)
+
+    @staticmethod
+    def _are_necessary_files_in_flow_cell(flow_cell: FlowCellDirectoryData) -> bool:
+        """Determine if the flow cell has a Run Parameters file and a sample sheet."""
+        try:
+            flow_cell.run_parameters_path.exists()
+        except FlowCellError:
+            LOG.error(f"Run parameters file for flow cell {flow_cell.full_name} does not exist")
+            return False
+        if not flow_cell.sample_sheet_path.exists():
+            LOG.error(f"Sample sheet for flow cell {flow_cell.full_name} does not exist")
+            return False
+        return True
+
+    @staticmethod
+    def _is_sample_sheet_bcl2fastq(flow_cell: FlowCellDirectoryData) -> bool:
+        """Determine if the sample sheet from the flow cell directory is in BCL2FASTQ format."""
+        sample_sheet_content: list[list[str]] = ReadFile.get_content_from_file(
+            file_format=FileFormat.CSV, file_path=flow_cell.sample_sheet_path
+        )
+        if get_sample_type_from_content(sample_sheet_content) is not FlowCellSampleBcl2Fastq:
+            LOG.error(
+                f"Sample sheet for flow cell {flow_cell.full_name} is not a Bcl2Fastq sample sheet"
+            )
+            return False
+        return True
+
+    def _is_sample_sheet_from_flow_cell_translatable(
+        self, flow_cell: FlowCellDirectoryData
+    ) -> bool:
+        """
+        Determine if the sample sheet from the flow cell directory is translatable to BCLConvert.
+        """
+        return self._are_necessary_files_in_flow_cell(
+            flow_cell
+        ) and self._is_sample_sheet_bcl2fastq(flow_cell)
+
+    @staticmethod
+    def _replace_sample_header(sample_sheet_content: list[list[str]]) -> list[list[str]]:
+        """
+        Replace the old sample ID header in the Bcl2Fastq sample sheet content with the BCLConvert
+        formatted one.
+        Raises:
+            SampleSheetError: If the data header is not found in the sample sheet.
+        """
+        for line in sample_sheet_content:
+            if SampleSheetBcl2FastqSections.Data.SAMPLE_INTERNAL_ID_BCL2FASTQ.value in line:
+                idx = line.index(
+                    SampleSheetBcl2FastqSections.Data.SAMPLE_INTERNAL_ID_BCL2FASTQ.value
+                )
+                line[idx] = SampleSheetBCLConvertSections.Data.SAMPLE_INTERNAL_ID.value
+                return sample_sheet_content
+        raise SampleSheetError("Could not find data header in sample sheet")
+
+    def translate_sample_sheet(self, flow_cell_name: str) -> None:
+        """Translate a Bcl2Fastq sample sheet to a BCLConvert sample sheet."""
+        flow_cell: FlowCellDirectoryData = self._get_flow_cell(
+            flow_cell_name=flow_cell_name, bcl_converter=BclConverter.BCLCONVERT
+        )
+        if not self._is_sample_sheet_from_flow_cell_translatable(flow_cell):
+            raise SampleSheetError("Could not translate sample sheet")
+        original_content: list[list[str]] = ReadFile.get_content_from_file(
+            file_format=FileFormat.CSV, file_path=flow_cell.sample_sheet_path
+        )
+        content_with_fixed_header: list[list[str]] = self._replace_sample_header(original_content)
+
+        flow_cell_samples: list[FlowCellSampleBCLConvert] = get_flow_cell_samples_from_content(
+            sample_sheet_content=content_with_fixed_header, sample_type=FlowCellSampleBCLConvert
+        )
+        bcl_convert_creator = SampleSheetCreator(
+            flow_cell=flow_cell, lims_samples=flow_cell_samples
+        )
+        new_content = bcl_convert_creator.construct_sample_sheet()
+        self.validator.validate_sample_sheet_from_content(new_content)
+        if self.dry_run:
+            click.echo(
+                WriteStream.write_stream_from_content(
+                    file_format=FileFormat.CSV, content=new_content
+                )
+            )
+            return
+        WriteFile.write_file_from_content(
+            content=new_content,
+            file_format=FileFormat.CSV,
+            file_path=flow_cell.sample_sheet_path,
         )
 
     def _use_sample_sheet_from_housekeeper(self, flow_cell: FlowCellDirectoryData) -> None:
         """
         Copy the sample sheet from Housekeeper to the flow cell directory if it exists and is valid.
         """
         try:
             sample_sheet_path: Path = self.hk_api.get_sample_sheet_path(flow_cell.id)
         except HousekeeperFileMissingError:
             raise SampleSheetError(
                 f"Sample sheet for flow cell {flow_cell.id} does not exist in Housekeeper"
             )
-        self.validate_sample_sheet(
-            sample_sheet_path=sample_sheet_path, bcl_converter=self.bcl_converter
-        )
+        self.validate_sample_sheet(sample_sheet_path)
         LOG.info("Sample sheet from Housekeeper is valid. Copying it to flow cell directory")
         if not self.dry_run:
             link_or_overwrite_file(src=sample_sheet_path, dst=flow_cell.sample_sheet_path)
 
     def _use_flow_cell_sample_sheet(self, flow_cell: FlowCellDirectoryData) -> None:
         """Use the sample sheet from the flow cell directory if it is valid."""
-        self.validate_sample_sheet(
-            sample_sheet_path=flow_cell.sample_sheet_path, bcl_converter=self.bcl_converter
-        )
+        self.validate_sample_sheet(flow_cell.sample_sheet_path)
         LOG.info("Sample sheet from flow cell directory is valid. Adding it to Housekeeper")
         if not self.dry_run:
             try:
                 delete_sample_sheet_from_housekeeper(flow_cell_id=flow_cell.id, hk_api=self.hk_api)
             except HousekeeperFileMissingError:
                 pass
             add_and_include_sample_sheet_path_to_housekeeper(
                 flow_cell_directory=flow_cell.path,
                 flow_cell_name=flow_cell.id,
                 hk_api=self.hk_api,
             )
 
     def _get_sample_sheet_content(self, flow_cell: FlowCellDirectoryData) -> list[list[str]]:
         """Return the sample sheet content for a flow cell."""
-        lims_samples: list[FlowCellSample] = list(
+        lims_samples: list[FlowCellSampleBCLConvert] = list(
             get_flow_cell_samples(
                 lims=self.lims_api,
                 flow_cell_id=flow_cell.id,
                 flow_cell_sample_type=flow_cell.sample_type,
             )
         )
         if not lims_samples:
             message: str = f"Could not find any samples in LIMS for {flow_cell.id}"
             LOG.warning(message)
             raise SampleSheetError(message)
-        return create_sample_sheet_content(flow_cell=flow_cell, lims_samples=lims_samples)
+        creator = SampleSheetCreator(flow_cell=flow_cell, lims_samples=lims_samples)
+        LOG.info(
+            f"Constructing sample sheet for the {flow_cell.sequencer_type} flow cell {flow_cell.id}"
+        )
+        return creator.construct_sample_sheet()
 
     def _create_sample_sheet_file(self, flow_cell: FlowCellDirectoryData) -> None:
         """Create a valid sample sheet in the flow cell directory and add it to Housekeeper."""
         sample_sheet_content: list[list[str]] = self._get_sample_sheet_content(flow_cell)
         if not self.force:
-            self.validator.validate_sample_sheet_from_content(
-                content=sample_sheet_content, bcl_convert=flow_cell.bcl_converter
-            )
+            self.validator.validate_sample_sheet_from_content(sample_sheet_content)
         LOG.info(f"Writing sample sheet to {flow_cell.sample_sheet_path.resolve()}")
         if self.dry_run:
             click.echo(
                 WriteStream.write_stream_from_content(
                     file_format=FileFormat.CSV, content=sample_sheet_content
                 )
             )
@@ -153,20 +247,21 @@
             delete_sample_sheet_from_housekeeper(flow_cell_id=flow_cell.id, hk_api=self.hk_api)
         except HousekeeperFileMissingError:
             pass
         add_and_include_sample_sheet_path_to_housekeeper(
             flow_cell_directory=flow_cell.path, flow_cell_name=flow_cell.id, hk_api=self.hk_api
         )
 
-    def get_or_create_sample_sheet(self, flow_cell_name: str, bcl_converter: str | None) -> None:
+    def get_or_create_sample_sheet(
+        self, flow_cell_name: str, bcl_converter: str | None = None
+    ) -> None:
         """
         Ensure that a valid sample sheet is present in the flow cell directory by fetching it from
         housekeeper or creating it if there is not a valid sample sheet.
         """
-        self.bcl_converter = bcl_converter
         flow_cell: FlowCellDirectoryData = self._get_flow_cell(
             flow_cell_name=flow_cell_name, bcl_converter=bcl_converter
         )
         LOG.info("Fetching and validating sample sheet from Housekeeper")
         try:
             self._use_sample_sheet_from_housekeeper(flow_cell)
             return
@@ -185,12 +280,13 @@
         self._create_sample_sheet_file(flow_cell)
 
     def get_or_create_all_sample_sheets(self):
         """Ensure that a valid sample sheet is present in all flow cell directories."""
         for flow_cell_dir in get_directories_in_path(self.flow_cell_runs_dir):
             try:
                 self.get_or_create_sample_sheet(
-                    flow_cell_name=flow_cell_dir.name, bcl_converter=None
+                    flow_cell_name=flow_cell_dir.name,
+                    bcl_converter=BclConverter.BCLCONVERT,
                 )
             except Exception as error:
                 LOG.error(f"Could not create sample sheet for {flow_cell_dir.name}: {error}")
                 continue
```

### Comparing `cg-59.9.1/cg/apps/demultiplex/sample_sheet/index.py` & `cg-60.0.0/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Functions that deal with modifications of the indexes."""
 
 import logging
 
 from pydantic import BaseModel
 
-from cg.constants.constants import FileFormat
-from cg.io.controller import ReadFile
-from cg.resources import VALID_INDEXES_PATH
 from cg.utils.utils import get_hamming_distance
 
 LOG = logging.getLogger(__name__)
 DNA_COMPLEMENTS: dict[str, str] = {"A": "T", "C": "G", "G": "C", "T": "A"}
 INDEX_ONE_PAD_SEQUENCE: str = "AT"
 INDEX_TWO_PAD_SEQUENCE: str = "AC"
 LONG_INDEX_CYCLE_NR: int = 10
@@ -26,30 +23,14 @@
 class Index(BaseModel):
     """Class that represents an index."""
 
     name: str
     sequence: str
 
 
-def get_valid_indexes(dual_indexes_only: bool = True) -> list[Index]:
-    """Return a list of valid indexes from the valid indexes file."""
-    LOG.info(f"Fetch valid indexes from {VALID_INDEXES_PATH}")
-    indexes: list[Index] = []
-    indexes_csv: list[list[str]] = ReadFile.get_content_from_file(
-        file_format=FileFormat.CSV, file_path=VALID_INDEXES_PATH
-    )
-    for row in indexes_csv:
-        index_name: str = row[0]
-        index_sequence: str = row[1]
-        if dual_indexes_only and not is_dual_index(index=index_sequence):
-            continue
-        indexes.append(Index(name=index_name, sequence=index_sequence))
-    return indexes
-
-
 def is_padding_needed(index1_cycles: int, index2_cycles: int, sample_index_length: int) -> bool:
     """Returns whether a sample needs padding or not given the sample index length.
     A sample from a NovaSeq6000 flow cell needs padding if its adapted index lengths are shorter
     than the number of index cycles reads stated in the run parameters file for both indexes.
     This happens when the sample index is 8 nucleotides long and the number of index cycles read is
     10 nucleotides long.
     """
```

### Comparing `cg-59.9.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py` & `cg-60.0.0/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-60.0.0/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     """Validate that each sample only exists once per lane in a sample sheet."""
     sample_by_lane: dict[int, list[FlowCellSample]] = get_samples_by_lane(samples)
     for lane, lane_samples in sample_by_lane.items():
         LOG.debug(f"Validate that samples are unique in lane: {lane}")
         validate_samples_are_unique(samples=lane_samples)
 
 
-def get_sample_type_from_content(sample_sheet_content: list[list[str]]) -> Type[FlowCellSample]:
+def get_sample_type_from_content(
+    sample_sheet_content: list[list[str]],
+) -> Type[FlowCellSampleBcl2Fastq | FlowCellSampleBCLConvert]:
     """Returns the sample type identified from the sample sheet content."""
     for row in sample_sheet_content:
         if not row:
             continue
         if SampleSheetBCLConvertSections.Data.HEADER in row[0]:
             LOG.info("Sample sheet was generated for BCL Convert")
             return FlowCellSampleBCLConvert
@@ -91,20 +93,22 @@
         sample_by_lane[sample.lane].append(sample)
     return sample_by_lane
 
 
 def get_flow_cell_samples_from_content(
     sample_sheet_content: list[list[str]],
     sample_type: Type[FlowCellSample] | None = None,
-) -> list[FlowCellSample]:
+) -> list[FlowCellSampleBcl2Fastq | FlowCellSampleBCLConvert]:
     """
     Return the samples in a sample sheet as a list of FlowCellSample objects.
     Raises:
         ValidationError: if the samples do not have the correct attributes based on their model.
     """
     if not sample_type:
-        sample_type: Type[FlowCellSample] = get_sample_type_from_content(sample_sheet_content)
+        sample_type: Type[FlowCellSampleBcl2Fastq | FlowCellSampleBCLConvert] = (
+            get_sample_type_from_content(sample_sheet_content)
+        )
     raw_samples: list[dict[str, str]] = get_raw_samples_from_content(
         sample_sheet_content=sample_sheet_content
     )
     adapter = TypeAdapter(list[sample_type])
     return adapter.validate_python(raw_samples)
```

### Comparing `cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_models.py` & `cg-60.0.0/cg/apps/demultiplex/sample_sheet/sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-60.0.0/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,223 +1,186 @@
-""" Create a sample sheet for NovaSeq flow cells."""
+"""Module with validator classes for the sample sheet."""
 
 import logging
-from abc import abstractmethod
+from pathlib import Path
 from typing import Type
 
-from cg.apps.demultiplex.sample_sheet.index import Index, get_valid_indexes, is_dual_index
-from cg.apps.demultiplex.sample_sheet.read_sample_sheet import get_samples_by_lane
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
-from cg.constants.demultiplexing import (
-    BclConverter,
-    IndexSettings,
-    SampleSheetBcl2FastqSections,
-    SampleSheetBCLConvertSections,
+from pydantic import ValidationError
+
+from cg.apps.demultiplex.sample_sheet.override_cycles_validator import OverrideCyclesValidator
+from cg.apps.demultiplex.sample_sheet.read_sample_sheet import (
+    get_flow_cell_samples_from_content,
+    get_raw_samples_from_content,
+    validate_samples_unique_per_lane,
 )
-from cg.exc import SampleSheetError
-from cg.models.demultiplex.run_parameters import RunParameters
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample, FlowCellSampleBCLConvert
+from cg.apps.demultiplex.sample_sheet.sample_sheet_models import SampleSheet
+from cg.constants.constants import FileFormat
+from cg.constants.demultiplexing import NAME_TO_INDEX_SETTINGS, SampleSheetBCLConvertSections
+from cg.exc import OverrideCyclesError, SampleSheetError
+from cg.io.controller import ReadFile
 
 LOG = logging.getLogger(__name__)
 
 
-class SampleSheetCreator:
-    """Base class for sample sheet creation."""
+class SampleSheetValidator:
+    """Class for validating the content of a sample sheet."""
 
-    def __init__(
-        self,
-        flow_cell: FlowCellDirectoryData,
-        lims_samples: list[FlowCellSampleBCLConvert | FlowCellSampleBcl2Fastq],
-    ):
-        self.flow_cell: FlowCellDirectoryData = flow_cell
-        self.flow_cell_id: str = flow_cell.id
-        self.lims_samples: list[FlowCellSampleBCLConvert | FlowCellSampleBcl2Fastq] = lims_samples
-        self.run_parameters: RunParameters = flow_cell.run_parameters
-        self.sample_type: Type[FlowCellSampleBCLConvert | FlowCellSampleBcl2Fastq] = (
-            flow_cell.sample_type
+    def __init__(self):
+        """Instantiate the class with a sample sheet file path or sample sheet content."""
+        self.content: list[list[str]] | None = None
+        self.read1_cycles: int | None = None
+        self.read2_cycles: int | None = None
+        self.index1_cycles: int | None = None
+        self.index2_cycles: int | None = None
+        self.is_index2_reverse_complement: bool | None = None
+
+    def set_sample_sheet_content(self, content: list[list[str]]) -> None:
+        """Set the sample sheet content."""
+        self.content = content
+
+    def _validate_all_sections_present(self) -> None:
+        """
+        Returns whether the sample sheet has the four mandatory sections:
+            - Header
+            - Reads
+            - BCLConvert Settings
+            - BCLConvert Data
+        Raises:
+            SampleSheetError if the sample sheet does not have all the sections.
+        """
+        LOG.debug("Validating that the sample sheet has all the necessary sections")
+        has_header: bool = [SampleSheetBCLConvertSections.Header.HEADER] in self.content
+        has_cycles: bool = [SampleSheetBCLConvertSections.Reads.HEADER] in self.content
+        has_settings: bool = [SampleSheetBCLConvertSections.Settings.HEADER] in self.content
+        has_data: bool = [SampleSheetBCLConvertSections.Data.HEADER] in self.content
+        if not all([has_header, has_cycles, has_settings, has_data]):
+            message: str = "Sample sheet does not have all the necessary sections"
+            LOG.error(message)
+            raise SampleSheetError(message)
+
+    def _get_index_settings_name(self) -> str:
+        """
+        Find the entry in the sample sheet holding the index settings name, which has the form:
+        `IndexSettings,<index_setting_name>`, and extract its value.
+        """
+
+        for row in self.content:
+            if SampleSheetBCLConvertSections.Header.INDEX_SETTINGS in row:
+                LOG.debug(f"Found index settings: {row[1]}")
+                return row[1]
+        message: str = "No index settings found in sample sheet"
+        LOG.error(message)
+        raise SampleSheetError(message)
+
+    def _set_is_index2_reverse_complement(self) -> None:
+        """Return whether the index2 override cycles value is reverse-complemented."""
+        LOG.debug("Looking for index settings in the sample sheet")
+        settings_name: str = self._get_index_settings_name()
+        self.is_index2_reverse_complement = NAME_TO_INDEX_SETTINGS[
+            settings_name
+        ].are_i5_override_cycles_reverse_complemented
+
+    def _get_cycle(self, cycle_name: str, nullable: bool = False) -> int | None:
+        """
+        Return the cycle from the sample sheet given the cycle name. Set nullable to True to
+        return None if the cycle is not found.
+        Raises:
+            SampleSheetError if the cycle is not found and nullable is False.
+        """
+        for row in self.content:
+            if cycle_name in row:
+                return int(row[1])
+        if not nullable:
+            message: str = f"No {cycle_name} found in sample sheet"
+            LOG.error(message)
+            raise SampleSheetError(message)
+
+    def _set_cycles(self):
+        """Set values to the run cycle attributes."""
+        LOG.debug("Looking for read and index run cycles in the sample sheet")
+        self.read1_cycles = self._get_cycle(SampleSheetBCLConvertSections.Reads.READ_CYCLES_1)
+        self.read2_cycles = self._get_cycle(SampleSheetBCLConvertSections.Reads.READ_CYCLES_2)
+        self.index1_cycles = self._get_cycle(SampleSheetBCLConvertSections.Reads.INDEX_CYCLES_1)
+        self.index2_cycles = self._get_cycle(
+            cycle_name=SampleSheetBCLConvertSections.Reads.INDEX_CYCLES_2, nullable=True
         )
-        self.index_settings: IndexSettings = self.run_parameters.index_settings
 
-    @property
-    def bcl_converter(self) -> str:
-        """Return the bcl converter used for demultiplexing."""
-        return self.flow_cell.bcl_converter
-
-    @property
-    def valid_indexes(self) -> list[Index]:
-        return get_valid_indexes(dual_indexes_only=True)
-
-    @abstractmethod
-    def remove_samples_with_simple_index(self) -> None:
-        """Filter out samples with single indexes."""
-        pass
-
-    def convert_sample_to_header_dict(
-        self,
-        sample: FlowCellSampleBCLConvert | FlowCellSampleBcl2Fastq,
-        data_column_names: list[str],
-    ) -> list[str]:
-        """Convert a lims sample object to a list that corresponds to the sample sheet headers."""
-        if self.run_parameters.is_single_index:
-            sample_serialisation: dict = sample.model_dump(
-                by_alias=True, exclude={"index2", "barcode_mismatches_2"}
+    def _validate_samples(self, sample_type: Type[FlowCellSample] | None = None) -> None:
+        """
+        Determine if the samples have the correct attributes and are unique per lane.
+        Raises:
+            SampleSheetError if the samples do not have the correct attributes based on their model
+            or are not unique per lane.
+        """
+        LOG.debug("Validating samples")
+        try:
+            validated_samples: list[FlowCellSample] = get_flow_cell_samples_from_content(
+                sample_sheet_content=self.content, sample_type=sample_type
             )
-        else:
-            sample_serialisation: dict = sample.model_dump(by_alias=True)
-
-        return [str(sample_serialisation[column_name]) for column_name in data_column_names]
-
-    def get_additional_sections_sample_sheet(self) -> list | None:
-        """Return all sections of the sample sheet that are not the data section."""
-        raise NotImplementedError("Impossible to get sample sheet sections from parent class")
-
-    def get_data_section_header_and_columns(self) -> list[list[str]] | None:
-        """Return the header and column names of the data section of the sample sheet."""
-        raise NotImplementedError("Impossible to get sample sheet sections from parent class")
-
-    def create_sample_sheet_content(self) -> list[list[str]]:
-        """Create sample sheet content with samples."""
-        LOG.info("Creating sample sheet content")
-        complete_data_section: list[list[str]] = self.get_data_section_header_and_columns()
-        sample_sheet_content: list[list[str]] = (
-            self.get_additional_sections_sample_sheet() + complete_data_section
+        except ValidationError as error:
+            LOG.error("Sample sheet failed validation: samples are not in the correct format")
+            raise SampleSheetError from error
+        validate_samples_unique_per_lane(validated_samples)
+
+    def _validate_override_cycles(self) -> None:
+        """Determine if the samples' override cycles are valid.
+        Raises:
+            SampleSheetError if any of the samples' override cycles are not valid.
+        """
+        LOG.debug("Validating override cycles for all samples")
+        validator = OverrideCyclesValidator(
+            run_read1_cycles=self.read1_cycles,
+            run_read2_cycles=self.read2_cycles,
+            run_index1_cycles=self.index1_cycles,
+            run_index2_cycles=self.index2_cycles,
+            is_reverse_complement=self.is_index2_reverse_complement,
         )
-        LOG.debug(f"Use sample sheet header {complete_data_section[1]}")
-        for sample in self.lims_samples:
-            sample_sheet_content.append(
-                self.convert_sample_to_header_dict(
-                    sample=sample,
-                    data_column_names=complete_data_section[1],
-                )
-            )
-        return sample_sheet_content
+        samples: list[dict[str, str]] = get_raw_samples_from_content(self.content)
+        for sample in samples:
+            try:
+                validator.validate_sample(sample)
+            except OverrideCyclesError as error:
+                raise SampleSheetError from error
+
+    def validate_sample_sheet_from_content(self, content: list[list[str]]) -> None:
+        """
+        Determine if the BCLConvert sample sheet is valid, which means:
+        - All sections are present
+        - The index settings are specified in the sample sheet header
+        - The read and index cycles are specified in the sample sheet's reads section
+        - The samples have the correct attributes
+        - The override cycles are valid
+        Raises:
+            SampleSheetError: If the sample sheet is not valid.
+        """
+        self.set_sample_sheet_content(content)
+        LOG.debug("Validating sample sheet")
+        self._validate_all_sections_present()
+        self._set_is_index2_reverse_complement()
+        self._set_cycles()
+        self._validate_samples(sample_type=FlowCellSampleBCLConvert)
+        self._validate_override_cycles()
+        LOG.info("Samplesheet passed validation")
+
+    def validate_sample_sheet_from_file(self, file_path: Path) -> None:
+        """
+        Validate a sample sheet given the path to the file.
+        Raises:
+            SampleSheetError: If the sample sheet is not valid.
+        """
+        content: list[list[str]] = ReadFile.get_content_from_file(
+            file_format=FileFormat.CSV, file_path=file_path
+        )
+        self.validate_sample_sheet_from_content(content)
 
-    def process_samples_for_sample_sheet(self) -> None:
-        """Remove unwanted samples and adapt remaining samples."""
-        self.remove_samples_with_simple_index()
-        for lims_sample in self.lims_samples:
-            lims_sample.process_indexes(run_parameters=self.run_parameters)
-        is_reverse_complement: bool = (
-            self.index_settings.are_i5_override_cycles_reverse_complemented
+    def get_sample_sheet_object_from_file(self, file_path: Path) -> SampleSheet:
+        """Return a sample sheet object given the path to the file.
+        Raises:
+            SampleSheetError: If the sample sheet is not valid.
+        """
+        self.validate_sample_sheet_from_file(file_path)
+        samples: list[FlowCellSample] = get_flow_cell_samples_from_content(
+            sample_sheet_content=self.content,
+            sample_type=FlowCellSampleBCLConvert,
         )
-        for lane, samples_in_lane in get_samples_by_lane(self.lims_samples).items():
-            LOG.info(f"Updating barcode mismatch values for samples in lane {lane}")
-            for lims_sample in samples_in_lane:
-                lims_sample.update_barcode_mismatches(
-                    samples_to_compare=samples_in_lane,
-                    is_run_single_index=self.run_parameters.is_single_index,
-                    is_reverse_complement=is_reverse_complement,
-                )
-
-    def construct_sample_sheet(self) -> list[list[str]]:
-        """Construct and validate the sample sheet."""
-        self.process_samples_for_sample_sheet()
-        sample_sheet_content: list[list[str]] = self.create_sample_sheet_content()
-        return sample_sheet_content
-
-
-class SampleSheetCreatorBcl2Fastq(SampleSheetCreator):
-    """Create a raw sample sheet for flow cells."""
-
-    def remove_samples_with_simple_index(self) -> None:
-        """Filter out samples with single indexes."""
-        LOG.info("Removing all samples without dual indexes")
-        samples_to_keep: list[FlowCellSampleBcl2Fastq] = []
-        for sample in self.lims_samples:
-            if not is_dual_index(sample.index):
-                LOG.warning(f"Removing sample {sample.sample_id} since it does not have dual index")
-                continue
-            samples_to_keep.append(sample)
-        self.lims_samples = samples_to_keep
-
-    def get_additional_sections_sample_sheet(self) -> list[list[str]]:
-        """Return all sections of the sample sheet that are not the data section."""
-        return [
-            [SampleSheetBcl2FastqSections.Settings.HEADER],
-            SampleSheetBcl2FastqSections.Settings.barcode_mismatch_index_1(),
-            SampleSheetBcl2FastqSections.Settings.barcode_mismatch_index_2(),
-        ]
-
-    def get_data_section_header_and_columns(self) -> list[list[str]]:
-        """Return the header and column names of the data section of the sample sheet."""
-        column_names: list[str] = SampleSheetBcl2FastqSections.Data.column_names()
-        if self.run_parameters.is_single_index:
-            column_names.remove(SampleSheetBcl2FastqSections.Data.INDEX_2)
-        return [
-            [SampleSheetBcl2FastqSections.Data.HEADER.value],
-            column_names,
-        ]
-
-
-class SampleSheetCreatorBCLConvert(SampleSheetCreator):
-    """Create a raw sample sheet for BCLConvert flow cells."""
-
-    def __init__(
-        self,
-        flow_cell: FlowCellDirectoryData,
-        lims_samples: list[FlowCellSampleBCLConvert],
-    ):
-        super().__init__(flow_cell, lims_samples)
-        if flow_cell.bcl_converter == BclConverter.BCL2FASTQ:
-            raise SampleSheetError(f"Can't use {BclConverter.BCL2FASTQ} with sample sheet v2")
-
-    def remove_samples_with_simple_index(self) -> None:
-        """Filter out samples with single indexes."""
-        LOG.info("Removing of single index samples is not required for V2 sample sheet")
-
-    def get_additional_sections_sample_sheet(self) -> list[list[str]]:
-        """Return all sections of the sample sheet that are not the data section."""
-        header_section: list[list[str]] = [
-            [SampleSheetBCLConvertSections.Header.HEADER.value],
-            SampleSheetBCLConvertSections.Header.file_format(),
-            [SampleSheetBCLConvertSections.Header.RUN_NAME.value, self.flow_cell_id],
-            [
-                SampleSheetBCLConvertSections.Header.INSTRUMENT_PLATFORM_TITLE.value,
-                SampleSheetBCLConvertSections.Header.instrument_platform_sequencer().get(
-                    self.flow_cell.sequencer_type
-                ),
-            ],
-            SampleSheetBCLConvertSections.Header.index_orientation_forward(),
-            [SampleSheetBCLConvertSections.Header.INDEX_SETTINGS.value, self.index_settings.name],
-        ]
-        reads_section: list[list[str]] = [
-            [SampleSheetBCLConvertSections.Reads.HEADER],
-            [
-                SampleSheetBCLConvertSections.Reads.READ_CYCLES_1,
-                self.run_parameters.get_read_1_cycles(),
-            ],
-            [
-                SampleSheetBCLConvertSections.Reads.READ_CYCLES_2,
-                self.run_parameters.get_read_2_cycles(),
-            ],
-            [
-                SampleSheetBCLConvertSections.Reads.INDEX_CYCLES_1,
-                self.run_parameters.get_index_1_cycles(),
-            ],
-        ]
-        if not self.run_parameters.is_single_index:
-            reads_section.append(
-                [
-                    SampleSheetBCLConvertSections.Reads.INDEX_CYCLES_2,
-                    self.run_parameters.get_index_2_cycles(),
-                ]
-            )
-        settings_section: list[list[str]] = [
-            [SampleSheetBCLConvertSections.Settings.HEADER],
-            SampleSheetBCLConvertSections.Settings.software_version(),
-            SampleSheetBCLConvertSections.Settings.fastq_compression_format(),
-        ]
-        return header_section + reads_section + settings_section
-
-    def get_data_section_header_and_columns(self) -> list[list[str]]:
-        """Return the header and column names of the data section of the sample sheet."""
-        column_names: list[str] = SampleSheetBCLConvertSections.Data.column_names()
-        if self.run_parameters.is_single_index:
-            column_names.remove(SampleSheetBCLConvertSections.Data.BARCODE_MISMATCHES_2)
-            column_names.remove(SampleSheetBCLConvertSections.Data.INDEX_2)
-        return [
-            [SampleSheetBCLConvertSections.Data.HEADER],
-            column_names,
-        ]
+        return SampleSheet(samples=samples)
```

### Comparing `cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py` & `cg-60.0.0/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/demultiplex/sample_sheet/validators.py` & `cg-60.0.0/cg/apps/demultiplex/sample_sheet/validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/downsample/downsample.py` & `cg-60.0.0/cg/apps/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/downsample/utils.py` & `cg-60.0.0/cg/apps/downsample/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/gens.py` & `cg-60.0.0/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/gt.py` & `cg-60.0.0/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/hermes/hermes_api.py` & `cg-60.0.0/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/hermes/models.py` & `cg-60.0.0/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/housekeeper/hk.py` & `cg-60.0.0/cg/apps/housekeeper/hk.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             if path.is_absolute():
                 file = self.files(path=str(path).replace(f"{self.root_dir}/", "")).first()
             else:
                 file = self.files(path=f"{self.root_dir}/{path}").first()
         return file
 
     @staticmethod
-    def get_files_from_version(version: Version, tags: set[str]) -> list[File] | None:
+    def get_files_from_version(version: Version, tags: set[str]) -> list[File]:
         """Return a list of files associated with the given version and tags."""
         LOG.debug(f"Getting files from version with tags {tags}")
         files: list[File] = []
         for file in list(version.files):
             file_tags = {tag.name for tag in file.tags}
             if tags.issubset(file_tags):
                 LOG.debug(f"Found file {file}")
@@ -160,15 +160,15 @@
             LOG.warning(f"Could not find any files matching the tags {tags}")
         return files
 
     @staticmethod
     def get_file_from_version(version: Version, tags: set[str]) -> File | None:
         """Return the first file matching the given tags."""
         files: list[File] = HousekeeperAPI.get_files_from_version(version=version, tags=tags)
-        return files[0] if files else None
+        return next((file for file in files), None)
 
     @staticmethod
     def get_latest_file_from_version(version: Version, tags: set[str]) -> File | None:
         """Return the latest file from Housekeeper given its version and tags."""
         files: list[File] = HousekeeperAPI.get_files_from_version(version=version, tags=tags)
         return sorted(files, key=lambda file_obj: file_obj.id)[-1] if files else None
 
@@ -385,25 +385,27 @@
         """Return a file in the latest version of a bundle."""
         version: Version = self.last_version(bundle=bundle_name)
         if not version:
             LOG.warning(f"Bundle: {bundle_name} not found in Housekeeper")
             raise HousekeeperBundleVersionMissingError
         return self.files(version=version.id, tags=tags).first()
 
-    def get_files_from_latest_version(self, bundle_name: str, tags: list[str]) -> Query:
+    def get_files_from_latest_version(
+        self, bundle_name: str, tags: list[str] | None = None
+    ) -> list[File] | None:
         """Return files in the latest version of a bundle.
 
         Raises HousekeeperBundleVersionMissingError:
         - When no version was found for the given bundle
         """
         version: Version = self.last_version(bundle=bundle_name)
         if not version:
             LOG.warning(f"Bundle: {bundle_name} not found in Housekeeper")
             raise HousekeeperBundleVersionMissingError
-        return self.files(version=version.id, tags=tags)
+        return self.files(version=version.id, tags=tags).all()
 
     def is_fastq_or_spring_in_all_bundles(self, bundle_names: list[str]) -> bool:
         """Return whether all FASTQ/SPRING files are included for the given bundles."""
         sequencing_files_in_hk: dict[str, bool] = {}
         if not bundle_names:
             return False
         for bundle_name in bundle_names:
@@ -511,15 +513,15 @@
         self.commit()
 
     def get_sample_sheets_from_latest_version(self, flow_cell_id: str) -> list[File]:
         """Returns the files tagged with 'samplesheet' for the given bundle."""
         try:
             sample_sheet_files: list[File] = self.get_files_from_latest_version(
                 bundle_name=flow_cell_id, tags=[flow_cell_id, SequencingFileTag.SAMPLE_SHEET]
-            ).all()
+            )
         except HousekeeperBundleVersionMissingError:
             sample_sheet_files = []
         return sample_sheet_files
 
     def get_sample_sheet_path(self, flow_cell_id: str) -> Path:
         """Returns the sample sheet path for the flow cell."""
         sample_sheet_files: list[File] = self.get_sample_sheets_from_latest_version(flow_cell_id)
@@ -658,7 +660,42 @@
     def reset_retrieved_archive_data(self, files_to_reset: list[File]):
         """Resets 'retrieval_task_id' and 'retrieved_at' for all files' corresponding archive entries"""
         for file in files_to_reset:
             LOG.debug(f"Resetting retrieval data for file {file.path}")
             file.archive.retrieval_task_id = None
             file.archive.retrieved_at = None
         self.commit()
+
+    @staticmethod
+    def get_files_containing_tags(files: list[File], tags: list[set[str]]) -> list[File]:
+        """Return files containing specified tags."""
+        filtered_files: list[File] = []
+        for file in files:
+            file_tags: set[str] = {tag.name for tag in file.tags}
+            if any(tag.issubset(file_tags) for tag in tags):
+                filtered_files.append(file)
+        return filtered_files
+
+    @staticmethod
+    def get_files_without_excluded_tags(files: list[File], excluded_tags: list[str]) -> list[File]:
+        """Return files without specified tags."""
+        filtered_files: list[File] = []
+        for file in files:
+            file_tags: list[str] = [tag.name for tag in file.tags]
+            if not any(excluded_tag in file_tags for excluded_tag in excluded_tags):
+                filtered_files.append(file)
+        return filtered_files
+
+    def get_files_from_latest_version_containing_tags(
+        self, bundle_name: str, tags: list[set[str]], excluded_tags: list[str] | None = None
+    ) -> list[File]:
+        """
+        Return files from the latest version of a bundle matching provided tags. Files containing
+        any tag sets specified in the excluded_tags list will be excluded from the output.
+        """
+        files: list[File] = self.get_files_from_latest_version(bundle_name=bundle_name)
+        filtered_files: list[File] = self.get_files_containing_tags(files=files, tags=tags)
+        if excluded_tags:
+            filtered_files: list[File] = self.get_files_without_excluded_tags(
+                files=filtered_files, excluded_tags=excluded_tags
+            )
+        return filtered_files
```

### Comparing `cg-59.9.1/cg/apps/invoice/render.py` & `cg-60.0.0/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-60.0.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-60.0.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-60.0.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-60.0.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/lims/api.py` & `cg-60.0.0/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/lims/batch.py` & `cg-60.0.0/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/lims/order.py` & `cg-60.0.0/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/lims/sample_sheet.py` & `cg-60.0.0/cg/apps/lims/sample_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import re
 from typing import Iterable, Type
 
 from genologics.entities import Artifact, Container, Sample
 from genologics.lims import Lims
 
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBCLConvert
 
 LOG = logging.getLogger(__name__)
 
 
 def get_placement_lane(lane: str) -> int:
     """Parse out the lane information from an artifact.placement."""
     return int(lane.split(":")[0])
@@ -65,16 +65,16 @@
 
     return sequence
 
 
 def get_flow_cell_samples(
     lims: Lims,
     flow_cell_id: str,
-    flow_cell_sample_type: Type[FlowCellSample],
-) -> Iterable[FlowCellSample]:
+    flow_cell_sample_type: Type[FlowCellSampleBCLConvert],
+) -> Iterable[FlowCellSampleBCLConvert]:
     """Return samples from LIMS for a given flow cell."""
     LOG.info(f"Fetching samples from lims for flowcell {flow_cell_id}")
     containers: list[Container] = lims.get_containers(name=flow_cell_id)
     if not containers:
         return []
     container: Container = containers[-1]  # only take the last one. See ÖA#217.
     raw_lanes: list[str] = sorted(container.placements.keys())
```

### Comparing `cg-59.9.1/cg/apps/loqus.py` & `cg-60.0.0/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/madeline/api.py` & `cg-60.0.0/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/mip/confighandler.py` & `cg-60.0.0/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/mutacc_auto.py` & `cg-60.0.0/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/orderform/excel_orderform_parser.py` & `cg-60.0.0/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/orderform/json_orderform_parser.py` & `cg-60.0.0/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/orderform/orderform_parser.py` & `cg-60.0.0/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/osticket.py` & `cg-60.0.0/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/scout/scout_export.py` & `cg-60.0.0/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/scout/scoutapi.py` & `cg-60.0.0/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/sequencing_metrics_parser/api.py` & `cg-60.0.0/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py` & `cg-60.0.0/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/sequencing_metrics_parser/models/bcl_convert.py` & `cg-60.0.0/cg/apps/sequencing_metrics_parser/models/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py` & `cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py` & `cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py` & `cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py` & `cg-60.0.0/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py` & `cg-60.0.0/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/slurm/sbatch.py` & `cg-60.0.0/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/slurm/slurm_api.py` & `cg-60.0.0/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/apps/tb/api.py` & `cg-60.0.0/cg/apps/tb/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 from typing import Any
 
 from google.auth import jwt
 from google.auth.crypt import RSASigner
 
 from cg.apps.tb.dto.create_job_request import CreateJobRequest
-from cg.apps.tb.dto.summary_response import SummariesResponse, AnalysisSummary
+from cg.apps.tb.dto.summary_response import AnalysisSummary, SummariesResponse
 from cg.apps.tb.models import AnalysesResponse, TrailblazerAnalysis
 from cg.constants import Workflow
 from cg.constants.constants import APIMethods, FileFormat, JobType, WorkflowManager
 from cg.constants.priority import SlurmQos
 from cg.constants.tb import AnalysisStatus
 from cg.exc import TrailblazerAnalysisNotFound, TrailblazerAPIHTTPError
 from cg.io.controller import APIRequest, ReadStream
@@ -174,7 +174,16 @@
 
     def get_summaries(self, order_ids: list[int]) -> list[AnalysisSummary]:
         orders_param = "orderIds=" + ",".join(map(str, order_ids))
         endpoint = f"summary?{orders_param}"
         response = self.query_trailblazer(command=endpoint, request_body={}, method=APIMethods.GET)
         response_data = SummariesResponse.model_validate(response)
         return response_data.summaries
+
+    def get_analyses_to_deliver(self, order_id: int) -> list[TrailblazerAnalysis]:
+        """Return the analyses in the order which have a 'Completed' status."""
+        endpoint = f"analyses?orderId={order_id}&status[]={AnalysisStatus.COMPLETED}"
+        raw_response = self.query_trailblazer(
+            command=endpoint, request_body={}, method=APIMethods.GET
+        )
+        validated_response = AnalysesResponse.model_validate(raw_response)
+        return validated_response.analyses
```

### Comparing `cg-59.9.1/cg/apps/tb/models.py` & `cg-60.0.0/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/add.py` & `cg-60.0.0/cg/cli/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from cg.store.models import (
     Application,
     ApplicationVersion,
     Case,
     CaseSample,
     Collaboration,
     Customer,
+    Order,
     Panel,
     Sample,
     User,
 )
 from cg.store.store import Store
 from cg.utils.click.EnumChoice import EnumChoice
 
@@ -165,47 +166,52 @@
 @click.option(
     "-p",
     "--priority",
     type=EnumChoice(Priority, use_value=False),
     default="standard",
     help="Set the priority for the samples",
 )
+@click.option(
+    "-t", "--original-ticket", required=True, help="Original ticket this sample is associated to."
+)
 @click.argument("customer_id")
 @click.argument("name")
 @click.pass_obj
 def add_sample(
     context: CGConfig,
     lims_id: str | None,
     down_sampled: int | None,
     sex: Sex,
     order: str | None,
     application_tag: str,
     priority: Priority,
     customer_id: str,
     name: str,
+    original_ticket: str,
 ):
     """Add a sample for CUSTOMER_ID with a NAME (display)."""
     status_db: Store = context.status_db
 
     customer: Customer = status_db.get_customer_by_internal_id(customer_internal_id=customer_id)
     if not customer:
         LOG.error(f"Customer: {customer_id} not found")
         raise click.Abort
     application: Application = status_db.get_application_by_tag(tag=application_tag)
     if not application:
         LOG.error(f"Application: {application_tag} not found")
-
         raise click.Abort
+
     new_record: Sample = status_db.add_sample(
         name=name,
         sex=sex,
         downsampled_to=down_sampled,
         internal_id=lims_id,
         order=order,
         priority=priority,
+        original_ticket=original_ticket,
     )
     new_record.application_version: ApplicationVersion = (
         status_db.get_current_application_version_by_tag(tag=application_tag)
     )
     new_record.customer: Customer = customer
     status_db.session.add(new_record)
     status_db.session.commit()
@@ -269,14 +275,24 @@
         data_analysis=data_analysis,
         data_delivery=data_delivery,
         name=name,
         panels=list(panel_abbreviations),
         priority=priority,
         ticket=ticket,
     )
+    order: Order = status_db.get_order_by_ticket_id(int(ticket))
+    if not order:
+        LOG.warning(f"No order found with ticket_id {ticket}")
+        click.confirm("No order found for the given ticket, proceed?", default=False, abort=True)
+        order = Order(
+            customer_id=customer.id,
+            ticket_id=int(ticket),
+            workflow=data_analysis,
+        )
+    new_case.orders.append(order)
 
     new_case.customer: Customer = customer
     status_db.session.add(new_case)
     status_db.session.commit()
     LOG.info(f"{new_case.internal_id}: new case added")
```

### Comparing `cg-59.9.1/cg/cli/archive.py` & `cg-60.0.0/cg/cli/archive.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/backup.py` & `cg-60.0.0/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/base.py` & `cg-60.0.0/cg/cli/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from cg.cli.delete.base import delete
 from cg.cli.deliver.base import deliver as deliver_cmd
 from cg.cli.demultiplex.base import demultiplex_cmd_group as demultiplex_cmd
 from cg.cli.downsample import downsample
 from cg.cli.generate.base import generate as generate_cmd
 from cg.cli.get import get
 from cg.cli.set.base import set_cmd
-from cg.cli.store.store import store as store_cmd
+from cg.cli.store.base import store as store_cmd
 from cg.cli.transfer import transfer_group
 from cg.cli.upload.base import upload
 from cg.cli.workflow.base import workflow as workflow_cmd
 from cg.constants.constants import FileFormat
 from cg.io.controller import ReadFile
 from cg.models.cg_config import CGConfig
 from cg.store.database import (
```

### Comparing `cg-59.9.1/cg/cli/clean.py` & `cg-60.0.0/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/compress/base.py` & `cg-60.0.0/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/compress/fastq.py` & `cg-60.0.0/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/compress/helpers.py` & `cg-60.0.0/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/delete/base.py` & `cg-60.0.0/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/delete/case.py` & `cg-60.0.0/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/delete/cases.py` & `cg-60.0.0/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/delete/observations.py` & `cg-60.0.0/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/deliver/base.py` & `cg-60.0.0/cg/cli/deliver/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 import click
 
 from cg.apps.tb import TrailblazerAPI
 from cg.constants.delivery import PIPELINE_ANALYSIS_OPTIONS, PIPELINE_ANALYSIS_TAG_MAP
 from cg.meta.deliver import DeliverAPI
-from cg.meta.deliver_ticket import DeliverTicketAPI
+from cg.meta.deliver import DeliverTicketAPI
 from cg.meta.rsync.rsync_api import RsyncAPI
 from cg.models.cg_config import CGConfig
 from cg.services.fastq_file_service.fastq_file_service import FastqFileService
 from cg.store.models import Case
 from cg.store.store import Store
 
 LOG = logging.getLogger(__name__)
@@ -137,15 +137,15 @@
 @click.pass_context
 def concatenate(context: click.Context, ticket: str, dry_run: bool):
     """The fastq files in the folder generated using "cg deliver analysis"
     will be concatenated into one forward and one reverse fastq file
     """
     cg_context: CGConfig = context.obj
     deliver_ticket_api = DeliverTicketAPI(config=cg_context)
-    deliver_ticket_api.concatenate(ticket=ticket, dry_run=dry_run)
+    deliver_ticket_api.concatenate_fastq_files(ticket=ticket, dry_run=dry_run)
 
 
 @deliver.command(name="ticket")
 @DELIVERY_TYPE
 @DRY_RUN
 @FORCE_ALL
 @IGNORE_MISSING_BUNDLES
@@ -181,14 +181,10 @@
             force_all=force_all,
             ticket=ticket,
             ignore_missing_bundles=ignore_missing_bundles,
         )
     else:
         LOG.info("Files already delivered to customer inbox on the HPC")
         return
-    is_concatenation_needed: bool = deliver_ticket_api.check_if_concatenation_is_needed(
-        ticket=ticket
-    )
-    if is_concatenation_needed and "fastq" in delivery_type:
-        context.invoke(concatenate, ticket=ticket, dry_run=dry_run)
+
     deliver_ticket_api.report_missing_samples(ticket=ticket, dry_run=dry_run)
     context.invoke(rsync, ticket=ticket, dry_run=dry_run)
```

### Comparing `cg-59.9.1/cg/cli/demultiplex/base.py` & `cg-60.0.0/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py` & `cg-60.0.0/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/demultiplex/demux.py` & `cg-60.0.0/cg/cli/demultiplex/demux.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from cg.apps.tb import TrailblazerAPI
 from cg.cli.demultiplex.copy_novaseqx_demultiplex_data import (
     hardlink_flow_cell_analysis_data,
     is_ready_for_post_processing,
     mark_as_demultiplexed,
     mark_flow_cell_as_queued_for_post_processing,
 )
-from cg.constants.demultiplexing import OPTION_BCL_CONVERTER, DemultiplexingDirsAndFiles
+from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.exc import FlowCellError, SampleSheetError
 from cg.meta.demultiplex.utils import (
     create_manifest_file,
     is_flow_cell_sync_confirmed,
     is_manifest_file_required,
     is_syncing_complete,
 )
@@ -57,15 +57,15 @@
             continue
 
         if not demultiplex_api.is_demultiplexing_possible(flow_cell=flow_cell):
             LOG.warning(f"Can not start demultiplexing for flow cell {flow_cell.id}!")
             continue
 
         try:
-            sample_sheet_api.validate_sample_sheet(sample_sheet_path=flow_cell.sample_sheet_path)
+            sample_sheet_api.validate_sample_sheet(flow_cell.sample_sheet_path)
         except (SampleSheetError, ValidationError):
             LOG.warning(
                 f"Malformed sample sheet. Run cg demultiplex samplesheet validate {flow_cell.sample_sheet_path}"
             )
             continue
 
         if not dry_run:
@@ -76,50 +76,44 @@
                 tb_api=tb_api, slurm_job_id=slurm_job_id, flow_cell=flow_cell
             )
 
 
 @click.command(name="flow-cell")
 @click.argument("flow-cell-name")
 @DRY_RUN
-@OPTION_BCL_CONVERTER
 @click.pass_obj
 def demultiplex_flow_cell(
     context: CGConfig,
     dry_run: bool,
     flow_cell_name: str,
-    bcl_converter: str,
 ):
-    """Demultiplex a flow cell.
+    """Demultiplex a flow cell using BCLConvert.
 
     flow cell name is the flow cell run directory name, e.g. '201203_D00483_0200_AHVKJCDRXX'
     """
 
-    LOG.info(f"Running cg demultiplex flow cell, using {bcl_converter}")
+    LOG.info(f"Starting demultiplexing of flow cell {flow_cell_name}")
     sample_sheet_api: SampleSheetAPI = context.sample_sheet_api
     demultiplex_api: DemultiplexingAPI = context.demultiplex_api
     flow_cell_directory: Path = Path(context.demultiplex_api.flow_cells_dir, flow_cell_name)
     demultiplex_api.set_dry_run(dry_run=dry_run)
     LOG.info(f"setting flow cell id to {flow_cell_name}")
     LOG.info(f"setting demultiplexed runs dir to {demultiplex_api.demultiplexed_runs_dir}")
 
     try:
-        flow_cell = FlowCellDirectoryData(
-            flow_cell_path=flow_cell_directory, bcl_converter=bcl_converter
-        )
+        flow_cell = FlowCellDirectoryData(flow_cell_directory)
     except FlowCellError as error:
         raise click.Abort from error
 
     if not demultiplex_api.is_demultiplexing_possible(flow_cell=flow_cell):
         LOG.warning("Can not start demultiplexing!")
         return
 
     try:
-        sample_sheet_api.validate_sample_sheet(
-            sample_sheet_path=flow_cell.sample_sheet_path, bcl_converter=bcl_converter
-        )
+        sample_sheet_api.validate_sample_sheet(flow_cell.sample_sheet_path)
     except (SampleSheetError, ValidationError) as error:
         LOG.warning(
             f"Malformed sample sheet. Run cg demultiplex samplesheet validate {flow_cell.sample_sheet_path}"
         )
         raise click.Abort from error
 
     if not dry_run:
```

### Comparing `cg-59.9.1/cg/cli/demultiplex/sample_sheet.py` & `cg-60.0.0/cg/cli/demultiplex/sample_sheet.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from pathlib import Path
 
 import click
 from pydantic import ValidationError
 
 from cg.apps.demultiplex.sample_sheet.api import SampleSheetAPI
 from cg.constants.constants import DRY_RUN
-from cg.constants.demultiplexing import OPTION_BCL_CONVERTER
 from cg.exc import SampleSheetError
 from cg.models.cg_config import CGConfig
 
 LOG = logging.getLogger(__name__)
 
 
 @click.group(name="samplesheet")
@@ -19,52 +18,64 @@
 
 
 @sample_sheet_commands.command(name="validate")
 @click.argument("sheet", type=click.Path(exists=True, dir_okay=False))
 @click.pass_obj
 def validate_sample_sheet(context: CGConfig, sheet: click.Path):
     """
-    Validate a sample sheet. The bcl converter would be determined from the sample sheet content.
+    Validate a sample sheet.
     """
     LOG.info(f"Validating {sheet} sample sheet")
     sample_sheet_api: SampleSheetAPI = context.sample_sheet_api
     try:
         sample_sheet_api.validate_sample_sheet(Path(sheet))
     except (SampleSheetError, ValidationError) as error:
         LOG.error("Sample sheet failed validation")
         raise click.Abort from error
     LOG.info("Sample sheet passed validation")
 
 
+@sample_sheet_commands.command(name="translate")
+@click.argument("flow-cell-name")
+@DRY_RUN
+@click.pass_obj
+def translate_sample_sheet(context: CGConfig, flow_cell_name: str, dry_run: bool):
+    """
+    Translate a sample sheet from Bcl2Fastq to BclConvert format.
+    'flow-cell-name' is the flow cell run directory name, e.g. '181005_D00410_0735_BHM2LNBCX2' with
+    a Bcl2Fastq sample sheet in it.
+    """
+    LOG.info(f"Translating Bcl2Fastq sample sheet for flow cell {flow_cell_name}")
+    sample_sheet_api: SampleSheetAPI = context.sample_sheet_api
+    sample_sheet_api.set_dry_run(dry_run)
+    sample_sheet_api.translate_sample_sheet(flow_cell_name=flow_cell_name)
+
+
 @sample_sheet_commands.command(name="create")
 @click.argument("flow-cell-name")
-@OPTION_BCL_CONVERTER
 @DRY_RUN
 @click.option("--force", is_flag=True, help="Skips the validation of the sample sheet")
 @click.pass_obj
 def create_sheet(
     context: CGConfig,
     flow_cell_name: str,
-    bcl_converter: str | None,
     dry_run: bool,
     force: bool = False,
 ):
     """Create a sample sheet or hard-link it from Housekeeper in the flow cell directory.
 
-    flow-cell-name is the flow cell run directory name, e.g. '201203_D00483_0200_AHVKJCDRXX'
+    'flow-cell-name' is the flow cell run directory name, e.g. '181005_D00410_0735_BHM2LNBCX2'
 
     Search the flow cell in the directory specified in config.
     """
     LOG.info(f"Getting a valid sample sheet for flow cell {flow_cell_name}")
     sample_sheet_api: SampleSheetAPI = context.sample_sheet_api
     sample_sheet_api.set_dry_run(dry_run)
     sample_sheet_api.set_force(force)
-    sample_sheet_api.get_or_create_sample_sheet(
-        flow_cell_name=flow_cell_name, bcl_converter=bcl_converter
-    )
+    sample_sheet_api.get_or_create_sample_sheet(flow_cell_name)
 
 
 @sample_sheet_commands.command(name="create-all")
 @DRY_RUN
 @click.pass_obj
 def create_all_sheets(context: CGConfig, dry_run: bool):
     """Command to create sample sheets for all flow cells that lack a sample sheet.
```

### Comparing `cg-59.9.1/cg/cli/downsample.py` & `cg-60.0.0/cg/cli/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/generate/report/base.py` & `cg-60.0.0/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/generate/report/options.py` & `cg-60.0.0/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/generate/report/utils.py` & `cg-60.0.0/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/get.py` & `cg-60.0.0/cg/cli/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             "Yes" if existing_sample.application_version.application.is_external else "No",
         ]
         click.echo(tabulate([row], headers=SAMPLE_HEADERS, tablefmt="psql"))
         if cases:
             case_ids: list[str] = [link_obj.case.internal_id for link_obj in existing_sample.links]
             context.invoke(get_case, case_ids=case_ids, samples=False)
         if not hide_flow_cell:
-            for sample_flow_cell in existing_sample.flowcells:
+            for sample_flow_cell in existing_sample.flow_cells:
                 LOG.debug(f"Get info on flow cell: {sample_flow_cell.name}")
                 context.invoke(get_flow_cell, flow_cell_id=sample_flow_cell.name, samples=False)
 
 
 @get.command("analysis")
 @click.argument("case-id")
 @click.pass_obj
```

### Comparing `cg-59.9.1/cg/cli/set/base.py` & `cg-60.0.0/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/set/case.py` & `cg-60.0.0/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/set/cases.py` & `cg-60.0.0/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/store/fastq.py` & `cg-60.0.0/cg/cli/store/store.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 from typing import Iterable
 
 import click
 from housekeeper.store.models import File
 
 from cg.apps.crunchy.files import update_metadata_paths
 from cg.cli.compress.helpers import update_compress_api
+from cg.clients.arnold.exceptions import ArnoldClientError, ArnoldServerError
+from cg.clients.janus.exceptions import JanusClientError, JanusServerError
 from cg.constants import SequencingFileTag
 from cg.constants.constants import DRY_RUN
 from cg.exc import CaseNotFoundError
 from cg.meta.compress import CompressAPI
+from cg.meta.qc_metrics.collect_qc_metrics import CollectQCMetricsAPI
 from cg.models.cg_config import CGConfig
 from cg.store.models import Sample
 from cg.store.store import Store
 
 LOG = logging.getLogger(__name__)
 
 
@@ -126,7 +129,25 @@
                 LOG.info(
                     f"Updating file paths in SPRING metadata file {spring_metadata_file.full_path}: for sample: {sample.internal_id}"
                 )
                 update_metadata_paths(
                     spring_metadata_path=spring_metadata_file.full_path,
                     new_parent_path=Path(spring_metadata_file.full_path).parent,
                 )
+
+
+@click.command("qc-metrics")
+@click.argument("case-id", type=str)
+@DRY_RUN
+@click.pass_obj
+def store_qc_metrics(config: CGConfig, case_id: str, dry_run: bool = False) -> None:
+    """Fetch the QC metrics for a case from Janus and Store them in Arnold."""
+    metrics_api = CollectQCMetricsAPI(
+        hk_api=config.housekeeper_api,
+        status_db=config.status_db,
+        janus_api=config.janus_api,
+        arnold_api=config.arnold_api,
+    )
+    try:
+        metrics_api.create_case(case_id=case_id, dry_run=dry_run)
+    except (JanusClientError, JanusServerError, ArnoldClientError, ArnoldServerError):
+        return
```

### Comparing `cg-59.9.1/cg/cli/store/store.py` & `cg-60.0.0/cg/cli/store/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 import click
 
 from cg.apps.crunchy.crunchy import CrunchyAPI
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.meta.compress.compress import CompressAPI
 from cg.models.cg_config import CGConfig
 
-from .fastq import (
+from .store import (
     store_case,
     store_demultiplexed_flow_cell,
     store_flow_cell,
+    store_qc_metrics,
     store_sample,
     store_ticket,
 )
 
 LOG = logging.getLogger(__name__)
 
 
@@ -38,9 +39,10 @@
 
 for sub_cmd in [
     store_case,
     store_demultiplexed_flow_cell,
     store_flow_cell,
     store_sample,
     store_ticket,
+    store_qc_metrics,
 ]:
     store.add_command(sub_cmd)
```

### Comparing `cg-59.9.1/cg/cli/transfer.py` & `cg-60.0.0/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/base.py` & `cg-60.0.0/cg/cli/upload/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from cg.cli.upload.validate import validate
 from cg.constants import Workflow
 from cg.exc import AnalysisAlreadyUploadedError
 from cg.meta.upload.balsamic.balsamic import BalsamicUploadAPI
 from cg.meta.upload.microsalt.microsalt_upload_api import MicrosaltUploadAPI
 from cg.meta.upload.mip.mip_dna import MipDNAUploadAPI
 from cg.meta.upload.mip.mip_rna import MipRNAUploadAPI
-from cg.meta.upload.rnafusion.rnafusion import RnafusionUploadAPI
+from cg.meta.upload.nf_analysis import NfAnalysisUploadAPI
 from cg.meta.upload.upload_api import UploadAPI
 from cg.models.cg_config import CGConfig
 from cg.store.models import Case
 from cg.store.store import Store
 from cg.utils.click.EnumChoice import EnumChoice
 
 LOG = logging.getLogger(__name__)
@@ -73,20 +73,20 @@
             upload_api.verify_analysis_upload(case_obj=case, restart=restart)
         except AnalysisAlreadyUploadedError:
             # Analysis being uploaded or it has been already uploaded
             return
 
         if Workflow.BALSAMIC in case.data_analysis:
             upload_api = BalsamicUploadAPI(config_object)
-        elif case.data_analysis == Workflow.RNAFUSION:
-            upload_api = RnafusionUploadAPI(config_object)
         elif case.data_analysis == Workflow.MIP_RNA:
             upload_api = MipRNAUploadAPI(config_object)
         elif case.data_analysis == Workflow.MICROSALT:
             upload_api = MicrosaltUploadAPI(config_object)
+        elif case.data_analysis in {Workflow.RNAFUSION, Workflow.TOMTE, Workflow.TAXPROFILER}:
+            upload_api = NfAnalysisUploadAPI(config_object, case.data_analysis)
 
         context.obj.meta_apis["upload_api"] = upload_api
         upload_api.upload(ctx=context, case=case, restart=restart)
         click.echo(click.style(f"{case_id} analysis has been successfully uploaded", fg="green"))
     else:
         suggest_cases_to_upload(status_db=upload_api.status_db)
         raise click.Abort()
```

### Comparing `cg-59.9.1/cg/cli/upload/clinical_delivery.py` & `cg-60.0.0/cg/cli/upload/clinical_delivery.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from cg.apps.tb.models import TrailblazerAnalysis
 from cg.constants import EXIT_FAIL, EXIT_SUCCESS, Priority, Workflow
 from cg.constants.constants import DRY_RUN
 from cg.constants.delivery import PIPELINE_ANALYSIS_TAG_MAP
 from cg.constants.tb import AnalysisTypes
 from cg.meta.deliver import DeliverAPI
 from cg.meta.rsync import RsyncAPI
+from cg.services.analysis_service.analysis_service import AnalysisService
 from cg.services.fastq_file_service.fastq_file_service import FastqFileService
 from cg.store.models import Case
 from cg.store.store import Store
 
 LOG = logging.getLogger(__name__)
 
 
@@ -60,15 +61,17 @@
     is_complete_delivery, job_id = rsync_api.slurm_rsync_single_case(
         case=case,
         dry_run=dry_run,
         sample_files_present=is_sample_delivery,
         case_files_present=is_case_delivery,
     )
     RsyncAPI.write_trailblazer_config(
-        {"jobs": [str(job_id)]}, config_path=rsync_api.trailblazer_config_path
+        content={"jobs": [str(job_id)]},
+        config_path=rsync_api.trailblazer_config_path,
+        dry_run=dry_run,
     )
     analysis_name: str = f"{case_id}_rsync" if is_complete_delivery else f"{case_id}_partial"
     order_id: int = case.latest_order.id
     if not dry_run:
         trailblazer_api: TrailblazerAPI = context.obj.trailblazer_api
         analysis: TrailblazerAnalysis = trailblazer_api.add_pending_analysis(
             case_id=analysis_name,
@@ -77,14 +80,18 @@
             order_id=order_id,
             out_dir=rsync_api.log_dir.as_posix(),
             slurm_quality_of_service=Priority.priority_to_slurm_qos().get(case.priority),
             workflow=Workflow.RSYNC,
             ticket=case.latest_ticket,
         )
         trailblazer_api.add_upload_job_to_analysis(analysis_id=analysis.id, slurm_id=job_id)
+
+        analysis_service: AnalysisService = context.obj.analysis_service
+        analysis_service.add_upload_job(slurm_id=job_id, case_id=case_id)
+
     LOG.info(f"Transfer of case {case_id} started with SLURM job id {job_id}")
 
 
 @click.command("all-fastq")
 @click.pass_context
 @DRY_RUN
 def auto_fastq(context: click.Context, dry_run: bool):
```

### Comparing `cg-59.9.1/cg/cli/upload/coverage.py` & `cg-60.0.0/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/delivery_report.py` & `cg-60.0.0/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/fohm.py` & `cg-60.0.0/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/genotype.py` & `cg-60.0.0/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/gens.py` & `cg-60.0.0/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/gisaid.py` & `cg-60.0.0/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/mutacc.py` & `cg-60.0.0/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/nipt/base.py` & `cg-60.0.0/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/nipt/ftp.py` & `cg-60.0.0/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/nipt/statina.py` & `cg-60.0.0/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/observations/observations.py` & `cg-60.0.0/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/observations/utils.py` & `cg-60.0.0/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/scout.py` & `cg-60.0.0/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/utils.py` & `cg-60.0.0/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/upload/validate.py` & `cg-60.0.0/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/balsamic/base.py` & `cg-60.0.0/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/balsamic/options.py` & `cg-60.0.0/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/balsamic/pon.py` & `cg-60.0.0/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/balsamic/qc.py` & `cg-60.0.0/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/balsamic/umi.py` & `cg-60.0.0/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/base.py` & `cg-60.0.0/cg/cli/workflow/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from cg.cli.workflow.microsalt.base import microsalt
 from cg.cli.workflow.mip_dna.base import mip_dna
 from cg.cli.workflow.mip_rna.base import mip_rna
 from cg.cli.workflow.mutant.base import mutant
 from cg.cli.workflow.raredisease.base import raredisease
 from cg.cli.workflow.rnafusion.base import rnafusion
 from cg.cli.workflow.taxprofiler.base import taxprofiler
+from cg.cli.workflow.tomte.base import tomte
 
 
 @click.group()
 def workflow():
     """Workflows commands"""
 
 
@@ -27,11 +28,12 @@
 workflow.add_command(balsamic_umi)
 workflow.add_command(balsamic_pon)
 workflow.add_command(microsalt)
 workflow.add_command(mip_dna)
 workflow.add_command(mip_rna)
 workflow.add_command(fluffy)
 workflow.add_command(mutant)
-workflow.add_command(rnafusion)
 workflow.add_command(raredisease)
+workflow.add_command(rnafusion)
 workflow.add_command(taxprofiler)
+workflow.add_command(tomte)
 workflow.add_command(fastq)
```

### Comparing `cg-59.9.1/cg/cli/workflow/commands.py` & `cg-60.0.0/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/fastq/base.py` & `cg-60.0.0/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/fastq/fastq_service.py` & `cg-60.0.0/cg/cli/workflow/fastq/fastq_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/fluffy/base.py` & `cg-60.0.0/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/microsalt/base.py` & `cg-60.0.0/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/mip/base.py` & `cg-60.0.0/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/mip/options.py` & `cg-60.0.0/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/mip_dna/base.py` & `cg-60.0.0/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/mip_rna/base.py` & `cg-60.0.0/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/mutant/base.py` & `cg-60.0.0/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/cli/workflow/raredisease/base.py` & `cg-60.0.0/cg/cli/workflow/raredisease/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """CLI support to create config and/or start RAREDISEASE."""
 
 import logging
 
 import click
 
 from cg.cli.utils import echo_lines
-from cg.cli.workflow.commands import ARGUMENT_CASE_ID, OPTION_DRY
+from cg.cli.workflow.commands import ARGUMENT_CASE_ID, OPTION_DRY, resolve_compression
+from cg.cli.workflow.nf_analysis import config_case, run, start, start_available
 from cg.constants.constants import MetaApis
 from cg.meta.workflow.analysis import AnalysisAPI
 from cg.meta.workflow.raredisease import RarediseaseAnalysisAPI
 from cg.models.cg_config import CGConfig
 
 LOG = logging.getLogger(__name__)
 
@@ -18,14 +19,21 @@
 @click.pass_context
 def raredisease(context: click.Context) -> None:
     """NF-core/raredisease analysis workflow."""
     AnalysisAPI.get_help(context)
     context.obj.meta_apis[MetaApis.ANALYSIS_API] = RarediseaseAnalysisAPI(config=context.obj)
 
 
+raredisease.add_command(resolve_compression)
+raredisease.add_command(config_case)
+raredisease.add_command(run)
+raredisease.add_command(start)
+raredisease.add_command(start_available)
+
+
 @raredisease.command("panel")
 @OPTION_DRY
 @ARGUMENT_CASE_ID
 @click.pass_obj
 def panel(context: CGConfig, case_id: str, dry_run: bool) -> None:
     """Write aggregated gene panel file exported from Scout."""
```

### Comparing `cg-59.9.1/cg/clients/janus/api.py` & `cg-60.0.0/cg/clients/janus/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """The JanusAPIClient."""
 
+import logging
 from http import HTTPStatus
 
 import requests
 from requests import Response
 
 from cg.clients.janus.dto.create_qc_metrics_request import CreateQCMetricsRequest
 from cg.clients.janus.exceptions import JanusClientError, JanusServerError
 
+LOG = logging.getLogger(__name__)
+
 
 class JanusAPIClient:
     def __init__(self, config: dict[str]):
         self.host = config["janus"]["host"]
 
     def qc_metrics(self, collect_qc_request: CreateQCMetricsRequest) -> dict | None:
-        endpoint: str = f"{self.host}/collect_qc_metrics"
+        endpoint: str = f"{self.host}/collect_qc"
         post_request_data: str = collect_qc_request.model_dump_json()
-        response = requests.post(endpoint, data=post_request_data)
+        response = requests.post(endpoint, data=post_request_data, verify=True)
         if response.status_code == HTTPStatus.OK:
             return response.json()
         self._handle_errors(response)
 
     @staticmethod
     def _handle_errors(response: Response):
-        if 400 <= response.status_code < 500:
-            raise JanusClientError(f"Client error: {response.status_code}")
-        elif 500 <= response.status_code:
-            raise JanusServerError(f"Server error: {response.status_code}")
+        if HTTPStatus.BAD_REQUEST <= response.status_code < HTTPStatus.INTERNAL_SERVER_ERROR:
+            LOG.error(f"Client error: {response.content}")
+            raise JanusClientError
+        elif HTTPStatus.INTERNAL_SERVER_ERROR <= response.status_code:
+            LOG.error(f"Server error: {response.content}")
+            raise JanusServerError
```

### Comparing `cg-59.9.1/cg/constants/__init__.py` & `cg-60.0.0/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/constants/bcl_convert_metrics.py` & `cg-60.0.0/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/constants/constants.py` & `cg-60.0.0/cg/constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Constants for cg."""
 
-from enum import StrEnum
+from enum import IntEnum, StrEnum
 
 import click
 
 from cg.utils.date import get_date
 
 VALID_DATA_IN_PRODUCTION = get_date("2017-09-27")
 
@@ -132,14 +132,15 @@
     MIP_RNA: str = "mip-rna"
     MUTANT: str = "mutant"
     RAREDISEASE: str = "raredisease"
     RNAFUSION: str = "rnafusion"
     RSYNC: str = "rsync"
     SPRING: str = "spring"
     TAXPROFILER: str = "taxprofiler"
+    TOMTE: str = "tomte"
 
 
 class FileFormat(StrEnum):
     FASTQ: str = "fastq"
     JSON: str = "json"
     YAML: str = "yaml"
     CSV: str = "csv"
@@ -177,19 +178,22 @@
 class HastaSlurmPartitions(StrEnum):
     DRAGEN: str = "dragen"
 
 
 class FileExtensions(StrEnum):
     BED: str = ".bed"
     COMPLETE: str = ".complete"
+    CONFIG: str = ".config"
     CRAM: str = ".cram"
     CSV: str = ".csv"
     FASTQ: str = ".fastq"
+    FASTQ_GZ: str = ".fastq.gz"
     GPG: str = ".gpg"
     GZIP: str = ".gz"
+    HTML: str = ".html"
     JSON: str = ".json"
     KEY: str = ".key"
     LOG: str = ".log"
     MD5SUM: str = ".md5sum"
     NO_EXTENSION: str = ""
     PASS_PHRASE: str = ".passphrase"
     PENDING: str = ".pending"
@@ -239,14 +243,15 @@
     TARGET_READS: int = 6000000
     TARGET_READS_FAIL_THRESHOLD: float = 0.7
 
 
 class MicrosaltAppTags(StrEnum):
     MWRNXTR003: str = "MWRNXTR003"
     MWXNXTR003: str = "MWXNXTR003"
+    VWGNXTR001: str = "VWGNXTR001"
     PREP_CATEGORY: str = "mic"
 
 
 DRY_RUN_MESSAGE = "Dry run: process call will not be executed!"
 
 
 class MetaApis:
@@ -262,14 +267,21 @@
     """Strandedness types."""
 
     FORWARD: str = "forward"
     REVERSE: str = "reverse"
     UNSTRANDED: str = "unstranded"
 
 
+class ReadDirection(IntEnum):
+    """Read direction types."""
+
+    FORWARD: int = 1
+    REVERSE: int = 2
+
+
 PIPELINES_USING_PARTIAL_ANALYSES: list[Workflow] = [Workflow.MICROSALT, Workflow.MUTANT]
 
 
 class MultiQC(StrEnum):
     """MultiQC constants"""
 
     MULTIQC: str = "multiqc"
```

### Comparing `cg-59.9.1/cg/constants/delivery.py` & `cg-60.0.0/cg/constants/delivery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Constants for delivery."""
 
 from cg.constants.constants import Workflow
 from cg.constants.housekeeper_tags import (
     HK_DELIVERY_REPORT_TAG,
     AlignmentFileTag,
     AnalysisTag,
+    HermesFileTag,
 )
 
 ONLY_ONE_CASE_PER_TICKET: list[Workflow] = [
     Workflow.FASTQ,
     Workflow.MICROSALT,
     Workflow.MUTANT,
 ]
@@ -164,14 +165,17 @@
 ]
 
 RNAFUSION_ANALYSIS_SAMPLE_TAGS: list[set[str]] = [
     {AlignmentFileTag.CRAM},
     {AlignmentFileTag.CRAM_INDEX},
 ]
 
+NF_ANALYSIS_CASE_TAGS: list[set[str]] = [{HermesFileTag.CLINICAL_DELIVERY}]
+
+NF_ANALYSIS_SAMPLE_TAGS: list[set[str]] = [{HermesFileTag.CLINICAL_DELIVERY}]
 
 PIPELINE_ANALYSIS_TAG_MAP: dict[Workflow, dict] = {
     Workflow.BALSAMIC: {
         "case_tags": BALSAMIC_ANALYSIS_CASE_TAGS,
         "sample_tags": BALSAMIC_ANALYSIS_SAMPLE_TAGS,
     },
     Workflow.BALSAMIC_QC: {
@@ -202,13 +206,21 @@
         "case_tags": MUTANT_ANALYSIS_CASE_TAGS,
         "sample_tags": MUTANT_ANALYSIS_SAMPLE_TAGS,
     },
     Workflow.RNAFUSION: {
         "case_tags": RNAFUSION_ANALYSIS_CASE_TAGS,
         "sample_tags": RNAFUSION_ANALYSIS_SAMPLE_TAGS,
     },
+    Workflow.TAXPROFILER: {
+        "case_tags": NF_ANALYSIS_CASE_TAGS,
+        "sample_tags": NF_ANALYSIS_CASE_TAGS,
+    },
+    Workflow.TOMTE: {
+        "case_tags": NF_ANALYSIS_CASE_TAGS,
+        "sample_tags": NF_ANALYSIS_CASE_TAGS,
+    },
 }
 
 PIPELINE_ANALYSIS_OPTIONS = PIPELINE_ANALYSIS_TAG_MAP.keys()
 
 INBOX_NAME: str = "inbox"
 OUTBOX_NAME: str = "outbox"
```

### Comparing `cg-59.9.1/cg/constants/demultiplexing.py` & `cg-60.0.0/cg/constants/demultiplexing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Constants related to demultiplexing."""
 
 from enum import StrEnum
 from pathlib import Path
 
-import click
 from pydantic import BaseModel
 
 from cg.constants.sequencing import Sequencers
 
 
 class BclConverter(StrEnum):
     """Define the BCL converter."""
@@ -26,15 +25,14 @@
     HISEQ_X_COPY_COMPLETE: str = "copycomplete.txt"
     HISEQ_X_TILE_DIR: str = "l1t11"
     RTACOMPLETE: str = "RTAComplete.txt"
     RUN_PARAMETERS_PASCAL_CASE: str = "RunParameters.xml"
     RUN_PARAMETERS_CAMEL_CASE: str = "runParameters.xml"
     SAMPLE_SHEET_FILE_NAME: str = "SampleSheet.csv"
     UNALIGNED_DIR_NAME: str = "Unaligned"
-    BCL2FASTQ_TILE_DIR_PATTERN: str = r"l\dt\d{2}"
     QUEUED_FOR_POST_PROCESSING: str = "post_processing_queued.txt"
     ANALYSIS_COMPLETED: str = "Secondary_Analysis_Complete.txt"
     ANALYSIS: str = "Analysis"
     DATA: str = "Data"
     BCL_CONVERT: str = "BCLConvert"
     FLOW_CELLS_DIRECTORY_NAME: str = "flow_cells"
     DEMULTIPLEXED_RUNS_DIRECTORY_NAME: str = "demultiplexed_runs"
@@ -77,25 +75,14 @@
     NOVASEQ_X_INSTRUMENT: str = "NovaSeqXPlus"
     UNKNOWN_REAGENT_KIT_VERSION: str = "unknown"
 
 
 class SampleSheetBcl2FastqSections:
     """Class with all necessary constants for building a NovaSeqX sample sheet."""
 
-    class Settings(StrEnum):
-        HEADER: str = "[Settings]"
-
-        @classmethod
-        def barcode_mismatch_index_1(cls) -> list[str]:
-            return ["BarcodeMismatchesIndex1", "0"]
-
-        @classmethod
-        def barcode_mismatch_index_2(cls) -> list[str]:
-            return ["BarcodeMismatchesIndex2", "0"]
-
     class Data(StrEnum):
         HEADER: str = "[Data]"
         FLOW_CELL_ID: str = "FCID"
         LANE: str = "Lane"
         SAMPLE_INTERNAL_ID_BCL2FASTQ: str = "SampleID"
         SAMPLE_REFERENCE: str = "SampleRef"
         INDEX_1: str = "index"
@@ -197,24 +184,14 @@
     FULL_8_INDEX: str = "I8;"
     IGNORED_10_INDEX: str = "N10;"
     IGNORED_8_INDEX: str = "N8;"
     INDEX_8_IGNORED_2: str = "I8N2;"
     INDEX_8_IGNORED_2_REVERSED: str = "N2I8;"
 
 
-OPTION_BCL_CONVERTER = click.option(
-    "-b",
-    "--bcl-converter",
-    type=click.Choice([BclConverter.BCL2FASTQ, BclConverter.BCLCONVERT]),
-    default=None,
-    help="Specify bcl conversion software. Choose between bcl2fastq and dragen. "
-    "If not specified, the software will be determined automatically using the sequencer type.",
-)
-
-
 DEMUX_STATS_PATH: dict[str, dict[str, Path | None]] = {
     BclConverter.BCL2FASTQ: {
         "demultiplexing_stats": Path("Stats", "DemultiplexingStats.xml"),
         "conversion_stats": Path("Stats", "ConversionStats.xml"),
         "runinfo": None,
     },
     BclConverter.BCLCONVERT: {
```

### Comparing `cg-59.9.1/cg/constants/encryption.py` & `cg-60.0.0/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/constants/gene_panel.py` & `cg-60.0.0/cg/constants/gene_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             CustomerId.CUST004,
             CustomerId.CUST042,
         }
 
 
 class GenePanelCombo:
     COMBO_1: dict[str, set[str]] = {
-        "DSD": {"DSD", "DSD-S", "HYP", "SEXDIF", "SEXDET"},
+        "DSD": {"DSD", "DSD-S", "HYP", "SEXDIF", "SEXDET", "POI"},
         "CM": {"CNM", "CM"},
         "Horsel": {"Horsel", "141217", "141201"},
         "OPHTHALMO": {
             "OPHTHALMO",
             "ANTE-ED",
             "CATARACT",
             "CORNEA",
```

### Comparing `cg-59.9.1/cg/constants/housekeeper_tags.py` & `cg-60.0.0/cg/constants/housekeeper_tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,21 @@
 HK_MULTIQC_HTML_TAG = ["multiqc-html"]
 
 HK_FASTQ_TAGS = [SequencingFileTag.FASTQ]
 
 HK_DELIVERY_REPORT_TAG = "delivery-report"
 
 
+class HermesFileTag(StrEnum):
+    """Tags for hermes."""
+
+    CLINICAL_DELIVERY: str = "clinical-delivery"
+    LONG_TERM_STORAGE: str = "long-term-storage"
+
+
 class AnalysisTag(StrEnum):
     """Tags for analysis files."""
 
     ARRIBA: str = "arriba"
     ARRIBA_VISUALIZATION: str = "arriba-visualisation"
     FUSION: str = "fusion"
     FUSIONCATCHER: str = "fusioncatcher"
@@ -203,14 +210,20 @@
         [AnalysisTag.FUSIONINSPECTOR_HTML, AnalysisTag.RESEARCH],
         [AnalysisTag.ARRIBA_VISUALIZATION, AnalysisTag.RESEARCH],
         [AnalysisTag.MULTIQC_HTML, AnalysisTag.RNA],
         [HK_DELIVERY_REPORT_TAG],
         [AnalysisTag.VCF_FUSION],
         [AnalysisTag.GENE_COUNTS],
     ],
+    Workflow.TAXPROFILER: [
+        [HermesFileTag.LONG_TERM_STORAGE],
+    ],
+    Workflow.TOMTE: [
+        [HermesFileTag.LONG_TERM_STORAGE],
+    ],
 }
 
 
 class JanusTags:
     """Tags to communicate with the JanusAPI."""
 
     tags_to_retrieve: list[str] = ["qc-metrics", "janus"]
```

### Comparing `cg-59.9.1/cg/constants/lims.py` & `cg-60.0.0/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/constants/nextflow.py` & `cg-60.0.0/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/constants/observations.py` & `cg-60.0.0/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/constants/orderforms.py` & `cg-60.0.0/cg/constants/orderforms.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     @staticmethod
     def get_current_orderform_version(order_form: str) -> str:
         """Returns the current version of the given order form."""
         current_order_form_versions = {
             Orderform.MIP_DNA: "30",
             Orderform.RML: "17",
             Orderform.MICROSALT: "11",
-            Orderform.SARS_COV_2: "8",
+            Orderform.SARS_COV_2: "9",
         }
         return current_order_form_versions[order_form]
```

### Comparing `cg-59.9.1/cg/constants/priority.py` & `cg-60.0.0/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/constants/report.py` & `cg-60.0.0/cg/constants/report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Delivery report constants."""
 
 from cg.constants import DataDelivery
 from cg.constants.constants import Workflow
 
 BALSAMIC_REPORT_ACCREDITED_PANELS: list[str] = ["gmsmyeloid"]
 
+RNAFUSION_REPORT_ACCREDITED_APPTAGS: list[str] = ["RNAPOAR100"]
+RNAFUSION_REPORT_MINIMUM_INPUT_AMOUNT: int = 300
+
 REPORT_SUPPORTED_WORKFLOW: tuple[Workflow, ...] = (
     Workflow.BALSAMIC,
     Workflow.BALSAMIC_UMI,
     Workflow.BALSAMIC_QC,
     Workflow.MIP_DNA,
     Workflow.RNAFUSION,
 )
```

### Comparing `cg-59.9.1/cg/constants/scout.py` & `cg-60.0.0/cg/constants/scout.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/constants/sequencing.py` & `cg-60.0.0/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/constants/subject.py` & `cg-60.0.0/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/exc.py` & `cg-60.0.0/cg/exc.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,14 +122,20 @@
 
 class HousekeeperArchiveMissingError(CgError):
     """
     Exception raised when an archive is missing in Housekeeper.
     """
 
 
+class HousekeeperStoreError(CgError):
+    """
+    Exception raised when a deliverable file is malformed in Housekeeper.
+    """
+
+
 class LimsDataError(CgError):
     """
     Error related to missing/incomplete data in LIMS.
     """
 
 
 class MicrosaltError(CgError):
@@ -140,14 +146,20 @@
 
 class MissingAnalysisRunDirectory(CgError):
     """
     Error related to missing analysis.
     """
 
 
+class NfAnalysisError(CgError):
+    """
+    Error related to nf analysis.
+    """
+
+
 class OrderError(CgError):
     """
     Exception related to orders.
     """
 
 
 class OrderFormError(CgError):
@@ -262,9 +274,21 @@
     """Exception raised when an order is not found."""
 
 
 class OrderExistsError(CgError):
     """Exception raised when cases and samples are added to a pre-existing order."""
 
 
+class OrderMismatchError(CgError):
+    """Exception raised when cases expected to belong to the same order are not part of the same order."""
+
+
+class OrderNotDeliverableError(CgError):
+    """Exception raised when no analysis is ready for delivery for an order."""
+
+
+class DeliveryMessageNotSupportedError(CgError):
+    """Exception raised when trying to fetch delivery messages for unsupported workflows."""
+
+
 class OverrideCyclesError(CgError):
     """Exception raised when the override cycles are not correct."""
```

### Comparing `cg-59.9.1/cg/io/api.py` & `cg-60.0.0/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/io/controller.py` & `cg-60.0.0/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/io/csv.py` & `cg-60.0.0/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/io/json.py` & `cg-60.0.0/cg/io/json.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from pathlib import Path
 from typing import Any
+from cg.constants.symbols import EMPTY_STRING
 
 
 def read_json(file_path: Path) -> Any:
     """Read content in a json file"""
     with open(file_path, "r") as file:
         return json.load(file)
```

### Comparing `cg-59.9.1/cg/io/validate_path.py` & `cg-60.0.0/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/io/xml.py` & `cg-60.0.0/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/io/yaml.py` & `cg-60.0.0/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/archive/archive.py` & `cg-60.0.0/cg/meta/archive/archive.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/archive/ddn/constants.py` & `cg-60.0.0/cg/meta/archive/ddn/constants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/archive/ddn/ddn_data_flow_client.py` & `cg-60.0.0/cg/meta/archive/ddn/ddn_data_flow_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
     def _get_job_status(self, headers: dict, job_id: int) -> GetJobStatusResponse:
         """Gets the job status for the provided job_id."""
         LOG.info(f"Sending GET request for job {job_id}")
 
         url: str = urljoin(self.url, DataflowEndpoints.GET_JOB_STATUS + str(job_id))
         response: Response = APIRequest.api_request_from_content(
-            api_method=APIMethods.POST,
+            api_method=APIMethods.GET,
             url=url,
             headers=headers,
             json={},
             verify=False,
         )
         response.raise_for_status()
         return GetJobStatusResponse.model_validate(response.json())
```

### Comparing `cg-59.9.1/cg/meta/archive/ddn/models.py` & `cg-60.0.0/cg/meta/archive/ddn/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/archive/ddn/utils.py` & `cg-60.0.0/cg/meta/archive/ddn/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/archive/models.py` & `cg-60.0.0/cg/meta/archive/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/backup/backup.py` & `cg-60.0.0/cg/meta/backup/backup.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,30 +95,31 @@
 
     def _process_flow_cell(
         self, flow_cell: Flowcell, archived_key: Path, archived_flow_cell: Path
     ) -> float:
         """Process a flow cell from backup. Return elapsed time."""
         start_time: float = get_start_time()
         run_dir: Path = Path(self.flow_cells_dir)
+        flow_cell_output_directory: Path = Path(run_dir, archived_flow_cell.name.split(".")[0])
         self.retrieve_archived_key(archived_key=archived_key, flow_cell=flow_cell, run_dir=run_dir)
         self.retrieve_archived_flow_cell(
             archived_flow_cell=archived_flow_cell, flow_cell=flow_cell, run_dir=run_dir
         )
 
         try:
             (
                 decrypted_flow_cell,
                 encryption_key,
                 retrieved_flow_cell,
                 retrieved_key,
             ) = self.decrypt_flow_cell(archived_flow_cell, archived_key, run_dir)
 
             self.extract_flow_cell(decrypted_flow_cell, run_dir)
-            self.create_rta_complete(decrypted_flow_cell, run_dir)
-            self.create_copy_complete(decrypted_flow_cell, run_dir)
+            self.create_rta_complete(flow_cell_output_directory)
+            self.create_copy_complete(flow_cell_output_directory)
             self.unlink_files(
                 decrypted_flow_cell, encryption_key, retrieved_flow_cell, retrieved_key
             )
         except subprocess.CalledProcessError as error:
             LOG.error(f"Decryption failed: {error.stderr}")
             if not self.dry_run:
                 flow_cell.status: str = FlowCellStatus.REQUESTED
@@ -153,28 +154,22 @@
             LOG.info(message)
         try:
             encryption_key.unlink()
         except FileNotFoundError:
             LOG.info(message)
 
     @staticmethod
-    def create_rta_complete(decrypted_flow_cell: Path, run_dir: Path):
+    def create_rta_complete(flow_cell_directory: Path):
         """Create an RTAComplete.txt file in the flow cell run directory."""
-        rta_complete_file = Path(
-            run_dir, decrypted_flow_cell.stem, DemultiplexingDirsAndFiles.RTACOMPLETE
-        )
-        rta_complete_file.touch()
+        Path(flow_cell_directory, DemultiplexingDirsAndFiles.RTACOMPLETE).touch()
 
     @staticmethod
-    def create_copy_complete(decrypted_flow_cell: Path, run_dir: Path):
+    def create_copy_complete(flow_cell_directory: Path):
         """Create a CopyComplete.txt file in the flow cell run directory."""
-        copy_complete_file = Path(
-            run_dir, decrypted_flow_cell.stem, DemultiplexingDirsAndFiles.COPY_COMPLETE
-        )
-        copy_complete_file.touch()
+        Path(flow_cell_directory, DemultiplexingDirsAndFiles.COPY_COMPLETE).touch()
 
     def extract_flow_cell(self, decrypted_flow_cell, run_dir):
         """Extract the flow cell tar archive."""
         extraction_command = self.tar_api.get_extract_file_command(
             input_file=decrypted_flow_cell, output_dir=run_dir
         )
         LOG.debug(f"Extract flow cell command: {extraction_command}")
```

### Comparing `cg-59.9.1/cg/meta/backup/pdc.py` & `cg-60.0.0/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/clean/api.py` & `cg-60.0.0/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/clean/clean_flow_cells.py` & `cg-60.0.0/cg/meta/clean/clean_flow_cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         bundle_names: list[str] = [sample.internal_id for sample in flow_cell.samples]
         files: list[File] = []
         for bundle_name in bundle_names:
             try:
                 files.extend(
                     self.hk_api.get_files_from_latest_version(
                         bundle_name=bundle_name, tags=[tag, self.flow_cell.id]
-                    ).all()
+                    )
                 )
             except HousekeeperBundleVersionMissingError:
                 continue
         if not files:
             LOG.warning(f"No files with tag {tag} found on flow cell {self.flow_cell.id}")
             return None
         return files
```

### Comparing `cg-59.9.1/cg/meta/clean/clean_retrieved_spring_files.py` & `cg-60.0.0/cg/meta/clean/clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/compress/compress.py` & `cg-60.0.0/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/compress/files.py` & `cg-60.0.0/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/deliver.py` & `cg-60.0.0/cg/meta/deliver/deliver.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from housekeeper.store.models import File, Version
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import delivery as constants
 from cg.constants.constants import DataDelivery, Workflow
 from cg.exc import MissingFilesError
 from cg.services.fastq_file_service.fastq_file_service import FastqFileService
+from cg.meta.deliver.fastq_path_generator import (
+    generate_forward_concatenated_fastq_delivery_path,
+    generate_reverse_concatenated_fastq_delivery_path,
+)
 from cg.store.models import Case, CaseSample, Sample
 from cg.store.store import Store
 
 LOG = logging.getLogger(__name__)
 
 
 class DeliverAPI:
@@ -211,25 +215,30 @@
             raise MissingFilesError(f"No files were linked for sample {sample_name}")
 
         LOG.info(
             f"There were {number_previously_linked_files} previously linked files and {number_linked_files_now} were linked for sample {sample_id}, case {case_id}"
         )
 
         if self.delivery_type == Workflow.FASTQ and case.data_analysis == Workflow.MICROSALT:
+            LOG.debug(f"Concatenating fastqs for sample {sample_name}")
             self.concatenate_fastqs(sample_directory=delivery_base, sample_name=sample_name)
 
     def concatenate_fastqs(self, sample_directory: Path, sample_name: str):
         if self.dry_run:
             return
-        forward_out_path = Path(sample_directory, f"{sample_name}_R1.fastq.gz")
-        reverse_out_path = Path(sample_directory, f"{sample_name}_R2.fastq.gz")
+        forward_output_path: Path = generate_forward_concatenated_fastq_delivery_path(
+            fastq_directory=sample_directory, sample_name=sample_name
+        )
+        reverse_output_path: Path = generate_reverse_concatenated_fastq_delivery_path(
+            fastq_directory=sample_directory, sample_name=sample_name
+        )
         self.fastq_file_service.concatenate(
             fastq_directory=sample_directory,
-            forward_output=forward_out_path,
-            reverse_output=reverse_out_path,
+            forward_output_path=forward_output_path,
+            reverse_output_path=reverse_output_path,
             remove_raw=True,
         )
 
     def get_case_files_from_version(self, version: Version, sample_ids: set[str]) -> Iterable[Path]:
         """Fetch all case files from a version that are tagged with any of the case tags."""
 
         if not version:
```

### Comparing `cg-59.9.1/cg/meta/demultiplex/combine_sequencing_metrics.py` & `cg-60.0.0/cg/meta/demultiplex/combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/demultiplex/demux_post_processing.py` & `cg-60.0.0/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/demultiplex/files.py` & `cg-60.0.0/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/demultiplex/housekeeper_storage_functions.py` & `cg-60.0.0/cg/meta/demultiplex/housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/demultiplex/status_db_storage_functions.py` & `cg-60.0.0/cg/meta/demultiplex/status_db_storage_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,40 +35,19 @@
             sequencer_name=parsed_flow_cell.machine_name,
             sequenced_at=parsed_flow_cell.run_date,
         )
         LOG.info(f"Flow cell added to status db: {parsed_flow_cell.id}.")
     else:
         LOG.info(f"Flow cell already exists in status db: {parsed_flow_cell.id}.")
         flow_cell.status = FlowCellStatus.ON_DISK
-
-    sample_internal_ids: list[str] = parsed_flow_cell.sample_sheet.get_sample_ids()
-    add_samples_to_flow_cell_in_status_db(
-        flow_cell=flow_cell,
-        sample_internal_ids=sample_internal_ids,
-        store=store,
-    )
     LOG.info(f"Added samples to flow cell: {parsed_flow_cell.id}.")
     store.session.add(flow_cell)
     store.session.commit()
 
 
-def add_samples_to_flow_cell_in_status_db(
-    flow_cell: Flowcell, sample_internal_ids: list[str], store: Store
-) -> Flowcell:
-    """Adds samples to a flow cell in status db."""
-    samples: set[Sample] = {
-        store.get_sample_by_internal_id(sample_internal_id)
-        for sample_internal_id in sample_internal_ids
-    }
-    for sample in samples:
-        if isinstance(sample, Sample) and sample not in flow_cell.samples:
-            flow_cell.samples.append(sample)
-    return flow_cell
-
-
 def store_sequencing_metrics_in_status_db(flow_cell: FlowCellDirectoryData, store: Store) -> None:
     mapped_metrics: list[SampleLaneSequencingMetrics] = (
         create_sample_lane_sequencing_metrics_for_flow_cell(
             flow_cell_directory=flow_cell.path,
             bcl_converter=flow_cell.bcl_converter,
         )
     )
```

### Comparing `cg-59.9.1/cg/meta/demultiplex/utils.py` & `cg-60.0.0/cg/meta/demultiplex/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/demultiplex/validation.py` & `cg-60.0.0/cg/meta/demultiplex/validation.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/encryption/encryption.py` & `cg-60.0.0/cg/meta/encryption/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,18 @@
         self.slurm_api.set_dry_run(dry_run=self.dry_run)
 
     @property
     def flow_cell_encryption_dir(self) -> Path:
         return Path(self.encryption_dir, self.flow_cell.full_name)
 
     @property
+    def flow_cell_encrypt_tmp_dir(self) -> Path:
+        return Path(self.flow_cell_encryption_dir, "tmp")
+
+    @property
     def flow_cell_encrypt_file_path_prefix(self) -> Path:
         return Path(self.flow_cell_encryption_dir, self.flow_cell.id)
 
     @property
     def pending_file_path(self) -> Path:
         return Path(self.flow_cell_encrypt_file_path_prefix.with_suffix(FileExtensions.PENDING))
 
@@ -254,29 +258,42 @@
             )
         if self.pending_file_path.exists():
             raise FlowCellEncryptionError(
                 f"Encryption already started for flow cell: {self.flow_cell.id}"
             )
         return True
 
+    def make_tmp_encrypt_dir(self) -> str:
+        return f"mkdir -p {self.flow_cell_encrypt_tmp_dir}"
+
+    def copy_flow_cell_dir_to_tmp(self) -> str:
+        return f"cp -r {self.flow_cell.path} {self.flow_cell_encrypt_tmp_dir}"
+
+    def remove_tmp_encrypt_dir(self) -> str:
+        return f"rm -rf {self.flow_cell_encrypt_tmp_dir}"
+
     def encrypt_flow_cell(
         self,
     ) -> None:
         """Encrypt flow cell via GPG and SLURM."""
         error_function: str = FLOW_CELL_ENCRYPT_ERROR.format(
             pending_file_path=self.pending_file_path
         )
         commands: str = FLOW_CELL_ENCRYPT_COMMANDS.format(
             symmetric_passphrase=self.get_symmetric_passphrase_cmd(
                 passphrase_file_path=self.symmetric_passphrase_file_path
             ),
             asymmetrically_encrypt_passphrase=self.get_asymmetrically_encrypt_passphrase_cmd(
                 passphrase_file_path=self.symmetric_passphrase_file_path
             ),
-            tar_encrypt_flow_cell_dir=self.tar_api.get_compress_cmd(input_path=self.flow_cell.path),
+            make_tmp_encrypt_dir=self.make_tmp_encrypt_dir(),
+            copy_flow_cell_dir_to_tmp=self.copy_flow_cell_dir_to_tmp(),
+            tar_encrypt_tmp_dir=self.tar_api.get_compress_cmd(
+                input_path=self.flow_cell_encrypt_tmp_dir
+            ),
             parallel_gzip=f"{self.pigz_binary_path} -p {self.slurm_number_tasks - LIMIT_PIGZ_TASK} --fast -c",
             tee=f"tee >(md5sum > {self.encrypted_md5sum_file_path})",
             flow_cell_symmetric_encryption=self.get_flow_cell_symmetric_encryption_command(
                 output_file=self.encrypted_gpg_file_path,
                 passphrase_file_path=self.symmetric_passphrase_file_path,
             ),
             flow_cell_symmetric_decryption=self.get_flow_cell_symmetric_decryption_command(
@@ -284,14 +301,15 @@
                 passphrase_file_path=self.symmetric_passphrase_file_path,
             ),
             md5sum=f"md5sum > {self.decrypted_md5sum_file_path}",
             diff=f"diff -q {self.encrypted_md5sum_file_path} {self.decrypted_md5sum_file_path}",
             mv_passphrase_file=f"mv {self.symmetric_passphrase_file_path.with_suffix(FileExtensions.GPG)} {self.final_passphrase_file_path}",
             remove_pending_file=f"rm -f {self.pending_file_path}",
             flag_as_complete=f"touch {self.complete_file_path}",
+            remove_tmp_encrypt_dir=self.remove_tmp_encrypt_dir(),
         )
         sbatch_parameters = Sbatch(
             account=self.slurm_account,
             commands=commands,
             email=self.slurm_mail_user,
             error=error_function,
             hours=self.slurm_hours,
```

### Comparing `cg-59.9.1/cg/meta/invoice.py` & `cg-60.0.0/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/meta.py` & `cg-60.0.0/cg/meta/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from cg.apps.madeline.api import MadelineAPI
 from cg.apps.mutacc_auto import MutaccAutoAPI
 from cg.apps.scout.scoutapi import ScoutAPI
 from cg.apps.tb import TrailblazerAPI
 from cg.meta.backup.backup import SpringBackupAPI
 from cg.meta.backup.pdc import PdcAPI
 from cg.meta.compress import CompressAPI
+from cg.meta.delivery.delivery import DeliveryAPI
 from cg.meta.encryption.encryption import SpringEncryptionAPI
 from cg.meta.workflow.prepare_fastq import PrepareFastqAPI
 from cg.models.cg_config import CGConfig
 from cg.store.store import Store
 
 
 class MetaAPI:
@@ -44,7 +45,8 @@
                     pdc_api=PdcAPI(config.dict()["pdc"]["binary_path"]),
                 ),
             ),
         )
         self.status_db: Store = config.status_db
         self.scout_api: ScoutAPI = config.scout_api
         self.trailblazer_api: TrailblazerAPI = config.trailblazer_api
+        self.delivery_api: DeliveryAPI = config.delivery_api
```

### Comparing `cg-59.9.1/cg/meta/observations/balsamic_observations_api.py` & `cg-60.0.0/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/observations/mip_dna_observations_api.py` & `cg-60.0.0/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/observations/observations_api.py` & `cg-60.0.0/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/api.py` & `cg-60.0.0/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/case_submitter.py` & `cg-60.0.0/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/fastq_submitter.py` & `cg-60.0.0/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/lims.py` & `cg-60.0.0/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/metagenome_submitter.py` & `cg-60.0.0/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/microbial_submitter.py` & `cg-60.0.0/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/pool_submitter.py` & `cg-60.0.0/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/rnafusion_submitter.py` & `cg-60.0.0/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/sars_cov_2_submitter.py` & `cg-60.0.0/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/submitter.py` & `cg-60.0.0/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/orders/ticket_handler.py` & `cg-60.0.0/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/qc_metrics/collect_qc_metrics.py` & `cg-60.0.0/cg/meta/qc_metrics/collect_qc_metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import logging
 from typing import Iterator
 
 from housekeeper.store.models import File, Tag
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.clients.arnold.api import ArnoldAPIClient
+from cg.clients.arnold.dto.create_case_request import CreateCaseRequest
 from cg.clients.janus.api import JanusAPIClient
 from cg.clients.janus.dto.create_qc_metrics_request import (
     CreateQCMetricsRequest,
     FilePathAndTag,
     WorkflowInfo,
 )
-from cg.clients.janus.exceptions import JanusClientError, JanusServerError
 from cg.constants.housekeeper_tags import JanusTags
 from cg.exc import HousekeeperFileMissingError
 from cg.store.models import Case
 from cg.store.store import Store
 
 LOG = logging.getLogger(__name__)
 
@@ -79,15 +79,25 @@
         return CreateQCMetricsRequest(
             case_id=case_id,
             sample_ids=sample_ids,
             workflow_info=workflow_info,
             files=file_paths_and_tags,
         )
 
-    def get_qc_metrics(self, case_id) -> dict:
+    def get_case_qc_metrics(self, case_id: str) -> dict:
         """Get the qc metrics for a case."""
         qc_metrics_request: CreateQCMetricsRequest = self.create_qc_metrics_request(case_id)
-        try:
-            qc_metrics: dict = self.janus_api.qc_metrics(qc_metrics_request)
-            return qc_metrics
-        except (JanusClientError, JanusServerError) as error:
-            LOG.info(f"Cannot collect qc metrics from Janus: {error}")
+        qc_metrics: dict = self.janus_api.qc_metrics(qc_metrics_request)
+        return qc_metrics
+
+    def get_create_case_request(self, case_id: str) -> CreateCaseRequest:
+        case_qc_metrics: dict = self.get_case_qc_metrics(case_id)
+        if not case_qc_metrics:
+            raise ValueError(f"Could not retrieve qc metrics from Janus for case {case_id}")
+        return CreateCaseRequest(**case_qc_metrics)
+
+    def create_case(self, case_id: str, dry_run: bool = False):
+        case_request: CreateCaseRequest = self.get_create_case_request(case_id)
+        if dry_run:
+            LOG.info(f"Would have sent create case request to Arnold with: {case_request}")
+            return
+        self.arnold_api.create_case(case_request)
```

### Comparing `cg-59.9.1/cg/meta/report/balsamic.py` & `cg-60.0.0/cg/meta/report/balsamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
 
 class BalsamicReportAPI(ReportAPI):
     """API to create Balsamic delivery reports."""
 
     def __init__(self, config: CGConfig, analysis_api: BalsamicAnalysisAPI):
         super().__init__(config=config, analysis_api=analysis_api)
-        self.analysis_api: BalsamicAnalysisAPI = analysis_api
 
     def get_sample_metadata(
         self, case: Case, sample: Sample, analysis_metadata: BalsamicAnalysis
     ) -> BalsamicTargetedSampleMetadataModel | BalsamicWGSSampleMetadataModel:
         """Return sample metadata to include in the report."""
         sample_metrics: dict[str, BalsamicQCMetrics] = analysis_metadata.sample_metrics[
             sample.internal_id
```

### Comparing `cg-59.9.1/cg/meta/report/balsamic_qc.py` & `cg-60.0.0/cg/meta/report/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/report/balsamic_umi.py` & `cg-60.0.0/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/report/field_validators.py` & `cg-60.0.0/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/report/mip_dna.py` & `cg-60.0.0/cg/meta/report/mip_dna.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 
 class MipDNAReportAPI(ReportAPI):
     """API to create Rare disease DNA delivery reports."""
 
     def __init__(self, config: CGConfig, analysis_api: MipDNAAnalysisAPI):
         super().__init__(config=config, analysis_api=analysis_api)
-        self.analysis_api: MipDNAAnalysisAPI = analysis_api
 
     def get_sample_metadata(
         self, case: Case, sample: Sample, analysis_metadata: MipAnalysis
     ) -> MipDNASampleMetadataModel:
         """Return MIP DNA sample metadata to include in the report."""
         parsed_metrics = get_sample_id_metric(
             sample_id=sample.internal_id, sample_id_metrics=analysis_metadata.sample_id_metrics
```

### Comparing `cg-59.9.1/cg/meta/report/report_api.py` & `cg-60.0.0/cg/meta/report/report_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,14 +248,26 @@
         samples = list()
         case_samples: list[CaseSample] = self.status_db.get_case_samples_by_case_id(
             case_internal_id=case.internal_id
         )
         for case_sample in case_samples:
             sample: Sample = case_sample.sample
             lims_sample: dict | None = self.get_lims_sample(sample_id=sample.internal_id)
+            delivered_files: list[File] | None = (
+                self.delivery_api.get_analysis_sample_delivery_files_by_sample(
+                    case=case, sample=sample
+                )
+                if self.delivery_api.is_analysis_delivery(case.data_delivery)
+                else None
+            )
+            delivered_fastq_files: list[File] | None = (
+                self.delivery_api.get_fastq_delivery_files_by_sample(case=case, sample=sample)
+                if self.delivery_api.is_fastq_delivery(case.data_delivery)
+                else None
+            )
             samples.append(
                 SampleModel(
                     name=sample.name,
                     id=sample.internal_id,
                     ticket=sample.original_ticket,
                     gender=sample.sex,
                     source=lims_sample.get("source") if lims_sample else None,
@@ -265,14 +277,16 @@
                     ),
                     methods=self.get_sample_methods_data(sample_id=sample.internal_id),
                     status=case_sample.status,
                     metadata=self.get_sample_metadata(
                         case=case, sample=sample, analysis_metadata=analysis_metadata
                     ),
                     timestamps=self.get_sample_timestamp_data(sample=sample),
+                    delivered_files=delivered_files,
+                    delivered_fastq_files=delivered_fastq_files,
                 )
             )
         return samples
 
     def get_lims_sample(self, sample_id: str) -> dict | None:
         """Fetches sample data from LIMS. Returns an empty dictionary if the request was unsuccessful."""
         lims_sample = dict()
@@ -336,24 +350,30 @@
     def get_case_analysis_data(
         self,
         case: Case,
         analysis: Analysis,
         analysis_metadata: AnalysisModel,
     ) -> DataAnalysisModel:
         """Return workflow attributes used for data analysis."""
+        delivered_files: list[File] | None = (
+            self.delivery_api.get_analysis_case_delivery_files(case=case)
+            if self.delivery_api.is_analysis_delivery(case.data_delivery)
+            else None
+        )
         return DataAnalysisModel(
             customer_workflow=case.data_analysis,
             data_delivery=case.data_delivery,
             workflow=analysis.workflow,
             workflow_version=analysis.workflow_version,
             type=self.get_data_analysis_type(case=case),
             genome_build=self.get_genome_build(analysis_metadata=analysis_metadata),
             variant_callers=self.get_variant_callers(_analysis_metadata=analysis_metadata),
             panels=case.panels,
             scout_files=self.get_scout_uploaded_files(case=case),
+            delivered_files=delivered_files,
         )
 
     def get_scout_uploaded_files(self, case: Case) -> ScoutReportFiles:
         """Return files that will be uploaded to Scout."""
         raise NotImplementedError
 
     @staticmethod
```

### Comparing `cg-59.9.1/cg/meta/report/rnafusion.py` & `cg-60.0.0/cg/meta/report/rnafusion.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     REQUIRED_CUSTOMER_FIELDS,
     REQUIRED_DATA_ANALYSIS_RNAFUSION_FIELDS,
     REQUIRED_REPORT_FIELDS,
     REQUIRED_SAMPLE_METADATA_RNAFUSION_FIELDS,
     REQUIRED_SAMPLE_METHODS_FIELDS,
     REQUIRED_SAMPLE_RNAFUSION_FIELDS,
     REQUIRED_SAMPLE_TIMESTAMP_FIELDS,
+    RNAFUSION_REPORT_ACCREDITED_APPTAGS,
+    RNAFUSION_REPORT_MINIMUM_INPUT_AMOUNT,
     Workflow,
 )
 from cg.constants.constants import GenomeVersion
 from cg.constants.scout import RNAFUSION_CASE_TAGS
 from cg.meta.report.field_validators import (
     get_mapped_reads_fraction,
     get_million_read_pairs,
@@ -30,15 +32,14 @@
 
 
 class RnafusionReportAPI(ReportAPI):
     """API to create RNAfusion delivery reports."""
 
     def __init__(self, config: CGConfig, analysis_api: RnafusionAnalysisAPI):
         super().__init__(config=config, analysis_api=analysis_api)
-        self.analysis_api: RnafusionAnalysisAPI = analysis_api
 
     def get_sample_metadata(
         self, case: Case, sample: Sample, analysis_metadata: RnafusionAnalysis
     ) -> RnafusionSampleMetadataModel:
         """Return sample metadata to include in the report."""
         sample_metrics: RnafusionQCMetrics = analysis_metadata.sample_metrics[sample.internal_id]
 
@@ -74,19 +75,39 @@
             uniquely_mapped_reads=sample_metrics.uniquely_mapped_percent,
         )
 
     def get_genome_build(self, analysis_metadata: AnalysisModel) -> str:
         """Return build version of the genome reference of a specific case."""
         return GenomeVersion.hg38.value
 
+    @staticmethod
+    def is_apptag_accredited(samples: list[SampleModel]) -> bool:
+        """Return Rnafusion input application tag accreditation status."""
+        return all(
+            sample.application.tag in RNAFUSION_REPORT_ACCREDITED_APPTAGS for sample in samples
+        )
+
+    @staticmethod
+    def is_input_amount_accredited(samples: list[SampleModel]) -> bool:
+        """Return Rnafusion input amount accreditation status."""
+        try:
+            return all(
+                float(sample.metadata.input_amount) >= RNAFUSION_REPORT_MINIMUM_INPUT_AMOUNT
+                for sample in samples
+            )
+        except ValueError:
+            return False
+
     def is_report_accredited(
         self, samples: list[SampleModel], analysis_metadata: AnalysisModel
     ) -> bool:
-        """Check if the report is accredited. Rnafusion is an accredited workflow."""
-        return True
+        """Return whether the Rnafusion delivery report is accredited or not."""
+        is_apptag_accredited: bool = self.is_apptag_accredited(samples)
+        is_input_amount_accredited: bool = self.is_input_amount_accredited(samples)
+        return is_apptag_accredited and is_input_amount_accredited
 
     def get_template_name(self) -> str:
         """Return template name to render the delivery report."""
         return Workflow.RNAFUSION + "_report.html"
 
     def get_scout_uploaded_files(self, case: Case) -> ScoutReportFiles:
         """Return files that will be uploaded to Scout."""
```

### Comparing `cg-59.9.1/cg/meta/report/templates/balsamic_report.html` & `cg-60.0.0/cg/meta/report/templates/balsamic_report.html`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         <div class="card-block">
           <h4 class="card-title">Leveransrapport Clinical Genomics</h4>
         </div>
 
         <ul class="list-group list-group-flush">
           <li class="list-group-item">
           <brief>
-            <strong>Leveransrapport</strong> {{ customer.name }}, <strong>familj</strong> {{ case.name }}
+            <strong>Leveransrapport</strong> {{ customer.name }}, <strong>fall</strong> {{ case.name }}
             {% if version != 'N/A' %}
               , <strong>version</strong>: {{ version }}
             {% endif %}
             <br>
             Skapad: {{ date }}
           </brief>
           </li>
@@ -62,15 +62,15 @@
 
         <div class="card-block">
           <table class="table table-bordered" aria-describedby="Sample table">
             <thead>
               <tr>
                 <th>Prov</th>
                 <th>Beställt</th>
-                <th>Case</th>
+                <th>Fall</th>
                 <th>Kön</th>
                 <th>Provtyp</th>
                 <th>Ticket</th>
                 <th>Applikation</th>
                 <th>Bioinformatisk analys</th>
                 <th>Tumör</th>
               </tr>
@@ -133,15 +133,15 @@
           </table>
         </div>
 
         <div class="card-block">
           <table class="table table-bordered" aria-describedby="Case table">
             <thead>
               <tr>
-                <th>Case</th>
+                <th>Fall</th>
                 <th>Balsamic-version</th>
                 <th>Genomversion</th>
                 <th>Analystyp</th>
               </tr>
             </thead>
             <tbody>
               <tr>
@@ -288,14 +288,68 @@
           </p>
         </div>
 
         <div class="card-block">
           All kommunikation gällande ordern såsom tillägg, avvikelser eller ev undantag i metoden från Clinical Genomics finns tillgängligt i SupportSystem för detta ticket id. En stängd ticket kan närsomhelst öppnas upp igen för frågor.
         </div>
 
+	      {% if "analysis" in case.data_analysis.data_delivery or "fastq" in case.data_analysis.data_delivery %}
+          <div class="card-block">
+            <h4 class="card-title">Bilaga</h4>
+            <div class="card-text">
+	            <div class="card-block">
+                <h5 class="card-title">Caesar</h5>
+                <div class="card-text">
+	                <p>Filer som ska laddas upp till din inkorg: <i>/home/{{ customer.id }}/inbox/{{ case.samples[0].ticket }}</i></p>
+	                <ul>
+	                  {% if "analysis" in case.data_analysis.data_delivery %}
+		                  <li><b>Analysfiler</b>:</li>
+		                  <ul>
+		                    {% if case.data_analysis.delivered_files != 'N/A' %}
+			                    <li><b>Fall</b>: {{ case.name }}</li>
+				      			      <ul>
+				      				      {% for file in case.data_analysis.delivered_files %}
+                              <li>{{ file }}</li>
+                            {% endfor %}
+				                  </ul>
+		                    {% endif %}
+			                  {% for sample in case.samples %}
+				                  {% if sample.delivered_files != 'N/A' %}
+				      			        <li><b>Prov</b>: {{ sample.name }}</li>
+				                    <ul>
+				      				        {% for file in sample.delivered_files %}
+                                <li>{{ file }}</li>
+                              {% endfor %}
+				                    </ul>
+				                  {% endif %}
+			                  {% endfor %}
+		                  </ul>
+		                {% endif %}
+	                  {% if "fastq" in case.data_analysis.data_delivery %}
+			                <li><b>Fastq-filer</b>:</li>
+	                    <ul>
+			                  {% for sample in case.samples %}
+				                  {% if sample.delivered_fastq_files != 'N/A' %}
+				      			        <li><b>Prov</b>: {{ sample.name }}</li>
+				                    <ul>
+				                      {% for file in sample.delivered_fastq_files %}
+                                <li>{{ file }}</li>
+                              {% endfor %}
+				                    </ul>
+				                  {% endif %}
+			                  {% endfor %}
+	                    </ul>
+		                {% endif %}
+	                </ul>
+                </div>
+	            </div>
+            </div>
+          </div>
+				{% endif %}
+
         <div class="card-footer">
           <div class="text-muted text-center">Slut på rapport</div>
         </div>
       </div>
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% from "bootstrap.html" import css, custom_css %}
 {{ css() }} {{ custom_css() }}
 ****** LLeevveerraannssrraappppoorrtt CClliinniiccaall GGeennoommiiccss ******
-    * LLeevveerraannssrraappppoorrtt {{ customer.name }}, ffaammiilljj {{ case.name }} {% if version
+    * LLeevveerraannssrraappppoorrtt {{ customer.name }}, ffaallll {{ case.name }} {% if version
       != 'N/A' %} , vveerrssiioonn: {{ version }} {% endif %}
       Skapad: {{ date }}
 ****** KKoonnttaakktt CClliinniiccaall GGeennoommiiccss ******
      CClliinniiccaall GGeennoommiiccss
      Science for Life Laboratory
      Tomtebodavägen 23
      171 65 Solna
@@ -14,15 +14,15 @@
 ****** KKuunnddiinnffoorrmmaattiioonn ******
      {{{{ ccuussttoommeerr..nnaammee }}}}
      {{ customer.invoice_address | replace('\n', '
      ') | safe }}
 {% if accredited %}
 [SWEDAC logo]
 {% endif %}
-PPrroovv        BBeesstt?älllltt                     CCaassee      KK?önn           PPrroovvttyypp       TTiicckkeett        AApppplliikkaattiioonn            BBiiooiinnffoorrmmaattiisskk aannaallyyss                TTuumm?örr
+PPrroovv        BBeesstt?älllltt                     FFaallll      KK?önn           PPrroovvttyypp       TTiicckkeett        AApppplliikkaattiioonn            BBiiooiinnffoorrmmaattiisskk aannaallyyss                TTuumm?örr
 {
 {           {                            {         {             {             {             {                      {                                    {
 sample.name {                            {         {             {             {             {                      {                                    {
 }}* ({      sample.timestamps.ordered_at case.name sample.gender sample.source sample.ticket sample.application.tag case.data_analysis.customer_workflow sample.tumour
 { sample.id }}                           }}*       }}*           }}*           }}            }}*                    }}*                                  }}*
 }})
 PPrroovv        AAnnkkoomm                         BBiibblliiootteekkssbbeerreeddnniinngg         BBeerreedddd                        BBaaiitt SSeett                         SSeekkvveennsseerriinngg              SSeekkvveennsseerraadd                        BBiiooiinnffoorrmmaattiisskk aannaallyyss
@@ -30,15 +30,15 @@
                                                                                                     {% if sample.metadata.bait_set
 {           {                             {                           {                             != 'N/A' and                     {                         {                                  {
 {           {                             {                           {                             sample.metadata.bait_set_version {                         {                                  {
 sample.name sample.timestamps.received_at sample.methods.library_prep sample.timestamps.prepared_at != 'N/A' %} (version: {          sample.methods.sequencing sample.timestamps.reads_updated_at case.data_analysis.workflow
 }}*         }}                            }}                          }}                            {                                }}                        }}                                 }}
                                                                                                     sample.metadata.bait_set_version
                                                                                                     }}) {% endif %}
-CCaassee      BBaallssaammiicc--vveerrssiioonn                    GGeennoommvveerrssiioonn                    AAnnaallyyssttyypp
+FFaallll      BBaallssaammiicc--vveerrssiioonn                    GGeennoommvveerrssiioonn                    AAnnaallyyssttyypp
 {         {                                   {                               {
 {         {                                   {                               {
 case.name case.data_analysis.workflow_version case.data_analysis.genome_build case.data_analysis.type
 }}*       }}                                  }}                              }}
 PPrroovv        LL?ässppaarr [[MM]]                         MMeeddiiaanntt?äcckknniinngg [[bbaasseerr]]          TT?äcckknniinnggssggrraadd 1155xx [[%%]]   TT?äcckknniinnggssggrraadd 6600xx [[%%]]   TT?äcckknniinnggssggrraadd 6600xx [[%%]]   LL?ässnniinnggaarr mmeedd ffeellaakkttiiggaa ppaarr [[%%]]          TT?äcckknniinnggssggrraadd 225500xx [[%%]]                 TT?äcckknniinnggssggrraadd 550000xx [[%%]]   GGCC DDrrooppoouutt [[%%]]           DDuupplliikkaatt [[%%]]               MMeeddeellffrraaggmmeennttll?ännggdd         FFoolldd 8800 bbaassee ppeennaallttyy
                                                                                                                                                                                                                                                                                                                     [[bbaassppaarr]]
 {           {                                  {                               {                       {                       {                       {                                        {                                      {                        {                        {                          {                          {                                {
@@ -83,8 +83,39 @@
 resultaten gäller för provet såsom det har mottagits.
 ****** SSiiggnnaattuurr ff?örr ggooddkk?ännnnaannddee aavv rraappppoorrtt ******
 Valtteri Wirta
 Director, Clinical Genomics
 All kommunikation gällande ordern såsom tillägg, avvikelser eller ev undantag i
 metoden från Clinical Genomics finns tillgängligt i SupportSystem för detta
 ticket id. En stängd ticket kan närsomhelst öppnas upp igen för frågor.
+{% if "analysis" in case.data_analysis.data_delivery or "fastq" in
+case.data_analysis.data_delivery %}
+****** BBiillaaggaa ******
+**** CCaaeessaarr ****
+Filer som ska laddas upp till din inkorg: /home/{{ customer.id }}/inbox/{
+{ case.samples[0].ticket }}
+    * {% if "analysis" in case.data_analysis.data_delivery %}
+    * AAnnaallyyssffiilleerr:
+          o {% if case.data_analysis.delivered_files != 'N/A' %}
+          o FFaallll: {{ case.name }}
+                # {% for file in case.data_analysis.delivered_files %}
+                # {{ file }}
+                # {% endfor %}
+          o {% endif %} {% for sample in case.samples %} {% if
+            sample.delivered_files != 'N/A' %}
+          o PPrroovv: {{ sample.name }}
+                # {% for file in sample.delivered_files %}
+                # {{ file }}
+                # {% endfor %}
+          o {% endif %} {% endfor %}
+    * {% endif %} {% if "fastq" in case.data_analysis.data_delivery %}
+    * FFaassttqq--ffiilleerr:
+          o {% for sample in case.samples %} {% if sample.delivered_fastq_files
+            != 'N/A' %}
+          o PPrroovv: {{ sample.name }}
+                # {% for file in sample.delivered_fastq_files %}
+                # {{ file }}
+                # {% endfor %}
+          o {% endif %} {% endfor %}
+    * {% endif %}
+{% endif %}
 Slut på rapport
```

### Comparing `cg-59.9.1/cg/meta/report/templates/bootstrap.html` & `cg-60.0.0/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/report/templates/mip-dna_report.html` & `cg-60.0.0/cg/meta/report/templates/mip-dna_report.html`

 * *Files 4% similar despite different names*

```diff
@@ -257,14 +257,68 @@
           </p>
         </div>
 
         <div class="card-block">
           All kommunikation gällande ordern såsom tillägg, avvikelser eller ev undantag i metoden från Clinical Genomics finns tillgängligt i SupportSystem för detta ticket id. En stängd ticket kan närsomhelst öppnas upp igen för frågor.
         </div>
 
+	      {% if "analysis" in case.data_analysis.data_delivery or "fastq" in case.data_analysis.data_delivery %}
+          <div class="card-block">
+            <h4 class="card-title">Bilaga</h4>
+            <div class="card-text">
+	            <div class="card-block">
+                <h5 class="card-title">Caesar</h5>
+                <div class="card-text">
+	                <p>Filer som ska laddas upp till din inkorg: <i>/home/{{ customer.id }}/inbox/{{ case.samples[0].ticket }}</i></p>
+	                <ul>
+	                  {% if "analysis" in case.data_analysis.data_delivery %}
+		                  <li><b>Analysfiler</b>:</li>
+		                  <ul>
+		                    {% if case.data_analysis.delivered_files != 'N/A' %}
+			                    <li><b>Familj</b>: {{ case.name }}</li>
+				      			      <ul>
+				      				      {% for file in case.data_analysis.delivered_files %}
+                              <li>{{ file }}</li>
+                            {% endfor %}
+				                  </ul>
+		                    {% endif %}
+			                  {% for sample in case.samples %}
+				                  {% if sample.delivered_files != 'N/A' %}
+				      			        <li><b>Prov</b>: {{ sample.name }}</li>
+				                    <ul>
+				      				        {% for file in sample.delivered_files %}
+                                <li>{{ file }}</li>
+                              {% endfor %}
+				                    </ul>
+				                  {% endif %}
+			                  {% endfor %}
+		                  </ul>
+		                {% endif %}
+	                  {% if "fastq" in case.data_analysis.data_delivery %}
+			                <li><b>Fastq-filer</b>:</li>
+	                    <ul>
+			                  {% for sample in case.samples %}
+				                  {% if sample.delivered_fastq_files != 'N/A' %}
+				      			        <li><b>Prov</b>: {{ sample.name }}</li>
+				                    <ul>
+				                      {% for file in sample.delivered_fastq_files %}
+                                <li>{{ file }}</li>
+                              {% endfor %}
+				                    </ul>
+				                  {% endif %}
+			                  {% endfor %}
+	                    </ul>
+		                {% endif %}
+	                </ul>
+                </div>
+	            </div>
+            </div>
+          </div>
+				{% endif %}
+
         <div class="card-footer">
           <div class="text-muted text-center">Slut på rapport</div>
         </div>
       </div>
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -92,8 +92,39 @@
 resultaten gäller för provet såsom det har mottagits.
 ****** SSiiggnnaattuurr ff?örr ggooddkk?ännnnaannddee aavv rraappppoorrtt ******
 Valtteri Wirta
 Director, Clinical Genomics
 All kommunikation gällande ordern såsom tillägg, avvikelser eller ev undantag i
 metoden från Clinical Genomics finns tillgängligt i SupportSystem för detta
 ticket id. En stängd ticket kan närsomhelst öppnas upp igen för frågor.
+{% if "analysis" in case.data_analysis.data_delivery or "fastq" in
+case.data_analysis.data_delivery %}
+****** BBiillaaggaa ******
+**** CCaaeessaarr ****
+Filer som ska laddas upp till din inkorg: /home/{{ customer.id }}/inbox/{
+{ case.samples[0].ticket }}
+    * {% if "analysis" in case.data_analysis.data_delivery %}
+    * AAnnaallyyssffiilleerr:
+          o {% if case.data_analysis.delivered_files != 'N/A' %}
+          o FFaammiilljj: {{ case.name }}
+                # {% for file in case.data_analysis.delivered_files %}
+                # {{ file }}
+                # {% endfor %}
+          o {% endif %} {% for sample in case.samples %} {% if
+            sample.delivered_files != 'N/A' %}
+          o PPrroovv: {{ sample.name }}
+                # {% for file in sample.delivered_files %}
+                # {{ file }}
+                # {% endfor %}
+          o {% endif %} {% endfor %}
+    * {% endif %} {% if "fastq" in case.data_analysis.data_delivery %}
+    * FFaassttqq--ffiilleerr:
+          o {% for sample in case.samples %} {% if sample.delivered_fastq_files
+            != 'N/A' %}
+          o PPrroovv: {{ sample.name }}
+                # {% for file in sample.delivered_fastq_files %}
+                # {{ file }}
+                # {% endfor %}
+          o {% endif %} {% endfor %}
+    * {% endif %}
+{% endif %}
 Slut på rapport
```

### Comparing `cg-59.9.1/cg/meta/report/templates/rnafusion_report.html` & `cg-60.0.0/cg/meta/report/templates/rnafusion_report.html`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         <div class="card-block">
           <h4 class="card-title">Leveransrapport Clinical Genomics</h4>
         </div>
 
         <ul class="list-group list-group-flush">
           <li class="list-group-item">
           <brief>
-            <strong>Leveransrapport</strong> {{ customer.name }}, <strong>familj</strong> {{ case.name }}
+            <strong>Leveransrapport</strong> {{ customer.name }}, <strong>fall</strong> {{ case.name }}
             {% if version != 'N/A' %}
               , <strong>version</strong>: {{ version }}
             {% endif %}
             <br>
             Skapad: {{ date }}
           </brief>
           </li>
@@ -62,15 +62,15 @@
 
         <div class="card-block">
           <table class="table table-bordered" aria-describedby="Sample table">
             <thead>
               <tr>
                 <th>Prov</th>
                 <th>Beställt</th>
-                <th>Case</th>
+                <th>Fall</th>
                 <th>Kön</th>
                 <th>Provtyp</th>
                 <th>Ticket</th>
                 <th>Applikation</th>
                 <th>Bioinformatisk analys</th>
                 <th>Tumör</th>
               </tr>
@@ -122,15 +122,15 @@
           </table>
         </div>
 
         <div class="card-block">
           <table class="table table-bordered" aria-describedby="Case table">
             <thead>
               <tr>
-                <th>Case</th>
+                <th>Fall</th>
                 <th>Rnafusion-version</th>
                 <th>Genpaneler</th>
                 <th>Genomversion</th>
               </tr>
             </thead>
             <tbody>
               <tr>
@@ -270,14 +270,68 @@
           </p>
         </div>
 
         <div class="card-block">
           All kommunikation gällande ordern såsom tillägg, avvikelser eller ev undantag i metoden från Clinical Genomics finns tillgängligt i SupportSystem för detta ticket id. En stängd ticket kan närsomhelst öppnas upp igen för frågor.
         </div>
 
+	      {% if "analysis" in case.data_analysis.data_delivery or "fastq" in case.data_analysis.data_delivery %}
+          <div class="card-block">
+            <h4 class="card-title">Bilaga</h4>
+            <div class="card-text">
+	            <div class="card-block">
+                <h5 class="card-title">Caesar</h5>
+                <div class="card-text">
+	                <p>Filer som ska laddas upp till din inkorg: <i>/home/{{ customer.id }}/inbox/{{ case.samples[0].ticket }}</i></p>
+	                <ul>
+	                  {% if "analysis" in case.data_analysis.data_delivery %}
+		                  <li><b>Analysfiler</b>:</li>
+		                  <ul>
+		                    {% if case.data_analysis.delivered_files != 'N/A' %}
+			                    <li><b>Fall</b>: {{ case.name }}</li>
+				      			      <ul>
+				      				      {% for file in case.data_analysis.delivered_files %}
+                              <li>{{ file }}</li>
+                            {% endfor %}
+				                  </ul>
+		                    {% endif %}
+			                  {% for sample in case.samples %}
+				                  {% if sample.delivered_files != 'N/A' %}
+				      			        <li><b>Prov</b>: {{ sample.name }}</li>
+				                    <ul>
+				      				        {% for file in sample.delivered_files %}
+                                <li>{{ file }}</li>
+                              {% endfor %}
+				                    </ul>
+				                  {% endif %}
+			                  {% endfor %}
+		                  </ul>
+		                {% endif %}
+	                  {% if "fastq" in case.data_analysis.data_delivery %}
+			                <li><b>Fastq-filer</b>:</li>
+	                    <ul>
+			                  {% for sample in case.samples %}
+				                  {% if sample.delivered_fastq_files != 'N/A' %}
+				      			        <li><b>Prov</b>: {{ sample.name }}</li>
+				                    <ul>
+				                      {% for file in sample.delivered_fastq_files %}
+                                <li>{{ file }}</li>
+                              {% endfor %}
+				                    </ul>
+				                  {% endif %}
+			                  {% endfor %}
+	                    </ul>
+		                {% endif %}
+	                </ul>
+                </div>
+	            </div>
+            </div>
+          </div>
+				{% endif %}
+
         <div class="card-footer">
           <div class="text-muted text-center">Slut på rapport</div>
         </div>
       </div>
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% from "bootstrap.html" import css, custom_css %}
 {{ css() }} {{ custom_css() }}
 ****** LLeevveerraannssrraappppoorrtt CClliinniiccaall GGeennoommiiccss ******
-    * LLeevveerraannssrraappppoorrtt {{ customer.name }}, ffaammiilljj {{ case.name }} {% if version
+    * LLeevveerraannssrraappppoorrtt {{ customer.name }}, ffaallll {{ case.name }} {% if version
       != 'N/A' %} , vveerrssiioonn: {{ version }} {% endif %}
       Skapad: {{ date }}
 ****** KKoonnttaakktt CClliinniiccaall GGeennoommiiccss ******
      CClliinniiccaall GGeennoommiiccss
      Science for Life Laboratory
      Tomtebodavägen 23
      171 65 Solna
@@ -14,27 +14,27 @@
 ****** KKuunnddiinnffoorrmmaattiioonn ******
      {{{{ ccuussttoommeerr..nnaammee }}}}
      {{ customer.invoice_address | replace('\n', '
      ') | safe }}
 {% if accredited %}
 [SWEDAC logo]
 {% endif %}
-PPrroovv        BBeesstt?älllltt                     CCaassee      KK?önn           PPrroovvttyypp       TTiicckkeett        AApppplliikkaattiioonn            BBiiooiinnffoorrmmaattiisskk aannaallyyss                TTuumm?örr
+PPrroovv        BBeesstt?älllltt                     FFaallll      KK?önn           PPrroovvttyypp       TTiicckkeett        AApppplliikkaattiioonn            BBiiooiinnffoorrmmaattiisskk aannaallyyss                TTuumm?örr
 {
 {           {                            {         {             {             {             {                      {                                    {
 sample.name {                            {         {             {             {             {                      {                                    {
 }}* ({      sample.timestamps.ordered_at case.name sample.gender sample.source sample.ticket sample.application.tag case.data_analysis.customer_workflow sample.tumour
 { sample.id }}                           }}*       }}*           }}*           }}            }}*                    }}*                                  }}*
 }})
 PPrroovv        AAnnkkoomm                         BBiibblliiootteekkssbbeerreeddnniinngg         BBeerreedddd                        SSeekkvveennsseerriinngg              SSeekkvveennsseerraadd                        BBiiooiinnffoorrmmaattiisskk aannaallyyss
 {           {                             {                           {                             {                         {                                  {
 {           {                             {                           {                             {                         {                                  {
 sample.name sample.timestamps.received_at sample.methods.library_prep sample.timestamps.prepared_at sample.methods.sequencing sample.timestamps.reads_updated_at case.data_analysis.workflow
 }}*         }}                            }}                          }}                            }}                        }}                                 }}
-CCaassee      RRnnaaffuussiioonn--vveerrssiioonn                   GGeennppaanneelleerr                GGeennoommvveerrssiioonn
+FFaallll      RRnnaaffuussiioonn--vveerrssiioonn                   GGeennppaanneelleerr                GGeennoommvveerrssiioonn
 {         {                                   {                         {
 {         {                                   {                         {
 case.name case.data_analysis.workflow_version case.data_analysis.panels case.data_analysis.genome_build
 }}*       }}                                  }}                        }}
 PPrroovv
 {{ sample.name }}
 RRIINN                           IInngg?åeennddee mm?ännggdd [[nngg]]            LL?ässppaarr [[MM]]                         MMaappppaaddee sseekkvveennsseerr [[%%]]        UUnniikktt mmaappppaaddee sseekkvveennsseerr [[%%]]           DDuupplliikkaatt [[%%]]               AAddaapptteerr [[%%]]                     55''--33'' bbiiaass
@@ -74,8 +74,39 @@
 resultaten gäller för provet såsom det har mottagits.
 ****** SSiiggnnaattuurr ff?örr ggooddkk?ännnnaannddee aavv rraappppoorrtt ******
 Valtteri Wirta
 Director, Clinical Genomics
 All kommunikation gällande ordern såsom tillägg, avvikelser eller ev undantag i
 metoden från Clinical Genomics finns tillgängligt i SupportSystem för detta
 ticket id. En stängd ticket kan närsomhelst öppnas upp igen för frågor.
+{% if "analysis" in case.data_analysis.data_delivery or "fastq" in
+case.data_analysis.data_delivery %}
+****** BBiillaaggaa ******
+**** CCaaeessaarr ****
+Filer som ska laddas upp till din inkorg: /home/{{ customer.id }}/inbox/{
+{ case.samples[0].ticket }}
+    * {% if "analysis" in case.data_analysis.data_delivery %}
+    * AAnnaallyyssffiilleerr:
+          o {% if case.data_analysis.delivered_files != 'N/A' %}
+          o FFaallll: {{ case.name }}
+                # {% for file in case.data_analysis.delivered_files %}
+                # {{ file }}
+                # {% endfor %}
+          o {% endif %} {% for sample in case.samples %} {% if
+            sample.delivered_files != 'N/A' %}
+          o PPrroovv: {{ sample.name }}
+                # {% for file in sample.delivered_files %}
+                # {{ file }}
+                # {% endfor %}
+          o {% endif %} {% endfor %}
+    * {% endif %} {% if "fastq" in case.data_analysis.data_delivery %}
+    * FFaassttqq--ffiilleerr:
+          o {% for sample in case.samples %} {% if sample.delivered_fastq_files
+            != 'N/A' %}
+          o PPrroovv: {{ sample.name }}
+                # {% for file in sample.delivered_fastq_files %}
+                # {{ file }}
+                # {% endfor %}
+          o {% endif %} {% endfor %}
+    * {% endif %}
+{% endif %}
 Slut på rapport
```

### Comparing `cg-59.9.1/cg/meta/rsync/rsync_api.py` & `cg-60.0.0/cg/meta/rsync/rsync_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,16 +61,19 @@
 
     @staticmethod
     def get_trailblazer_config(slurm_job_id: int) -> dict[str, list[str]]:
         """Return dictionary of slurm job IDs."""
         return {"jobs": [str(slurm_job_id)]}
 
     @staticmethod
-    def write_trailblazer_config(content: dict, config_path: Path) -> None:
+    def write_trailblazer_config(content: dict, config_path: Path, dry_run: bool = False) -> None:
         """Write slurm job IDs to a .YAML file used as the trailblazer config."""
+        if dry_run:
+            LOG.info(f"Dry-run: it would write slurm jobs to {config_path.as_posix()}")
+            return
         LOG.info(f"Writing slurm jobs to {config_path.as_posix()}")
         WriteFile.write_file_from_content(
             content=content, file_format=FileFormat.YAML, file_path=config_path
         )
 
     @staticmethod
     def process_ready_to_clean(before: dt.datetime, process: Path) -> bool:
```

### Comparing `cg-59.9.1/cg/meta/tar/tar.py` & `cg-60.0.0/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/transfer/external_data.py` & `cg-60.0.0/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/transfer/lims.py` & `cg-60.0.0/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/balsamic/balsamic.py` & `cg-60.0.0/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/coverage.py` & `cg-60.0.0/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/fohm/fohm.py` & `cg-60.0.0/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/gisaid/constants.py` & `cg-60.0.0/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/gisaid/gisaid.py` & `cg-60.0.0/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/gisaid/models.py` & `cg-60.0.0/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/gt.py` & `cg-60.0.0/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/microsalt/microsalt_upload_api.py` & `cg-60.0.0/cg/meta/upload/microsalt/microsalt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/mip/mip_dna.py` & `cg-60.0.0/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/mip/mip_rna.py` & `cg-60.0.0/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/mutacc.py` & `cg-60.0.0/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/nipt/models.py` & `cg-60.0.0/cg/meta/upload/nipt/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/nipt/nipt.py` & `cg-60.0.0/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/rnafusion/rnafusion.py` & `cg-60.0.0/cg/meta/upload/nf_analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-"""Rnafusion upload API."""
+"""NF Analysis upload API."""
 
 import datetime as dt
 import logging
 
 import click
 
 from cg.cli.generate.report.base import generate_delivery_report
 from cg.cli.upload.clinical_delivery import upload_clinical_delivery
 from cg.cli.upload.scout import upload_to_scout
-from cg.constants import REPORT_SUPPORTED_DATA_DELIVERY, DataDelivery
+from cg.constants import (
+    REPORT_SUPPORTED_DATA_DELIVERY,
+    REPORT_SUPPORTED_WORKFLOW,
+    DataDelivery,
+    Workflow,
+)
 from cg.meta.upload.upload_api import UploadAPI
-from cg.meta.workflow.rnafusion import RnafusionAnalysisAPI
+from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.cg_config import CGConfig
 from cg.store.models import Analysis, Case
 
 LOG = logging.getLogger(__name__)
 
 
-class RnafusionUploadAPI(UploadAPI):
-    """Rnafusion upload API."""
+class NfAnalysisUploadAPI(UploadAPI):
+    """Nf analysis upload API."""
 
-    def __init__(self, config: CGConfig):
-        self.analysis_api: RnafusionAnalysisAPI = RnafusionAnalysisAPI(config)
+    def __init__(self, config: CGConfig, workflow: Workflow):
+        self.analysis_api: NfAnalysisAPI = NfAnalysisAPI(config, workflow)
         super().__init__(config=config, analysis_api=self.analysis_api)
 
     def upload(self, ctx: click.Context, case: Case, restart: bool) -> None:
-        """Upload Rnafusion analysis data and files."""
+        """Upload NF analysis data and files."""
         analysis: Analysis = case.analyses[0]
         self.update_upload_started_at(analysis=analysis)
 
         # Delivery report generation
-        if case.data_delivery in REPORT_SUPPORTED_DATA_DELIVERY:
+        if (
+            case.data_analysis in REPORT_SUPPORTED_WORKFLOW
+            and case.data_delivery in REPORT_SUPPORTED_DATA_DELIVERY
+        ):
             ctx.invoke(generate_delivery_report, case_id=case.internal_id)
 
         # Clinical delivery
         ctx.invoke(upload_clinical_delivery, case_id=case.internal_id)
 
         # Scout specific upload
         if DataDelivery.SCOUT in case.data_delivery:
```

### Comparing `cg-59.9.1/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-60.0.0/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-60.0.0/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/scout/hk_tags.py` & `cg-60.0.0/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/scout/mip_config_builder.py` & `cg-60.0.0/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-60.0.0/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/scout/scout_config_builder.py` & `cg-60.0.0/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/scout/uploadscoutapi.py` & `cg-60.0.0/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/upload/upload_api.py` & `cg-60.0.0/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/analysis.py` & `cg-60.0.0/cg/meta/workflow/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,31 @@
             AnalysisType.WHOLE_EXOME_SEQUENCING,
             AnalysisType.WHOLE_GENOME_SEQUENCING,
             AnalysisType.WHOLE_TRANSCRIPTOME_SEQUENCING,
         }:
             return prep_category.lower()
         return AnalysisType.OTHER
 
+    def get_case_application_type(self, case_id: str) -> str:
+        """Returns the application type for samples in a case."""
+        samples: list[Sample] = self.status_db.get_samples_by_case_id(case_id)
+        application_types: set[str] = {self.get_application_type(sample) for sample in samples}
+
+        if len(application_types) > 1:
+            raise CgError(
+                f"Different application_types found for case: {case_id} ({application_types})"
+            )
+
+        return application_types.pop()
+
+    def has_case_only_exome_samples(self, case_id: str) -> bool:
+        """Returns True if the application type for all samples in a case is WES."""
+        application_type: str = self.get_case_application_type(case_id)
+        return application_type == AnalysisType.WHOLE_EXOME_SEQUENCING
+
     def upload_bundle_housekeeper(self, case_id: str, dry_run: bool = False) -> None:
         """Storing bundle data in Housekeeper for CASE_ID"""
         LOG.info(f"Storing bundle data in Housekeeper for {case_id}")
         bundle_data: dict = self.get_hermes_transformed_deliverables(case_id)
         bundle_result: tuple[Bundle, Version] = self.housekeeper_api.add_bundle(
             bundle_data=bundle_data
         )
```

### Comparing `cg-59.9.1/cg/meta/workflow/balsamic.py` & `cg-60.0.0/cg/meta/workflow/balsamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,24 +450,28 @@
         verified_pon = (
             self.get_verified_pon(pon_cnn=pon_cnn, panel_bed=verified_panel_bed)
             if verified_panel_bed
             else None
         )
         verified_sex: Sex = sex or self.get_verified_sex(sample_data=sample_data)
 
+        verified_exome_argument: bool = self.has_case_only_exome_samples(case_id=case_id)
+
         config_case: dict[str, str] = {
             "case_id": case_id,
             "analysis_workflow": self.workflow,
             "genome_version": genome_version,
             "sex": verified_sex,
             "panel_bed": verified_panel_bed,
             "pon_cnn": verified_pon,
             "swegen_snv": self.get_swegen_verified_path(Variants.SNV),
             "swegen_sv": self.get_swegen_verified_path(Variants.SV),
+            "exome": verified_exome_argument,
         }
+
         config_case.update(self.get_verified_samples(case_id=case_id))
         config_case.update(self.get_parsed_observation_file_paths(observations))
         (
             config_case.update(self.get_verified_gens_file_paths(sex=verified_sex))
             if not verified_panel_bed
             else None
         )
@@ -508,23 +512,14 @@
             }
             for link_object in self.status_db.get_case_by_internal_id(internal_id=case_id).links
         }
 
         self.print_sample_params(case_id=case_id, sample_data=sample_data)
         return sample_data
 
-    def get_case_application_type(self, case_id: str) -> str:
-        application_types = {
-            self.get_application_type(link_object.sample)
-            for link_object in self.status_db.get_case_by_internal_id(internal_id=case_id).links
-        }
-
-        if application_types:
-            return application_types.pop().lower()
-
     def resolve_target_bed(self, panel_bed: str | None, link_object: CaseSample) -> str | None:
         if panel_bed:
             return panel_bed
         if self.get_application_type(link_object.sample) not in self.__BALSAMIC_BED_APPLICATIONS:
             return None
         return self.get_target_bed_from_lims(link_object.case.internal_id)
 
@@ -576,20 +571,22 @@
                 "--gender": arguments.get("sex"),
                 "--genome-interval": arguments.get("genome_interval"),
                 "--genome-version": arguments.get("genome_version"),
                 "--gens-coverage-pon": arguments.get("gens_coverage_pon"),
                 "--gnomad-min-af5": arguments.get("gnomad_min_af5"),
                 "--normal-sample-name": arguments.get("normal_sample_name"),
                 "--panel-bed": arguments.get("panel_bed"),
+                "--exome": arguments.get("exome"),
                 "--pon-cnn": arguments.get("pon_cnn"),
                 "--swegen-snv": arguments.get("swegen_snv"),
                 "--swegen-sv": arguments.get("swegen_sv"),
                 "--tumor-sample-name": arguments.get("tumor_sample_name"),
                 "--umi-trim-length": arguments.get("umi_trim_length"),
-            }
+            },
+            exclude_true=True,
         )
         parameters = command + options
         self.process.run_command(parameters=parameters, dry_run=dry_run)
 
     def run_analysis(
         self,
         case_id: str,
```

### Comparing `cg-59.9.1/cg/meta/workflow/balsamic_pon.py` & `cg-60.0.0/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/balsamic_qc.py` & `cg-60.0.0/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/balsamic_umi.py` & `cg-60.0.0/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/downsample/downsample.py` & `cg-60.0.0/cg/meta/workflow/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/downsample/sbatch.py` & `cg-60.0.0/cg/meta/workflow/downsample/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/fastq.py` & `cg-60.0.0/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/fluffy.py` & `cg-60.0.0/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/microsalt/metrics_parser/models.py` & `cg-60.0.0/cg/meta/workflow/microsalt/metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/microsalt/microsalt.py` & `cg-60.0.0/cg/meta/workflow/microsalt/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/models.py` & `cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py` & `cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py` & `cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/report_generator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py` & `cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/result_logger.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/utils.py` & `cg-60.0.0/cg/meta/workflow/microsalt/quality_controller/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/microsalt/utils.py` & `cg-60.0.0/cg/meta/workflow/microsalt/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/mip.py` & `cg-60.0.0/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/mip_dna.py` & `cg-60.0.0/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/mip_rna.py` & `cg-60.0.0/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/mutant.py` & `cg-60.0.0/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/nf_handlers.py` & `cg-60.0.0/cg/meta/workflow/nf_handlers.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/prepare_fastq.py` & `cg-60.0.0/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/meta/workflow/rnafusion.py` & `cg-60.0.0/cg/meta/workflow/rnafusion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 """Module for Rnafusion Analysis API."""
 
 import logging
 from pathlib import Path
-from typing import Any
 
-from cg import resources
 from cg.constants import Workflow
-from cg.constants.constants import FileFormat, Strandedness
+from cg.constants.constants import Strandedness
 from cg.constants.nf_analysis import MULTIQC_NEXFLOW_CONFIG, RNAFUSION_METRIC_CONDITIONS
-from cg.resources import RNAFUSION_BUNDLE_FILENAMES_PATH
 from cg.exc import MissingMetrics
-from cg.io.controller import ReadFile
-from cg.io.json import read_json
 from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.cg_config import CGConfig
-from cg.models.deliverables.metric_deliverables import MetricsBase, MultiqcDataJson
-from cg.models.fastq import FastqFileMeta
+from cg.models.deliverables.metric_deliverables import MetricsBase
 from cg.models.rnafusion.rnafusion import (
     RnafusionAnalysis,
     RnafusionParameters,
     RnafusionSampleSheetEntry,
 )
-from cg.store.models import Case, Sample
+from cg.resources import RNAFUSION_BUNDLE_FILENAMES_PATH
+from cg.store.models import CaseSample, Sample
 
 LOG = logging.getLogger(__name__)
 
 
 class RnafusionAnalysisAPI(NfAnalysisAPI):
     """Handles communication between RNAFUSION processes
     and the rest of CG infrastructure."""
@@ -47,138 +42,77 @@
         self.account: str = config.rnafusion.slurm.account
         self.email: str = config.rnafusion.slurm.mail_user
         self.compute_env_base: str = config.rnafusion.compute_env
         self.revision: str = config.rnafusion.revision
         self.nextflow_binary_path: str = config.rnafusion.binary_path
 
     @property
-    def use_read_count_threshold(self) -> bool:
-        """Defines whether the threshold for adequate read count should be passed for all samples
-        when determining if the analysis for a case should be automatically started."""
-        return True
-
-    def get_deliverables_template_content(self) -> list[dict]:
-        """Return deliverables file template content."""
-        return ReadFile.get_content_from_file(
-            file_format=FileFormat.YAML,
-            file_path=self.get_bundle_filenames_path(),
-        )
+    def sample_sheet_headers(self) -> list[str]:
+        """Headers for sample sheet."""
+        return RnafusionSampleSheetEntry.headers()
+
+    @property
+    def is_params_appended_to_nextflow_config(self) -> bool:
+        """Return True if parameters should be added into the nextflow config file instead of the params file."""
+        return False
 
-    def get_nextflow_config_content(self) -> str:
+    @property
+    def is_multiple_samples_allowed(self) -> bool:
+        """Return whether the analysis supports multiple samples to be linked to the case."""
+        return False
+
+    def get_nextflow_config_content(self, case_id: str) -> str:
         """Return nextflow config content."""
         return MULTIQC_NEXFLOW_CONFIG
 
     @staticmethod
     def get_bundle_filenames_path() -> Path:
         """Return Rnafusion bundle filenames path."""
         return RNAFUSION_BUNDLE_FILENAMES_PATH
 
-    def get_sample_sheet_content_per_sample(
-        self, sample: Sample, case_id: str, strandedness: Strandedness
-    ) -> list[list[str]]:
-        """Get sample sheet content per sample."""
-        sample_metadata: list[FastqFileMeta] = self.gather_file_metadata_for_sample(sample=sample)
-        fastq_forward_read_paths: list[str] = self.extract_read_files(
-            metadata=sample_metadata, forward_read=True
+    def get_sample_sheet_content_per_sample(self, case_sample: CaseSample) -> list[list[str]]:
+        """Collect and format information required to build a sample sheet for a single sample."""
+        fastq_forward_read_paths, fastq_reverse_read_paths = self.get_paired_read_paths(
+            sample=case_sample.sample
         )
-        fastq_reverse_read_paths: list[str] = self.extract_read_files(
-            metadata=sample_metadata, reverse_read=True
-        )
-
         sample_sheet_entry = RnafusionSampleSheetEntry(
-            name=case_id,
+            name=case_sample.case.internal_id,
             fastq_forward_read_paths=fastq_forward_read_paths,
             fastq_reverse_read_paths=fastq_reverse_read_paths,
-            strandedness=strandedness,
+            strandedness=Strandedness.REVERSE,
         )
         return sample_sheet_entry.reformat_sample_content()
 
-    def get_sample_sheet_content(self, case_id: str, strandedness: Strandedness) -> list[list[Any]]:
-        """Returns content for sample sheet."""
-        case: Case = self.status_db.get_case_by_internal_id(internal_id=case_id)
-        if len(case.links) != 1:
-            raise NotImplementedError(
-                "Case objects are assumed to be related to a single sample (one link)"
-            )
-        LOG.debug("Getting sample sheet information")
-        for link in case.links:
-            content_per_sample = self.get_sample_sheet_content_per_sample(
-                sample=link.sample, case_id=case_id, strandedness=strandedness
-            )
-            return content_per_sample
-
     def get_workflow_parameters(
         self, case_id: str, genomes_base: Path | None = None
     ) -> RnafusionParameters:
         """Get Rnafusion parameters."""
-        LOG.debug("Getting parameters information")
         return RnafusionParameters(
             cluster_options=f"--qos={self.get_slurm_qos_for_case(case_id=case_id)}",
             genomes_base=genomes_base or self.get_references_path(),
-            sample_sheet_path=self.get_sample_sheet_path(case_id=case_id),
+            input=self.get_sample_sheet_path(case_id=case_id),
             outdir=self.get_case_path(case_id=case_id),
             priority=self.account,
         )
 
     def get_references_path(self, genomes_base: Path | None = None) -> Path:
         if genomes_base:
             return genomes_base.absolute()
         return Path(self.references).absolute()
 
-    def config_case(
-        self,
-        case_id: str,
-        strandedness: Strandedness,
-        genomes_base: Path,
-        dry_run: bool,
-    ) -> None:
-        """Create config files (parameters and sample sheet) for Rnafusion analysis."""
-        self.create_case_directory(case_id=case_id, dry_run=dry_run)
-        sample_sheet_content: list[list[Any]] = self.get_sample_sheet_content(
-            case_id=case_id, strandedness=strandedness
-        )
-        workflow_parameters: RnafusionParameters = self.get_workflow_parameters(
-            case_id=case_id, genomes_base=genomes_base
-        )
-        if dry_run:
-            LOG.info("Dry run: Config files will not be written")
-            return
-        self.write_sample_sheet(
-            content=sample_sheet_content,
-            file_path=self.get_sample_sheet_path(case_id=case_id),
-            header=RnafusionSampleSheetEntry.headers(),
-        )
-        self.write_params_file(case_id=case_id, workflow_parameters=workflow_parameters.dict())
-        self.write_nextflow_config(case_id=case_id)
-
-    def parse_multiqc_json_for_case(self, case_id: str) -> dict:
-        """Parse a multiqc_data.json file and returns a dictionary with metric name and metric values for a case."""
-        multiqc_json = MultiqcDataJson(
-            **read_json(file_path=self.get_multiqc_json_path(case_id=case_id))
-        )
-        metrics_values: dict = {}
-        for key in multiqc_json.report_general_stats_data:
-            if case_id in key:
-                metrics_values.update(list(key.values())[0])
-                LOG.info(f"Key: {key}, Values: {list(key.values())[0]}")
-        return metrics_values
-
-    def get_multiqc_json_metrics(self, case_id: str) -> list[MetricsBase]:
-        """Get a multiqc_data.json file and returns metrics and values formatted."""
-        case: Case = self.status_db.get_case_by_internal_id(internal_id=case_id)
-        sample_id: str = case.links[0].sample.internal_id
-        metric_values: dict = self.parse_multiqc_json_for_case(case_id=case_id)
-        metric_base_list: list = self.get_metric_base_list(
-            sample_id=sample_id, metrics_values=metric_values
-        )
-        return metric_base_list
+    def get_multiqc_search_patterns(self, case_id: str) -> dict:
+        """Return search patterns for MultiQC for Rnafusion."""
+        samples: list[Sample] = self.status_db.get_samples_by_case_id(case_id=case_id)
+        search_patterns: dict[str, str] = {case_id: sample.internal_id for sample in samples}
+        return search_patterns
 
     @staticmethod
     def ensure_mandatory_metrics_present(metrics: list[MetricsBase]) -> None:
-        """Check that all mandatory metrics are present. Raise error if missing."""
+        """Check that all mandatory metrics are present.
+        Raise: MissingMetrics if mandatory metrics are missing."""
         given_metrics: set = {metric.name for metric in metrics}
         mandatory_metrics: set = set(RNAFUSION_METRIC_CONDITIONS.keys())
         LOG.info("Mandatory Metrics Keys:")
         for key in mandatory_metrics:
             LOG.info(key)
         missing_metrics: set = mandatory_metrics.difference(given_metrics)
         if missing_metrics:
```

### Comparing `cg-59.9.1/cg/models/balsamic/config.py` & `cg-60.0.0/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/balsamic/metrics.py` & `cg-60.0.0/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/cg_config.py` & `cg-60.0.0/cg/models/cg_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from pathlib import Path
 
 from pydantic.v1 import BaseModel, EmailStr, Field
 from typing_extensions import Literal
 
 from cg.apps.coverage import ChanjoAPI
 from cg.apps.crunchy import CrunchyAPI
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
@@ -13,19 +14,22 @@
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.apps.lims import LimsAPI
 from cg.apps.loqus import LoqusdbAPI
 from cg.apps.madeline.api import MadelineAPI
 from cg.apps.mutacc_auto import MutaccAutoAPI
 from cg.apps.scout.scoutapi import ScoutAPI
 from cg.apps.tb import TrailblazerAPI
-from cg.clients.janus.api import JanusAPIClient
 from cg.clients.arnold.api import ArnoldAPIClient
+from cg.clients.janus.api import JanusAPIClient
 from cg.constants.observations import LoqusdbInstance
 from cg.constants.priority import SlurmQos
 from cg.meta.backup.pdc import PdcAPI
+from cg.services.analysis_service.analysis_service import AnalysisService
+from cg.meta.delivery.delivery import DeliveryAPI
+from cg.services.fastq_file_service.fastq_file_service import FastqFileService
 from cg.services.slurm_service.slurm_cli_service import SlurmCLIService
 from cg.services.slurm_service.slurm_service import SlurmService
 from cg.services.slurm_upload_service.slurm_upload_config import SlurmUploadConfig
 from cg.services.slurm_upload_service.slurm_upload_service import SlurmUploadService
 from cg.store.database import initialize_database
 from cg.store.store import Store
 
@@ -164,28 +168,49 @@
     conda_env: str
     mip_config: str
     workflow: str
     root: str
     script: str
 
 
-class RareDiseaseConfig(CommonAppConfig):
+class RarediseaseConfig(CommonAppConfig):
+    binary_path: str | None = None
     compute_env: str
     conda_binary: str | None = None
     conda_env: str
+    config_platform: str
+    config_params: str
+    config_resources: str
     launch_directory: str
     workflow_path: str
     profile: str
     references: str
     revision: str
     root: str
     slurm: SlurmConfig
     tower_workflow: str
 
 
+class TomteConfig(CommonAppConfig):
+    binary_path: str | None = None
+    compute_env: str
+    conda_binary: str | None = None
+    conda_env: str
+    config_platform: str
+    config_params: str
+    config_resources: str
+    workflow_path: str
+    profile: str
+    references: str
+    revision: str
+    root: str
+    slurm: SlurmConfig
+    tower_workflow: str
+
+
 class RnafusionConfig(CommonAppConfig):
     root: str
     references: str
     binary_path: str
     workflow_path: str
     conda_env: str
     compute_env: str
@@ -324,28 +349,30 @@
     scout: CommonAppConfig = None
     scout_api_: ScoutAPI = None
     tar: CommonAppConfig | None = None
     trailblazer: TrailblazerConfig = None
     trailblazer_api_: TrailblazerAPI = None
     janus: JanusConfig | None = None
     janus_api_: JanusAPIClient | None = None
+    delivery_api_: DeliveryAPI | None = None
 
     # Meta APIs that will use the apps from CGConfig
     balsamic: BalsamicConfig = None
     statina: StatinaConfig = None
     fohm: FOHMConfig | None = None
     fluffy: FluffyConfig = None
     microsalt: MicrosaltConfig = None
     gisaid: GisaidConfig = None
     mip_rd_dna: MipConfig = Field(None, alias="mip-rd-dna")
     mip_rd_rna: MipConfig = Field(None, alias="mip-rd-rna")
     mutant: MutantConfig = None
-    raredisease: RareDiseaseConfig = Field(None, alias="raredisease")
+    raredisease: RarediseaseConfig = Field(None, alias="raredisease")
     rnafusion: RnafusionConfig = Field(None, alias="rnafusion")
     taxprofiler: TaxprofilerConfig = Field(None, alias="taxprofiler")
+    tomte: TomteConfig = Field(None, alias="tomte")
 
     # These are meta APIs that gets instantiated in the code
     meta_apis: dict = {}
 
     class Config:
         arbitrary_types_allowed = True
         fields = {
@@ -526,14 +553,18 @@
         return SlurmUploadService(
             slurm_service=self.slurm_service,
             trailblazer_api=self.trailblazer_api,
             config=slurm_upload_config,
         )
 
     @property
+    def analysis_service(self) -> AnalysisService:
+        return AnalysisService(analysis_client=self.trailblazer_api)
+
+    @property
     def scout_api(self) -> ScoutAPI:
         api = self.__dict__.get("scout_api_")
         if api is None:
             LOG.debug("Instantiating scout api")
             api = ScoutAPI(config=self.dict(), slurm_upload_service=self.slurm_upload_service)
             self.scout_api_ = api
         return api
@@ -552,7 +583,25 @@
     def trailblazer_api(self) -> TrailblazerAPI:
         api = self.__dict__.get("trailblazer_api_")
         if api is None:
             LOG.debug("Instantiating trailblazer api")
             api = TrailblazerAPI(config=self.dict())
             self.trailblazer_api_ = api
         return api
+
+    @property
+    def fastq_file_service(self) -> FastqFileService:
+        return FastqFileService()
+
+    @property
+    def delivery_api(self) -> DeliveryAPI:
+        api = self.__dict__.get("delivery_api_")
+        if api is None:
+            LOG.debug("Instantiating delivery api")
+            api = DeliveryAPI(
+                delivery_path=Path(self.delivery_path),
+                fastq_file_service=self.fastq_file_service,
+                housekeeper_api=self.housekeeper_api,
+                store=self.status_db,
+            )
+            self.delivery_api_ = api
+        return api
```

### Comparing `cg-59.9.1/cg/models/compression_data.py` & `cg-60.0.0/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/deliverables/metric_deliverables.py` & `cg-60.0.0/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/demultiplex/run_parameters.py` & `cg-60.0.0/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/demultiplex/sbatch.py` & `cg-60.0.0/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/downsample/downsample_data.py` & `cg-60.0.0/cg/models/downsample/downsample_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,17 @@
             reads=multiply_by_million(self.number_of_reads),
             downsampled_to=multiply_by_million(self.number_of_reads),
             from_sample=self.original_sample.internal_id,
             tumour=self.original_sample.is_tumour,
             priority=Priority.standard,
             customer=self.original_sample.customer,
             application_version=application_version,
+            received=self.original_sample.received_at,
+            prepared_at=self.original_sample.prepared_at,
+            last_sequenced_at=self.original_sample.last_sequenced_at,
         )
         return downsampled_sample
 
     def _generate_statusdb_downsampled_case(
         self,
     ) -> Case:
         """Generate a case for the downsampled samples. The new case uses existing case data."""
```

### Comparing `cg-59.9.1/cg/models/fastq.py` & `cg-60.0.0/cg/models/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/file_data.py` & `cg-60.0.0/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/flow_cell/flow_cell.py` & `cg-60.0.0/cg/models/flow_cell/flow_cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
     @property
     def sample_sheet(self) -> SampleSheet:
         """Return sample sheet object."""
         if not self._sample_sheet_path_hk:
             raise FlowCellError("Sample sheet path has not been assigned yet")
         return self.sample_sheet_validator.get_sample_sheet_object_from_file(
-            file_path=self._sample_sheet_path_hk, bcl_converter=self.bcl_converter
+            file_path=self._sample_sheet_path_hk
         )
 
     def is_sequencing_done(self) -> bool:
         """Check if sequencing is done.
         This is indicated by that the file RTAComplete.txt exists.
         """
         LOG.info("Check if sequencing is done")
```

### Comparing `cg-59.9.1/cg/models/invoice/invoice.py` & `cg-60.0.0/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/lims/sample.py` & `cg-60.0.0/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/mip/mip_config.py` & `cg-60.0.0/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/mip/mip_metrics_deliverables.py` & `cg-60.0.0/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/mip/mip_sample_info.py` & `cg-60.0.0/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/nf_analysis.py` & `cg-60.0.0/cg/models/nf_analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 from pathlib import Path
 
 from pydantic.v1 import BaseModel, Field, conlist, validator
 
 from cg.exc import SampleSheetError
 
 
-class PipelineParameters(BaseModel):
-    clusterOptions: str = Field(..., alias="cluster_options")
-    priority: str
+class WorkflowParameters(BaseModel):
+    input: Path
+    outdir: Path
+
+
+class NfCommandArgs(BaseModel):
+    """Model for arguments and options supported."""
+
+    log: str | Path | None
+    resume: bool | None
+    profile: str | None
+    stub: bool | None
+    config: str | Path | None
+    name: str | None
+    revision: str | None
+    wait: str | None
+    id: str | None
+    with_tower: bool | None
+    use_nextflow: bool | None
+    compute_env: str | None
+    work_dir: str | Path | None
+    params_file: str | Path | None
 
 
 class NextflowSampleSheetEntry(BaseModel):
-    """Nextflow samplesheet model.
+    """Nextflow sample sheet model.
 
     Attributes:
-        name: sample name, corresponds to case_id
+        name: sample name, or case id
         fastq_forward_read_paths: list of all fastq read1 file paths corresponding to sample
         fastq_reverse_read_paths: list of all fastq read2 file paths corresponding to sample
     """
 
     name: str
     fastq_forward_read_paths: conlist(Path, min_items=1)
     fastq_reverse_read_paths: conlist(Path, min_items=1)
```

### Comparing `cg-59.9.1/cg/models/observations/input_files.py` & `cg-60.0.0/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/orders/constants.py` & `cg-60.0.0/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/orders/excel_sample.py` & `cg-60.0.0/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/orders/json_sample.py` & `cg-60.0.0/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/orders/order.py` & `cg-60.0.0/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/orders/orderform_schema.py` & `cg-60.0.0/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/orders/sample_base.py` & `cg-60.0.0/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/orders/samples.py` & `cg-60.0.0/cg/models/orders/samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,14 +279,18 @@
     original_lab_address: str
     pre_processing_method: str
     region: str
     region_code: str
     selection_criteria: str
     volume: str | None
 
+    @validator("lab_code", pre=True, always=True)
+    def set_lab_code(cls, value):
+        return "SE100 Karolinska"
+
 
 def sample_class_for(project: OrderType):
     """Get the sample class for the specified project
 
     Args:
         project     (OrderType):    Project to get sample subclass for
     Returns:
```

### Comparing `cg-59.9.1/cg/models/orders/validators/excel_sample_validators.py` & `cg-60.0.0/cg/models/orders/validators/excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/orders/validators/json_sample_validators.py` & `cg-60.0.0/cg/models/orders/validators/json_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/report/metadata.py` & `cg-60.0.0/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/report/report.py` & `cg-60.0.0/cg/models/report/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing_extensions import Annotated
 
 from cg.constants import NA_FIELD, REPORT_SUPPORTED_WORKFLOW
 from cg.models.report.sample import ApplicationModel, SampleModel
 from cg.models.report.validators import (
     get_analysis_type_as_string,
     get_date_as_string,
+    get_delivered_files_as_file_names,
     get_list_as_string,
     get_path_as_string,
     get_report_string,
 )
 
 LOG = logging.getLogger(__name__)
 
@@ -66,25 +67,29 @@
         workflow: actual workflow used for analysis; source: statusDB/analysis/workflow
         workflow_version: workflow version; source: statusDB/analysis/workflow_version
         type: analysis type carried out; source: workflow
         genome_build: build version of the genome reference; source: workflow
         variant_callers: variant-calling filters; source: workflow
         panels: list of case specific panels; source: StatusDB/family/panels
         scout_files: list of file names uploaded to Scout
+        delivered_files: list of analysis case files to be delivered
     """
 
     customer_workflow: Annotated[str, BeforeValidator(get_report_string)] = NA_FIELD
     data_delivery: Annotated[str, BeforeValidator(get_report_string)] = NA_FIELD
     workflow: Annotated[str, BeforeValidator(get_report_string)] = NA_FIELD
     workflow_version: Annotated[str, BeforeValidator(get_report_string)] = NA_FIELD
     type: Annotated[str, BeforeValidator(get_analysis_type_as_string)] = NA_FIELD
     genome_build: Annotated[str, BeforeValidator(get_report_string)] = NA_FIELD
     variant_callers: Annotated[str, BeforeValidator(get_list_as_string)] = NA_FIELD
     panels: Annotated[str, BeforeValidator(get_list_as_string)] = NA_FIELD
     scout_files: ScoutReportFiles
+    delivered_files: Annotated[
+        list[str] | str, BeforeValidator(get_delivered_files_as_file_names)
+    ] = None
 
     @model_validator(mode="after")
     def check_supported_workflow(self) -> "DataAnalysisModel":
         """Check if the report generation supports a specific workflow and analysis type."""
         if self.workflow != self.customer_workflow:
             LOG.error(
                 f"The analysis requested by the customer ({self.customer_workflow}) does not match the one "
```

### Comparing `cg-59.9.1/cg/models/report/sample.py` & `cg-60.0.0/cg/models/report/sample.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     BalsamicWGSSampleMetadataModel,
     MipDNASampleMetadataModel,
     RnafusionSampleMetadataModel,
 )
 from cg.models.report.validators import (
     get_boolean_as_string,
     get_date_as_string,
+    get_delivered_files_as_file_names,
     get_gender_as_string,
     get_prep_category_as_string,
     get_report_string,
 )
 
 
 class ApplicationModel(BaseModel):
@@ -84,14 +85,16 @@
         gender: sample gender provided by the customer; source: StatusDB/sample/sex
         source: sample type/source; source: LIMS/sample/source
         tumour: whether the sample is a tumour or normal one; source: StatusDB/sample/is_tumour
         application: analysis application model
         methods: sample processing methods model
         metadata: sample associated metrics and trending data model
         timestamps: processing timestamp attributes
+        delivered_files: list of analysis sample files to be delivered
+        delivered_fastq_files: list of fastq sample files to be delivered
     """
 
     name: Annotated[str, BeforeValidator(get_report_string)] = NA_FIELD
     id: Annotated[str, BeforeValidator(get_report_string)] = NA_FIELD
     ticket: Annotated[str, BeforeValidator(get_report_string)] = NA_FIELD
     status: Annotated[str, BeforeValidator(get_report_string)] = NA_FIELD
     gender: Annotated[str, BeforeValidator(get_gender_as_string)] = NA_FIELD
@@ -102,7 +105,13 @@
     metadata: (
         MipDNASampleMetadataModel
         | BalsamicTargetedSampleMetadataModel
         | BalsamicWGSSampleMetadataModel
         | RnafusionSampleMetadataModel
     )
     timestamps: TimestampModel
+    delivered_files: Annotated[
+        list[str] | str, BeforeValidator(get_delivered_files_as_file_names)
+    ] = None
+    delivered_fastq_files: Annotated[
+        list[str] | str, BeforeValidator(get_delivered_files_as_file_names)
+    ] = None
```

### Comparing `cg-59.9.1/cg/models/report/validators.py` & `cg-60.0.0/cg/models/report/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     NO_FIELD,
     PRECISION,
     REPORT_GENDER,
     YES_FIELD,
 )
 from cg.constants.constants import PrepCategory, Workflow
 from cg.constants.subject import Sex
+from cg.models.delivery.delivery import DeliveryFile
 from cg.models.orders.constants import OrderType
 
 LOG = logging.getLogger(__name__)
 
 
 def get_report_string(value: Any) -> str:
     """Return report adapted string."""
@@ -48,14 +49,19 @@
 
 
 def get_list_as_string(value: list[str] | None) -> str:
     """Return list elements as comma separated individual string values."""
     return ", ".join(v for v in value) if value else NA_FIELD
 
 
+def get_delivered_files_as_file_names(delivery_files: list[DeliveryFile] | None) -> list[str] | str:
+    """Return a list of validated file names given a list of delivery files."""
+    return [file.destination_path.name for file in delivery_files] if delivery_files else NA_FIELD
+
+
 def get_path_as_string(file_path: str | None) -> str:
     """Return a report validated file name."""
     return Path(file_path).name if file_path and Path(file_path).is_file() else NA_FIELD
 
 
 def get_gender_as_string(gender: Sex | None) -> str:
     """Return a report adapted gender."""
```

### Comparing `cg-59.9.1/cg/models/rnafusion/rnafusion.py` & `cg-60.0.0/cg/models/rnafusion/rnafusion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from pydantic.v1 import BaseModel, Field
 
 from cg.constants.constants import Strandedness
 from cg.models.analysis import AnalysisModel
-from cg.models.nf_analysis import NextflowSampleSheetEntry, PipelineParameters
+from cg.models.nf_analysis import NextflowSampleSheetEntry, WorkflowParameters
 
 
 class RnafusionQCMetrics(BaseModel):
     """RNAfusion QC metrics."""
 
     after_filtering_gc_content: float | None
     after_filtering_q20_rate: float | None
@@ -21,46 +21,27 @@
     pct_ribosomal_bases: float | None
     pct_surviving: float | None
     pct_duplication: float | None
     read_pairs_examined: float | None
     uniquely_mapped_percent: float | None
 
 
-class RnafusionParameters(PipelineParameters):
+class RnafusionParameters(WorkflowParameters):
     """Rnafusion parameters."""
 
     genomes_base: Path
-    input: Path = Field(..., alias="sample_sheet_path")
-    outdir: Path
     all: bool = False
     arriba: bool = True
     cram: str = "arriba,starfusion"
     fastp_trim: bool = True
     fusioncatcher: bool = True
     starfusion: bool = True
     trim_tail: int = 50
-
-
-class CommandArgs(BaseModel):
-    """Model for arguments and options supported."""
-
-    log: str | Path | None
-    resume: bool | None
-    profile: str | None
-    stub: bool | None
-    config: str | Path | None
-    name: str | None
-    revision: str | None
-    wait: str | None
-    id: str | None
-    with_tower: bool | None
-    use_nextflow: bool | None
-    compute_env: str | None
-    work_dir: str | Path | None
-    params_file: str | Path | None
+    clusterOptions: str = Field(..., alias="cluster_options")
+    priority: str
 
 
 class RnafusionSampleSheetEntry(NextflowSampleSheetEntry):
     """Rnafusion sample sheet model."""
 
     strandedness: Strandedness
```

### Comparing `cg-59.9.1/cg/models/scout/scout_load_config.py` & `cg-60.0.0/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/slurm/sbatch.py` & `cg-60.0.0/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/models/taxprofiler/taxprofiler.py` & `cg-60.0.0/cg/models/taxprofiler/taxprofiler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 from pathlib import Path
-
-from pydantic import Field, BaseModel
+from pydantic.v1 import BaseModel, Field
 
 from cg.constants.sequencing import SequencingPlatform
-from cg.models.nf_analysis import NextflowSampleSheetEntry, PipelineParameters
+from cg.models.nf_analysis import NextflowSampleSheetEntry, WorkflowParameters
 
 
 class TaxprofilerQCMetrics(BaseModel):
     """Taxprofiler QC metrics."""
 
     after_filtering_total_reads: float | None
     reads_mapped: float | None
     before_filtering_total_reads: float | None
     paired_aligned_none: float | None
 
 
-class TaxprofilerParameters(PipelineParameters):
+class TaxprofilerParameters(WorkflowParameters):
     """Model for Taxprofiler parameters."""
 
-    input: Path = Field(..., alias="sample_sheet_path")
-    outdir: Path
     databases: Path
     save_preprocessed_reads: bool = True
     perform_shortread_qc: bool = True
     perform_shortread_complexityfilter: bool = True
     save_complexityfiltered_reads: bool = True
     perform_shortread_hostremoval: bool = True
     hostremoval_reference: Path
     save_hostremoval_index: bool = True
     save_hostremoval_mapped: bool = True
     save_hostremoval_unmapped: bool = True
     perform_runmerging: bool = True
     run_kraken2: bool = True
     kraken2_save_reads: bool = True
-    kraken2_save_readclassification: bool = True
+    kraken2_save_readclassifications: bool = True
     run_bracken: bool = True
     run_centrifuge: bool = True
     centrifuge_save_reads: bool = True
     run_krona: bool = True
     run_profile_standardisation: bool = True
+    clusterOptions: str = Field(..., alias="cluster_options")
+    priority: str
 
 
 class TaxprofilerSampleSheetEntry(NextflowSampleSheetEntry):
     """Taxprofiler sample model is used when building the sample sheet."""
 
     instrument_platform: SequencingPlatform
     run_accession: str
```

### Comparing `cg-59.9.1/cg/models/workflow/mutant.py` & `cg-60.0.0/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/resources/__init__.py` & `cg-60.0.0/cg/resources/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 from pathlib import Path
 
 import pkg_resources
 
-VALID_INDEXES_FILE: str = Path("resources", "20181012_Indices.csv").as_posix()
+from cg.constants import FileExtensions
 
-VALID_INDEXES_PATH: Path = Path(pkg_resources.resource_filename("cg", VALID_INDEXES_FILE))
+RNAFUSION_BUNDLE_FILENAMES: str = (
+    Path("resources", "rnafusion_bundle_filenames").with_suffix(FileExtensions.YAML).as_posix()
+)
 
-RNAFUSION_BUNDLE_FILENAMES: str = Path("resources", "rnafusion_bundle_filenames.csv").as_posix()
+TAXPROFILER_BUNDLE_FILENAMES: str = (
+    Path("resources", "taxprofiler_bundle_filenames").with_suffix(FileExtensions.YAML).as_posix()
+)
 
-TAXPROFILER_BUNDLE_FILENAMES: str = Path("resources", "taxprofiler_bundle_filenames.csv").as_posix()
+TOMTE_BUNDLE_FILENAMES: str = (
+    Path("resources", "tomte_bundle_filenames").with_suffix(FileExtensions.YAML).as_posix()
+)
 
 RNAFUSION_BUNDLE_FILENAMES_PATH: Path = Path(
     pkg_resources.resource_filename("cg", RNAFUSION_BUNDLE_FILENAMES)
 )
 
 TAXPROFILER_BUNDLE_FILENAMES_PATH: Path = Path(
     pkg_resources.resource_filename("cg", TAXPROFILER_BUNDLE_FILENAMES)
 )
+
+TOMTE_BUNDLE_FILENAMES_PATH: Path = Path(
+    pkg_resources.resource_filename("cg", TOMTE_BUNDLE_FILENAMES)
+)
```

### Comparing `cg-59.9.1/cg/resources/rnafusion_bundle_filenames.csv` & `cg-60.0.0/cg/resources/rnafusion_bundle_filenames.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -96,8 +96,42 @@
   tag: multiqc-json
 - format: yml
   id: CASEID
   path: PATHTOCASE/CASEID_metrics_deliverables.yaml
   path_index: ~
   step: qc-metrics
   tag: qc-metrics
-
+- format: json
+  id: CASEID
+  path: PATHTOCASE/multiqc/multiqc_data/multiqc_picard_RnaSeqMetrics.json
+  path_index: ~
+  step: multiqc
+  tag: multiqc-picard-rnaseq
+- format: json
+  id: CASEID
+  path: PATHTOCASE/multiqc/multiqc_data/multiqc_fastp.json
+  path_index: ~
+  step: multiqc
+  tag: multiqc-fastp
+- format: json
+  id: CASEID
+  path: PATHTOCASE/multiqc/multiqc_data/multiqc_general_stats.json
+  path_index: ~
+  step: multiqc
+  tag: multiqc-general-stats
+- format: json
+  id: CASEID
+  path: PATHTOCASE/multiqc/multiqc_data/multiqc_picard_dups.json
+  path_index: ~
+  step: multiqc
+  tag: multiqc-picard-duplicates
+- format: json
+  id: CASEID
+  path: PATHTOCASE/multiqc/multiqc_data/multiqc_star.json
+  path_index: ~
+  step: multiqc
+  tag: multiqc-star
+- format: json
+  id: CASEID
+  path: PATHTOCASE/multiqc/multiqc_data/multiqc_picard_insertSize.json
+  step: multiqc
+  tag: multiqc-picard-insert-size
```

### Comparing `cg-59.9.1/cg/resources/taxprofiler_bundle_filenames.csv` & `cg-60.0.0/cg/resources/taxprofiler_bundle_filenames.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -48,20 +48,14 @@
   tag: centrifuge_report
 - format: html
   id: CASEID
   path: PATHTOCASE/multiqc/multiqc_report.html
   path_index: ~
   step: report
   tag: multiqc-html
-- format: csv
-  id: CASEID
-  path: PATHTOCASE/pipeline_info/samplesheet.valid.csv
-  path_index: ~
-  step: samplesheet-valid
-  tag: samplesheet-valid
 - format: yml
   id: CASEID
   path: PATHTOCASE/pipeline_info/software_versions.yml
   path_index: ~
   step: software-versions
   tag: software-versions
 - format: json
```

### Comparing `cg-59.9.1/cg/server/admin.py` & `cg-60.0.0/cg/server/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,26 +182,26 @@
 
 
 class ApplicationLimitationsView(BaseView):
     """Admin view for Model.ApplicationLimitations."""
 
     column_list = (
         "application",
-        "pipeline",
+        "workflow",
         "limitations",
         "comment",
         "created_at",
         "updated_at",
     )
     column_formatters = {"application": ApplicationView.view_application_link}
-    column_filters = ["application.tag", "pipeline"]
+    column_filters = ["application.tag", "workflow"]
     column_searchable_list = ["application.tag"]
     column_editable_list = ["comment"]
     form_excluded_columns = ["created_at", "updated_at"]
-    form_extra_fields = {"pipeline": SelectEnumField(enum_class=Workflow)}
+    form_extra_fields = {"workflow": SelectEnumField(enum_class=Workflow)}
     create_modal = True
     edit_modal = True
 
 
 class BedView(BaseView):
     """Admin view for Model.Bed"""
 
@@ -444,14 +444,24 @@
     """Admin view for Model.Organism"""
 
     column_default_sort = ("created_at", True)
     column_editable_list = ["internal_id", "name", "reference_genome", "comment"]
     column_searchable_list = ["internal_id", "name", "reference_genome"]
 
 
+class OrderView(BaseView):
+    """Admin view for Model.Order"""
+
+    column_default_sort = ("order_date", True)
+    column_editable_list = ["is_delivered"]
+    column_display_pk = True
+    create_modal = True
+    edit_modal = True
+
+
 class PanelView(BaseView):
     """Admin view for Model.Panel"""
 
     column_editable_list = ["current_version", "name"]
     column_filters = ["customer.internal_id"]
     column_searchable_list = ["customer.internal_id", "name", "abbrev"]
     create_modal = True
@@ -469,15 +479,14 @@
 
 
 class SampleView(BaseView):
     """Admin view for Model.Sample"""
 
     column_exclude_list = [
         "age_at_sampling",
-        "invoiced_at",
         "_phenotype_groups",
         "_phenotype_terms",
     ]
     column_default_sort = ("created_at", True)
     column_editable_list = [
         "comment",
         "downsampled_to",
@@ -500,17 +509,15 @@
         "original_ticket",
     ]
     form_excluded_columns = [
         "age_at_sampling",
         "deliveries",
         "father_links",
         "flowcells",
-        "invoiced_at",
         "invoice",
-        "is_external",
         "_phenotype_groups",
         "_phenotype_terms",
         "links",
         "mother_links",
     ]
 
     @staticmethod
```

### Comparing `cg-59.9.1/cg/server/api.py` & `cg-60.0.0/cg/server/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,31 +23,38 @@
 from cg.constants import ANALYSIS_SOURCES, METAGENOME_SOURCES
 from cg.constants.constants import FileFormat
 from cg.exc import (
     CaseNotFoundError,
     OrderError,
     OrderExistsError,
     OrderFormError,
+    OrderMismatchError,
+    OrderNotDeliverableError,
+    OrderNotFoundError,
     TicketCreationError,
 )
 from cg.io.controller import WriteStream
 from cg.meta.orders import OrdersAPI
 from cg.meta.orders.ticket_handler import TicketHandler
 from cg.models.orders.order import OrderIn, OrderType
 from cg.models.orders.orderform_schema import Orderform
-from cg.server.dto.delivery_message_response import DeliveryMessageResponse
+from cg.server.dto.delivery_message.delivery_message_request import (
+    DeliveryMessageRequest,
+)
+from cg.server.dto.delivery_message.delivery_message_response import (
+    DeliveryMessageResponse,
+)
+from cg.server.dto.orders.order_delivery_update_request import OrderDeliveredUpdateRequest
+from cg.server.dto.orders.order_patch_request import OrderDeliveredPatch
 from cg.server.dto.orders.orders_request import OrdersRequest
 from cg.server.dto.orders.orders_response import Order, OrdersResponse
-from cg.server.ext import db, lims, osticket, order_service
-from cg.services.delivery_message.delivery_message_service import DeliveryMessageService
-from cg.services.orders.order_service.exceptions import OrderNotFoundError
+from cg.server.ext import db, delivery_message_service, lims, order_service, osticket
 from cg.store.models import (
     Analysis,
     Application,
-    ApplicationLimitations,
     Case,
     Customer,
     Flowcell,
     Pool,
     Sample,
     SampleLaneSequencingMetrics,
     User,
@@ -212,19 +219,33 @@
     if case is None:
         return abort(HTTPStatus.NOT_FOUND)
     if not g.current_user.is_admin and (case.customer not in g.current_user.customers):
         return abort(HTTPStatus.FORBIDDEN)
     return jsonify(**case.to_dict(links=True, analyses=True))
 
 
+@BLUEPRINT.route("/cases/delivery_message", methods=["GET"])
+def get_cases_delivery_message():
+    delivery_message_request = DeliveryMessageRequest.model_validate(request.args)
+    try:
+        response: DeliveryMessageResponse = delivery_message_service.get_cases_message(
+            delivery_message_request
+        )
+        return jsonify(response.model_dump()), HTTPStatus.OK
+    except (CaseNotFoundError, OrderMismatchError) as error:
+        return jsonify({"error": str(error)}), HTTPStatus.BAD_REQUEST
+
+
 @BLUEPRINT.route("/cases/<case_id>/delivery_message", methods=["GET"])
 def get_case_delivery_message(case_id: str):
-    service = DeliveryMessageService(db)
+    delivery_message_request = DeliveryMessageRequest(case_ids=[case_id])
     try:
-        response: DeliveryMessageResponse = service.get_delivery_message(case_id)
+        response: DeliveryMessageResponse = delivery_message_service.get_cases_message(
+            delivery_message_request
+        )
         return jsonify(response.model_dump()), HTTPStatus.OK
     except CaseNotFoundError as error:
         return jsonify({"error": str(error)}), HTTPStatus.BAD_REQUEST
 
 
 @BLUEPRINT.route("/families_in_collaboration")
 def parse_families_in_collaboration():
@@ -466,24 +487,22 @@
     """Return an application tag."""
     application: Application = db.get_application_by_tag(tag=tag)
     if not application:
         return abort(make_response(jsonify(message="Application not found"), HTTPStatus.NOT_FOUND))
     return jsonify(**application.to_dict())
 
 
-@BLUEPRINT.route("/applications/<tag>/pipeline_limitations")
+@BLUEPRINT.route("/applications/<tag>/workflow_limitations")
 @is_public
-def get_application_pipeline_limitations(tag: str):
-    """Return application pipeline specific limitations."""
-    application_limitations: list[ApplicationLimitations] = db.get_application_limitations_by_tag(
-        tag
-    )
-    if not application_limitations:
+def get_application_workflow_limitations(tag: str):
+    """Return application workflow specific limitations."""
+    if application_limitations := db.get_application_limitations_by_tag(tag):
+        return jsonify([limitation.to_dict() for limitation in application_limitations])
+    else:
         return jsonify(message="Application limitations not found"), HTTPStatus.NOT_FOUND
-    return jsonify([limitation.to_dict() for limitation in application_limitations])
 
 
 @BLUEPRINT.route("/orders")
 def get_orders():
     """Return the latest orders."""
     data = OrdersRequest.model_validate(request.args.to_dict())
     response: OrdersResponse = order_service.get_orders(data)
@@ -497,14 +516,49 @@
         response: Order = order_service.get_order(order_id)
         response_dict: dict = response.model_dump()
         return make_response(response_dict)
     except OrderNotFoundError as error:
         return make_response(jsonify(error=str(error)), HTTPStatus.NOT_FOUND)
 
 
+@BLUEPRINT.route("/orders/<order_id>/delivered", methods=["PATCH"])
+def set_order_delivered(order_id: int):
+    try:
+        request_data = OrderDeliveredPatch.model_validate(request.json)
+        delivered: bool = request_data.delivered
+        response_data: Order = order_service.set_delivery(order_id=order_id, delivered=delivered)
+        return jsonify(response_data.model_dump()), HTTPStatus.OK
+    except OrderNotFoundError as error:
+        return jsonify(error=str(error)), HTTPStatus.NOT_FOUND
+
+
+@BLUEPRINT.route("/orders/<order_id>/update-delivery-status", methods=["POST"])
+def update_order_delivered(order_id: int):
+    """Update the delivery status of an order based on the number of delivered analyses."""
+    try:
+        request_data = OrderDeliveredUpdateRequest.model_validate(request.json)
+        delivered_analyses: int = request_data.delivered_analyses_count
+        order_service.update_delivered(order_id=order_id, delivered_analyses=delivered_analyses)
+    except OrderNotFoundError as error:
+        return jsonify(error=str(error)), HTTPStatus.NOT_FOUND
+
+
+@BLUEPRINT.route("/orders/<order_id>/delivery_message")
+def get_delivery_message_for_order(order_id: int):
+    """Return the delivery message for an order."""
+    try:
+        response: DeliveryMessageResponse = delivery_message_service.get_order_message(order_id)
+        response_dict: dict = response.model_dump()
+        return make_response(response_dict)
+    except OrderNotDeliverableError as error:
+        return make_response(jsonify(error=str(error)), HTTPStatus.PRECONDITION_FAILED)
+    except OrderNotFoundError as error:
+        return make_response(jsonify(error=str(error))), HTTPStatus.NOT_FOUND
+
+
 @BLUEPRINT.route("/orderform", methods=["POST"])
 def parse_orderform():
     """Parse an orderform/JSON export."""
     input_file = request.files.get("file")
     filename = secure_filename(input_file.filename)
 
     error_message: str
```

### Comparing `cg-59.9.1/cg/server/app.py` & `cg-60.0.0/cg/server/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Case,
     CaseSample,
     Collaboration,
     Customer,
     Delivery,
     Flowcell,
     Invoice,
+    Order,
     Organism,
     Panel,
     Pool,
     Sample,
     SampleLaneSequencingMetrics,
     User,
 )
@@ -109,14 +110,15 @@
     ext.admin.add_view(admin.ApplicationVersionView(ApplicationVersion, ext.db.session))
     ext.admin.add_view(admin.ApplicationLimitationsView(ApplicationLimitations, ext.db.session))
     ext.admin.add_view(admin.BedView(Bed, ext.db.session))
     ext.admin.add_view(admin.BedVersionView(BedVersion, ext.db.session))
     ext.admin.add_view(admin.CustomerView(Customer, ext.db.session))
     ext.admin.add_view(admin.CollaborationView(Collaboration, ext.db.session))
     ext.admin.add_view(admin.OrganismView(Organism, ext.db.session))
+    ext.admin.add_view(admin.OrderView(Order, ext.db.session))
     ext.admin.add_view(admin.PanelView(Panel, ext.db.session))
     ext.admin.add_view(admin.UserView(User, ext.db.session))
     ext.admin.add_view(
         admin.SampleLaneSequencingMetricsView(SampleLaneSequencingMetrics, ext.db.session)
     )
 
     # Business data views
```

### Comparing `cg-59.9.1/cg/server/config.py` & `cg-60.0.0/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/server/dto/orders/orders_request.py` & `cg-60.0.0/cg/server/dto/orders/orders_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 
 
 class OrdersRequest(BaseModel):
     page_size: int | None = Field(alias="pageSize", default=50)
     page: int | None = 1
     sort_field: OrderSortField | None = Field(alias="sortField", default=OrderSortField.ORDER_DATE)
     sort_order: SortOrder | None = Field(alias="sortOrder", default=SortOrder.DESC)
+    search: str | None = None
     workflow: str | None = None
+    delivered: bool | None = None
```

### Comparing `cg-59.9.1/cg/server/ext.py` & `cg-60.0.0/cg/server/ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 
 from flask_admin import Admin
 from flask_cors import CORS
 from flask_wtf.csrf import CSRFProtect
 
 from cg.apps.lims import LimsAPI
 from cg.apps.osticket import OsTicket
-from cg.services.orders.order_status_service.order_status_service import OrderStatusService
-from cg.store.database import initialize_database
-from cg.store.store import Store
 from cg.apps.tb.api import TrailblazerAPI
+from cg.services.delivery_message.delivery_message_service import DeliveryMessageService
 from cg.services.orders.order_service.order_service import OrderService
+from cg.services.orders.order_status_service.order_summary_service import (
+    OrderSummaryService,
+)
+from cg.store.database import initialize_database
+from cg.store.store import Store
 
 
 class FlaskLims(LimsAPI):
     def __init__(self, app=None):
         if app:
             self.init_app(app)
 
@@ -71,9 +74,10 @@
 csrf = CSRFProtect()
 db = FlaskStore()
 
 admin = Admin(name="Clinical Genomics")
 lims = FlaskLims()
 osticket = OsTicket()
 analysis_client = AnalysisClient()
-summary_service = OrderStatusService(store=db, analysis_client=analysis_client)
+delivery_message_service = DeliveryMessageService(store=db, trailblazer_api=analysis_client)
+summary_service = OrderSummaryService(store=db, analysis_client=analysis_client)
 order_service = OrderService(store=db, status_service=summary_service)
```

### Comparing `cg-59.9.1/cg/server/invoices/templates/invoices/index.html` & `cg-60.0.0/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/server/invoices/templates/invoices/invoice.html` & `cg-60.0.0/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/server/invoices/templates/invoices/layout.html` & `cg-60.0.0/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/server/invoices/templates/invoices/new.html` & `cg-60.0.0/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/server/invoices/views.py` & `cg-60.0.0/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/services/delivery_message/messages/__init__.py` & `cg-60.0.0/cg/services/delivery_message/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/services/delivery_message/messages/analysis_scout_message.py` & `cg-60.0.0/cg/services/delivery_message/messages/fastq_analysis_scout_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,38 @@
 from cg.services.delivery_message.messages.delivery_message import DeliveryMessage
-from cg.services.delivery_message.messages.utils import get_fastq_delivery_path, get_scout_link
+from cg.services.delivery_message.messages.utils import (
+    get_fastq_delivery_path,
+    get_scout_link,
+)
 from cg.store.models import Case
 
 
-class AnalysisScoutMessage(DeliveryMessage):
-    def create_message(self, case: Case) -> str:
-        scout_link: str = get_scout_link(case)
-        delivery_path: str = get_fastq_delivery_path(case)
-        return (
-            f"Hello,\n\n "
-            f"The results have been uploaded to Scout for the following case:\n\n"
-            f"{scout_link}\n\n"
-            f"The analysis files are currently being uploaded to your inbox on Caesar:\n\n"
-            f"{delivery_path}"
-        )
+def get_case_message(case: Case) -> str:
+    scout_link: str = get_scout_link(case)
+    delivery_path: str = get_fastq_delivery_path(case)
+    return (
+        f"Hello,\n\n"
+        f"The analysis has been uploaded to Scout for the following case:\n\n"
+        f"{scout_link}\n\n"
+        f"The fastq and analysis files are currently being uploaded to your inbox on Caesar:\n\n"
+        f"{delivery_path}"
+    )
+
+
+def get_cases_message(cases: list[Case]) -> str:
+    scout_links: list[str] = [get_scout_link(case) for case in cases]
+    scout_links_row_separated: str = "\n".join(scout_links)
+    delivery_path: str = get_fastq_delivery_path(cases[0])
+    return (
+        f"Hello,\n\n"
+        f"The analyses have been uploaded to Scout for the following cases:\n\n"
+        f"{scout_links_row_separated}\n\n"
+        f"The fastq and analysis files are currently being uploaded to your inbox on Caesar:\n\n"
+        f"{delivery_path}"
+    )
+
+
+class FastqAnalysisScoutMessage(DeliveryMessage):
+    def create_message(self, cases: list[Case]) -> str:
+        if len(cases) == 1:
+            return get_case_message(cases[0])
+        return get_cases_message(cases)
```

### Comparing `cg-59.9.1/cg/services/delivery_message/messages/covid_message.py` & `cg-60.0.0/cg/services/delivery_message/messages/covid_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
     get_fastq_delivery_path,
     get_pangolin_delivery_path,
 )
 from cg.store.models import Case
 
 
 class CovidMessage(DeliveryMessage):
-    def create_message(self, case: Case) -> str:
-        delivery_path: str = get_fastq_delivery_path(case)
-        pangolin_delivery_path: str = get_pangolin_delivery_path(case)
+    def create_message(self, cases: list[Case]) -> str:
+        delivery_path: str = get_fastq_delivery_path(cases[0])
+        pangolin_delivery_path: str = get_pangolin_delivery_path(cases[0])
         return (
-            f"Hello,\n\n "
+            f"Hello,\n\n"
             f"The analysis is now complete.\n\n"
-            f"The result files are being uploaded on caesar at:\n\n"
+            f"The result files are being uploaded to Caesar at:\n\n"
             f"{delivery_path}\n\n"
             f"and the .csv files with pangolin-type have been sent to\n\n"
             f"{pangolin_delivery_path}"
         )
```

### Comparing `cg-59.9.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py` & `cg-60.0.0/cg/services/delivery_message/messages/fastq_scout_message.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,38 @@
 from cg.services.delivery_message.messages.delivery_message import DeliveryMessage
-from cg.services.delivery_message.messages.utils import get_fastq_delivery_path, get_scout_link
+from cg.services.delivery_message.messages.utils import (
+    get_fastq_delivery_path,
+    get_scout_link,
+)
 from cg.store.models import Case
 
 
-class FastqAnalysisScoutMessage(DeliveryMessage):
-    def create_message(self, case: Case) -> str:
-        scout_link: str = get_scout_link(case)
-        delivery_path: str = get_fastq_delivery_path(case)
-        return (
-            f"Hello,\n\n "
-            f"The results have been uploaded to Scout for the following case:\n\n"
-            f"{scout_link}\n\n"
-            f"The fastq and analysis files are currently being uploaded to your inbox on Caesar:\n\n"
-            f"{delivery_path}"
-        )
+def get_case_message(case: Case) -> str:
+    scout_link: str = get_scout_link(case)
+    delivery_path: str = get_fastq_delivery_path(case)
+    return (
+        f"Hello,\n\n"
+        f"The analysis has been uploaded to Scout for the following case:\n\n"
+        f"{scout_link}\n\n"
+        f"The fastq files are currently being uploaded to your inbox on Caesar:\n\n"
+        f"{delivery_path}"
+    )
+
+
+def get_cases_message(cases: list[Case]) -> str:
+    scout_links: list[str] = [get_scout_link(case) for case in cases]
+    scout_links_row_separated: str = "\n".join(scout_links)
+    delivery_path: str = get_fastq_delivery_path(cases[0])
+    return (
+        f"Hello,\n\n "
+        f"The analyses have been uploaded to Scout for the following cases:\n\n"
+        f"{scout_links_row_separated}\n\n"
+        f"The fastq files are currently being uploaded to your inbox on Caesar:\n\n"
+        f"{delivery_path}"
+    )
+
+
+class FastqScoutMessage(DeliveryMessage):
+    def create_message(self, cases: list[Case]) -> str:
+        if len(cases) == 1:
+            return get_case_message(cases[0])
+        return get_cases_message(cases)
```

### Comparing `cg-59.9.1/cg/services/delivery_message/messages/fastq_message.py` & `cg-60.0.0/cg/services/delivery_message/messages/fastq_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from cg.services.delivery_message.messages.delivery_message import DeliveryMessage
 from cg.services.delivery_message.messages.utils import get_fastq_delivery_path
 from cg.store.models import Case
 
 
 class FastqMessage(DeliveryMessage):
-    def create_message(self, case: Case) -> str:
-        delivery_path: str = get_fastq_delivery_path(case)
+    def create_message(self, cases: list[Case]) -> str:
+        delivery_path: str = get_fastq_delivery_path(cases[0])
         return (
-            f"Hello,\n\n "
+            f"Hello,\n\n"
             f"The fastq files for this order have been uploaded to your inbox on Caesar at:\n\n"
             f"{delivery_path}"
         )
```

### Comparing `cg-59.9.1/cg/services/delivery_message/messages/fastq_scout_message.py` & `cg-60.0.0/cg/services/delivery_message/messages/analysis_scout_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,38 @@
 from cg.services.delivery_message.messages.delivery_message import DeliveryMessage
-from cg.services.delivery_message.messages.utils import get_fastq_delivery_path, get_scout_link
+from cg.services.delivery_message.messages.utils import (
+    get_fastq_delivery_path,
+    get_scout_link,
+)
 from cg.store.models import Case
 
 
-class FastqScoutMessage(DeliveryMessage):
-    def create_message(self, case: Case) -> str:
-        scout_link: str = get_scout_link(case)
-        delivery_path: str = get_fastq_delivery_path(case)
-        return (
-            f"Hello,\n\n "
-            f"The results have been uploaded to Scout for the following case::\n\n"
-            f"{scout_link}\n\n"
-            f"The fastq files are currently being uploaded to your inbox on Caesar:\n\n"
-            f"{delivery_path}"
-        )
+def get_case_message(case: Case) -> str:
+    scout_link: str = get_scout_link(case)
+    delivery_path: str = get_fastq_delivery_path(case)
+    return (
+        f"Hello,\n\n"
+        f"The analysis has been uploaded to Scout for the following case:\n\n"
+        f"{scout_link}\n\n"
+        f"The analysis files are currently being uploaded to your inbox on Caesar:\n\n"
+        f"{delivery_path}"
+    )
+
+
+def get_cases_message(cases: list[Case]) -> str:
+    scout_links: list[str] = [get_scout_link(case) for case in cases]
+    scout_links_row_separated: str = "\n".join(scout_links)
+    delivery_path: str = get_fastq_delivery_path(cases[0])
+    return (
+        f"Hello,\n\n"
+        f"The analyses have been uploaded to Scout for the following cases:\n\n"
+        f"{scout_links_row_separated}\n\n"
+        f"The analysis files are currently being uploaded to your inbox on Caesar:\n\n"
+        f"{delivery_path}"
+    )
+
+
+class AnalysisScoutMessage(DeliveryMessage):
+    def create_message(self, cases: list[Case]) -> str:
+        if len(cases) == 1:
+            return get_case_message(cases[0])
+        return get_cases_message(cases)
```

### Comparing `cg-59.9.1/cg/services/delivery_message/messages/microsalt_mwr_message.py` & `cg-60.0.0/cg/services/delivery_message/messages/microsalt_mwr_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from cg.services.delivery_message.messages.delivery_message import DeliveryMessage
 from cg.services.delivery_message.messages.utils import get_fastq_delivery_path
 from cg.store.models import Case
 
 
 class MicrosaltMwrMessage(DeliveryMessage):
-    def create_message(self, case: Case) -> str:
-        delivery_path: str = get_fastq_delivery_path(case)
+    def create_message(self, cases: list[Case]) -> str:
+        delivery_path: str = get_fastq_delivery_path(cases[0])
         return (
-            f"Hello,\n\n "
+            f"Hello,\n\n"
             f"The analysis is now complete and the fastq files are being uploaded to:\n\n"
             f"{delivery_path} \n\n"
             "The QC and Typing reports can be found attached."
         )
```

### Comparing `cg-59.9.1/cg/services/delivery_message/messages/microsalt_mwx_message.py` & `cg-60.0.0/cg/services/delivery_message/messages/microsalt_mwx_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from cg.services.delivery_message.messages.delivery_message import DeliveryMessage
 from cg.services.delivery_message.messages.utils import get_fastq_delivery_path
 from cg.store.models import Case
 
 
 class MicrosaltMwxMessage(DeliveryMessage):
-    def create_message(self, case: Case) -> str:
-        delivery_path: str = get_fastq_delivery_path(case)
+    def create_message(self, cases: list[Case]) -> str:
+        delivery_path: str = get_fastq_delivery_path(cases[0])
         return (
-            f"Hello,\n\n "
+            f"Hello,\n\n"
             f"The analysis is now complete and the fastq files are being uploaded to:\n\n"
             f"{delivery_path} \n\n"
             "The QC report can be found attached."
         )
```

### Comparing `cg-59.9.1/cg/services/delivery_message/messages/utils.py` & `cg-60.0.0/cg/services/delivery_message/messages/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,10 +14,13 @@
 
 
 def get_pangolin_delivery_path(case: Case) -> str:
     customer_id: str = case.customer.internal_id
     return f"/home/{customer_id}/inbox/wwLab_automatisk_hamtning"
 
 
-def get_statina_link(case: Case) -> str:
-    batch_id: str = case.name.split("-")[1]
+def get_batch_id_for_case(case: Case) -> str:
+    return case.name.split("-")[1]
+
+
+def get_statina_link(batch_id: str) -> str:
     return f"https://statina.clinicalgenomics.se/batches/{batch_id}"
```

### Comparing `cg-59.9.1/cg/services/fastq_file_service/fastq_file_service.py` & `cg-60.0.0/cg/services/fastq_file_service/fastq_file_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,38 @@
+import logging
 from pathlib import Path
 
 from cg.services.fastq_file_service.utils import (
     concatenate_forward_reads,
     concatenate_reverse_reads,
     remove_raw_fastqs,
 )
 
+LOG = logging.getLogger(__name__)
+
 
 class FastqFileService:
 
     def concatenate(
         self,
         fastq_directory: Path,
-        forward_output: Path,
-        reverse_output: Path,
+        forward_output_path: Path,
+        reverse_output_path: Path,
         remove_raw: bool = False,
     ):
         temp_forward: Path | None = concatenate_forward_reads(fastq_directory)
         temp_reverse: Path | None = concatenate_reverse_reads(fastq_directory)
 
         if remove_raw:
             remove_raw_fastqs(
                 fastq_directory=fastq_directory,
                 forward_file=temp_forward,
                 reverse_file=temp_reverse,
             )
 
         if temp_forward:
-            temp_forward.rename(forward_output)
+            LOG.info(f"Concatenated forward reads to {forward_output_path}")
+            temp_forward.rename(forward_output_path)
 
         if temp_reverse:
-            temp_reverse.rename(reverse_output)
+            LOG.info(f"Concatenated reverse reads to {reverse_output_path}")
+            temp_reverse.rename(reverse_output_path)
```

### Comparing `cg-59.9.1/cg/services/fastq_file_service/utils.py` & `cg-60.0.0/cg/services/fastq_file_service/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
 import re
 import shutil
 import uuid
 
 from cg.services.fastq_file_service.exceptions import ConcatenationError
+from cg.constants.constants import ReadDirection
+from cg.constants import FileExtensions
 
 
 def concatenate_forward_reads(directory: Path) -> Path | None:
     fastqs: list[Path] = get_forward_read_fastqs(directory)
     if not fastqs:
         return
     output_file: Path = get_new_unique_file(directory)
@@ -24,27 +26,27 @@
     concatenate(input_files=fastqs, output_file=file)
     validate_concatenation(input_files=fastqs, output_file=file)
     return file
 
 
 def get_new_unique_file(directory: Path) -> Path:
     unique_id = uuid.uuid4()
-    return Path(directory, f"{unique_id}.fastq.gz")
+    return Path(directory, f"{unique_id}{FileExtensions.FASTQ}{FileExtensions.GZIP}")
 
 
 def get_forward_read_fastqs(fastq_directory: Path) -> list[Path]:
-    return get_fastqs_by_direction(fastq_directory=fastq_directory, direction=1)
+    return get_fastqs_by_direction(fastq_directory=fastq_directory, direction=ReadDirection.FORWARD)
 
 
 def get_reverse_read_fastqs(fastq_directory: Path) -> list[Path]:
-    return get_fastqs_by_direction(fastq_directory=fastq_directory, direction=2)
+    return get_fastqs_by_direction(fastq_directory=fastq_directory, direction=ReadDirection.REVERSE)
 
 
 def get_fastqs_by_direction(fastq_directory: Path, direction: int) -> list[Path]:
-    pattern = f".+_R{direction}_[0-9]+.fastq.gz"
+    pattern = f".+_R{direction}_[0-9]+{FileExtensions.FASTQ}{FileExtensions.GZIP}"
     fastqs: list[Path] = []
     for file in fastq_directory.iterdir():
         if re.match(pattern, file.name):
             fastqs.append(file)
     return sort_files_by_name(fastqs)
 
 
@@ -67,14 +69,14 @@
 
 
 def sort_files_by_name(files: list[Path]) -> list[Path]:
     return sorted(files, key=lambda file: file.name)
 
 
 def file_can_be_removed(file: Path, forward_file: Path, reverse_file: Path) -> bool:
-    return file.suffix == ".gz" and file != forward_file and file != reverse_file
+    return file.suffix == FileExtensions.GZIP and file != forward_file and file != reverse_file
 
 
 def remove_raw_fastqs(fastq_directory: Path, forward_file: Path, reverse_file: Path) -> None:
     for file in fastq_directory.iterdir():
         if file_can_be_removed(file=file, forward_file=forward_file, reverse_file=reverse_file):
             file.unlink()
```

### Comparing `cg-59.9.1/cg/services/orders/order_service/order_service.py` & `cg-60.0.0/cg/services/orders/order_service/order_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 from cg.models.orders.order import OrderIn
 from cg.server.dto.orders.orders_request import OrdersRequest
 from cg.server.dto.orders.orders_response import Order as OrderResponse
 from cg.server.dto.orders.orders_response import OrdersResponse
-from cg.services.orders.order_service.exceptions import OrderNotFoundError
 from cg.services.orders.order_service.utils import (
     create_order_response,
     create_orders_response,
+    order_is_delivered,
 )
-from cg.services.orders.order_status_service import OrderStatusService
-from cg.services.orders.order_status_service.dto.order_status_summary import (
-    OrderSummary,
-)
+from cg.services.orders.order_status_service import OrderSummaryService
+from cg.services.orders.order_status_service.dto.order_summary import OrderSummary
 from cg.store.models import Case, Order
 from cg.store.store import Store
 
 
 class OrderService:
-    def __init__(self, store: Store, status_service: OrderStatusService) -> None:
+    def __init__(self, store: Store, status_service: OrderSummaryService) -> None:
         self.store = store
         self.summary_service = status_service
 
     def get_order(self, order_id: int) -> OrderResponse:
-        order: Order | None = self.store.get_order_by_id(order_id)
-        if not order:
-            raise OrderNotFoundError(f"Order {order_id} not found.")
-        summary: OrderSummary = self.summary_service.get_status_summary(order_id)
+        order: Order = self.store.get_order_by_id(order_id)
+        summary: OrderSummary = self.summary_service.get_summary(order_id)
         return create_order_response(order=order, summary=summary)
 
     def get_orders(self, orders_request: OrdersRequest) -> OrdersResponse:
         orders, total_count = self.store.get_orders(orders_request)
         order_ids: list[int] = [order.id for order in orders]
-        summaries: list[OrderSummary] = self.summary_service.get_status_summaries(order_ids)
+        summaries: list[OrderSummary] = self.summary_service.get_summaries(order_ids)
         return create_orders_response(orders=orders, summaries=summaries, total=total_count)
 
     def create_order(self, order_data: OrderIn) -> OrderResponse:
         """Creates an order and links it to the given cases."""
         order: Order = self.store.add_order(order_data)
         cases: list[Case] = self.store.get_cases_by_ticket_id(order_data.ticket)
         for case in cases:
             self.store.link_case_to_order(order_id=order.id, case_id=case.id)
         return create_order_response(order)
+
+    def set_delivery(self, order_id: int, delivered: bool) -> OrderResponse:
+        order: Order = self.store.update_order_delivery(order_id=order_id, delivered=delivered)
+        return create_order_response(order)
+
+    def update_delivered(self, order_id: int, delivered_analyses: int) -> None:
+        """Update the delivery status of an order based on the number of delivered analyses."""
+        order: Order = self.store.get_order_by_id(order_id)
+        case_count: int = len(order.cases)
+        if order_is_delivered(case_count=case_count, delivered_analyses=delivered_analyses):
+            self.set_delivery(order_id=order_id, delivered=True)
+        elif order.is_delivered:
+            self.set_delivery(order_id=order_id, delivered=False)
```

### Comparing `cg-59.9.1/cg/services/orders/order_service/utils.py` & `cg-60.0.0/cg/services/orders/order_service/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 def create_order_response(order: DatabaseOrder, summary: OrderSummary | None = None) -> Order:
     return Order(
         customer_id=order.customer.internal_id,
         ticket_id=order.ticket_id,
         order_date=str(order.order_date.date()),
         id=order.id,
+        is_delivered=order.is_delivered,
         workflow=order.workflow,
         summary=summary,
     )
 
 
 def create_orders_response(
     orders: list[DatabaseOrder], summaries: list[OrderSummary], total: int
@@ -23,7 +24,11 @@
 
 def _add_summaries(orders: list[Order], summaries: list[OrderSummary]) -> list[Order]:
     order_map = {order.id: order for order in orders}
     for summary in summaries:
         order = order_map[summary.order_id]
         order.summary = summary
     return orders
+
+
+def order_is_delivered(case_count: int, delivered_analyses: int) -> bool:
+    return delivered_analyses >= case_count
```

### Comparing `cg-59.9.1/cg/services/slurm_service/slurm_cli_service.py` & `cg-60.0.0/cg/services/slurm_service/slurm_cli_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/services/slurm_upload_service/slurm_upload_service.py` & `cg-60.0.0/cg/services/slurm_upload_service/slurm_upload_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/base.py` & `cg-60.0.0/tests/cli/add/test_cli_add_family.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,194 +1,241 @@
-"""All models aggregated in a base class."""
+"""Tests the CLI methods to add cases to the status database."""
 
-from dataclasses import dataclass
-from typing import Callable, Type
+from click.testing import CliRunner
 
-from sqlalchemy import and_, func
-from sqlalchemy.orm import Query, Session
+from cg.cli.add import add
+from cg.constants import DataDelivery, Workflow
+from cg.models.cg_config import CGConfig
+from cg.store.models import Case, Customer, Panel
+from cg.store.store import Store
+from tests.store_helpers import StoreHelpers
+
+CLI_OPTION_ANALYSIS = Workflow.BALSAMIC_UMI
+CLI_OPTION_DELIVERY = DataDelivery.FASTQ_QC
+
+
+def test_add_case_required(
+    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers, ticket_id: str
+):
+    """Test to add a case using only the required arguments"""
+    # GIVEN a database with a customer and a panel
+    disk_store: Store = base_context.status_db
+
+    customer: Customer = helpers.ensure_customer(store=disk_store)
+    customer_id = customer.internal_id
+    panel: Panel = helpers.ensure_panel(store=disk_store)
+    panel_id = panel.name
+    name = "case_name"
+
+    # WHEN adding a panel
+    result = cli_runner.invoke(
+        add,
+        [
+            "case",
+            "--panel",
+            panel_id,
+            "--analysis",
+            CLI_OPTION_ANALYSIS,
+            "--data-delivery",
+            CLI_OPTION_DELIVERY,
+            "--ticket",
+            ticket_id,
+            customer_id,
+            name,
+        ],
+        obj=base_context,
+        input="y",
+    )
+
+    # THEN it should be added
+    assert result.exit_code == 0
+    case_query = disk_store._get_query(table=Case)
+    assert case_query.count() == 1
+    assert case_query.first().name == name
+    assert case_query.first().panels == [panel_id]
+
+
+def test_add_case_bad_workflow(
+    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers, ticket_id: str
+):
+    """Test to add a case using only the required arguments"""
+    # GIVEN a database with a customer and a panel
+
+    # WHEN adding a case
+    disk_store: Store = base_context.status_db
+
+    customer: Customer = helpers.ensure_customer(store=disk_store)
+    customer_id = customer.internal_id
+    panel: Panel = helpers.ensure_panel(store=disk_store)
+    panel_id = panel.name
+    non_existing_analysis = "epigenentic_alterations"
+    name = "case_name"
+
+    result = cli_runner.invoke(
+        add,
+        [
+            "case",
+            "--panel",
+            panel_id,
+            "--analysis",
+            non_existing_analysis,
+            "--data-delivery",
+            CLI_OPTION_DELIVERY,
+            "--ticket",
+            ticket_id,
+            customer_id,
+            name,
+        ],
+        input="y",
+    )
+
+    # THEN it should not be added
+    assert result.exit_code != 0
+    assert disk_store._get_query(table=Case).count() == 0
+
+
+def test_add_case_bad_data_delivery(
+    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers
+):
+    """Test to add a case using only the required arguments"""
+    # GIVEN a database with a customer and an panel
+
+    # WHEN adding a case without data delivery
+    disk_store: Store = base_context.status_db
+
+    customer: Customer = helpers.ensure_customer(store=disk_store)
+    customer_id = customer.internal_id
+    panel: Panel = helpers.ensure_panel(store=disk_store)
+    panel_id = panel.name
+    name = "case_name"
+    non_existing_data_delivery = "aws"
+
+    result = cli_runner.invoke(
+        add,
+        [
+            "case",
+            "--panel",
+            panel_id,
+            "--analysis",
+            CLI_OPTION_ANALYSIS,
+            "--data-delivery",
+            non_existing_data_delivery,
+            customer_id,
+            name,
+        ],
+        obj=base_context,
+        input="y",
+    )
+
+    # THEN it should not be added
+    assert result.exit_code != 0
+    assert disk_store._get_query(table=Case).count() == 0
+
+
+def test_add_case_bad_customer(cli_runner: CliRunner, base_context: CGConfig, ticket_id: str):
+    """Test to add a case using a non-existing customer"""
+    # GIVEN an empty database
+    disk_store: Store = base_context.status_db
+    # WHEN adding a case
+    panel_id = "dummy_panel"
+    customer_id = "dummy_customer"
+    name = "dummy_name"
+    result = cli_runner.invoke(
+        add,
+        [
+            "case",
+            "--panel",
+            panel_id,
+            "--analysis",
+            CLI_OPTION_ANALYSIS,
+            "--data-delivery",
+            CLI_OPTION_DELIVERY,
+            "--ticket",
+            ticket_id,
+            customer_id,
+            name,
+        ],
+        obj=base_context,
+        input="y",
+    )
+
+    # THEN it should complain about missing customer instead of adding a case
+    assert result.exit_code == 1
+    assert disk_store._get_query(table=Case).count() == 0
+
+
+def test_add_case_bad_panel(
+    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers, ticket_id: str
+):
+    """Test to add a case using a non-existing panel"""
+    # GIVEN a database with a customer
+    disk_store: Store = base_context.status_db
+    # WHEN adding a case
+    customer: Customer = helpers.ensure_customer(store=disk_store)
+    customer_id = customer.internal_id
+    panel_id = "dummy_panel"
+    name = "dummy_name"
+    result = cli_runner.invoke(
+        add,
+        [
+            "case",
+            "--panel",
+            panel_id,
+            "--analysis",
+            CLI_OPTION_ANALYSIS,
+            "--data-delivery",
+            CLI_OPTION_DELIVERY,
+            "--ticket",
+            ticket_id,
+            customer_id,
+            name,
+        ],
+        obj=base_context,
+    )
+
+    # THEN it should complain about missing panel instead of adding a case
+    assert result.exit_code == 1
+    assert disk_store._get_query(table=Case).count() == 0
+
+
+def test_add_case_priority(
+    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers, ticket_id: str
+):
+    """Test that the added case get the priority we send in"""
+    # GIVEN a database with a customer and a panel
+    disk_store: Store = base_context.status_db
+    # WHEN adding a case
+    customer: Customer = helpers.ensure_customer(store=disk_store)
+    customer_id = customer.internal_id
+    panel: Panel = helpers.ensure_panel(store=disk_store)
+    panel_id = panel.name
+
+    name = "case_name"
+    priority = "priority"
+
+    result = cli_runner.invoke(
+        add,
+        [
+            "case",
+            "--panel",
+            panel_id,
+            "--priority",
+            priority,
+            "--analysis",
+            CLI_OPTION_ANALYSIS,
+            "--data-delivery",
+            CLI_OPTION_DELIVERY,
+            "--ticket",
+            ticket_id,
+            customer_id,
+            name,
+        ],
+        obj=base_context,
+        input="y",
+    )
+
+    # THEN it should be added
+    assert result.exit_code == 0
+    case_query = disk_store._get_query(table=Case)
 
-from cg.store.filters.status_case_filters import CaseFilter, apply_case_filter
-from cg.store.filters.status_customer_filters import (
-    CustomerFilter,
-    apply_customer_filter,
-)
-from cg.store.filters.status_sample_filters import SampleFilter, apply_sample_filter
-from cg.store.models import (
-    Analysis,
-    Application,
-    ApplicationLimitations,
-    ApplicationVersion,
-)
-from cg.store.models import Base as ModelBase
-from cg.store.models import Case, CaseSample, Customer, Flowcell, Sample
-from cg.utils.date import get_date_days_ago
-
-
-@dataclass
-class BaseHandler:
-    """All queries in one base class."""
-
-    def __init__(self, session: Session):
-        self.session = session
-
-    def _get_query(self, table: Type[ModelBase]) -> Query:
-        """Return a query for the given table."""
-        return self.session.query(table)
-
-    def _get_outer_join_cases_with_analyses_query(self) -> Query:
-        """Return a query for all cases in the database with an analysis."""
-        return (
-            self._get_query(table=Case)
-            .outerjoin(Analysis)
-            .join(Case.links)
-            .join(CaseSample.sample)
-            .join(ApplicationVersion)
-            .join(Application)
-        )
-
-    def _get_join_cases_with_samples_query(self) -> Query:
-        """Return a join query for all cases in the database with samples."""
-        return (
-            self._get_query(table=Case).join(Case.links).join(CaseSample.sample).join(Case.customer)
-        )
-
-    def _get_join_analysis_case_query(self) -> Query:
-        """Return join analysis case query."""
-        return self._get_query(table=Analysis).join(Analysis.case)
-
-    def _get_join_case_sample_query(self) -> Query:
-        """Return join case sample query."""
-        return self._get_query(table=CaseSample).join(CaseSample.case).join(CaseSample.sample)
-
-    def _get_join_case_and_sample_query(self) -> Query:
-        """Return join case sample query."""
-        return self._get_query(table=Case).join(Case.links).join(CaseSample.sample)
-
-    def _get_join_sample_and_customer_query(self) -> Query:
-        """Return join sample and customer query."""
-        return self._get_query(table=Sample).join(Customer)
-
-    def _get_join_flow_cell_sample_links_query(self) -> Query:
-        """Return join flow cell samples and relationship query."""
-        return self._get_query(table=Flowcell).join(Flowcell.samples).join(Sample.links)
-
-    def _get_join_sample_family_query(self) -> Query:
-        """Return a join sample case relationship query."""
-        return self._get_query(table=Sample).join(Case.links).join(CaseSample.sample)
-
-    def _get_join_sample_application_version_query(self) -> Query:
-        """Return join sample to application version query."""
-        return (
-            self._get_query(table=Sample)
-            .join(Sample.application_version)
-            .join(ApplicationVersion.application)
-        )
-
-    def _get_join_analysis_sample_family_query(self) -> Query:
-        """Return join analysis to sample to case query."""
-        return self._get_query(table=Analysis).join(Case).join(Case.links).join(CaseSample.sample)
-
-    def _get_subquery_with_latest_case_analysis_date(self) -> Query:
-        """Return a subquery with the case internal id and the date of its latest analysis."""
-        case_and_date: Query = (
-            self._get_join_analysis_case_query()
-            .group_by(Case.id)
-            .with_entities(Analysis.case_id, func.max(Analysis.started_at).label("started_at"))
-            .subquery()
-        )
-        return case_and_date
-
-    def _get_latest_analyses_for_cases_query(self) -> Query:
-        """Return a join query for the latest analysis for each case."""
-        analyses: Query = self._get_query(table=Analysis)
-        case_and_date_subquery: Query = self._get_subquery_with_latest_case_analysis_date()
-        return analyses.join(
-            case_and_date_subquery,
-            and_(
-                Analysis.case_id == case_and_date_subquery.c.case_id,
-                Analysis.started_at == case_and_date_subquery.c.started_at,
-            ),
-        )
-
-    def _get_filtered_case_query(
-        self,
-        case_action: str | None,
-        customer_id: str,
-        data_analysis: str,
-        days: int,
-        exclude_customer_id: bool,
-        internal_id: str,
-        name: str,
-        priority: str,
-        sample_id: str,
-    ) -> Query:
-        cases_query: Query = self._get_query(table=Case)
-        filter_functions: list[Callable] = []
-
-        filter_case_order_date = None
-        if days != 0:
-            filter_case_order_date = get_date_days_ago(days_ago=days)
-            filter_functions.append(CaseFilter.NEW_BY_ORDER_DATE)
-        if case_action:
-            filter_functions.append(CaseFilter.BY_ACTION)
-        if priority:
-            filter_functions.append(CaseFilter.BY_PRIORITY)
-        if internal_id:
-            filter_functions.append(CaseFilter.BY_INTERNAL_ID_SEARCH)
-        if name:
-            filter_functions.append(CaseFilter.BY_NAME_SEARCH)
-        if data_analysis:
-            filter_functions.append(CaseFilter.BY_WORKFLOW_SEARCH)
-
-        cases_query = apply_case_filter(
-            cases=cases_query,
-            filter_functions=filter_functions,
-            action=case_action,
-            internal_id_search=internal_id,
-            name_search=name,
-            order_date=filter_case_order_date,
-            workflow_search=data_analysis,
-            priority=priority,
-        )
-
-        # customer filters
-        customer_filters: list[Callable] = []
-        if customer_id or exclude_customer_id:
-            cases_query = cases_query.join(Case.customer)
-
-        if customer_id:
-            customer_filters.append(CustomerFilter.BY_INTERNAL_ID)
-
-        if exclude_customer_id:
-            customer_filters.append(CustomerFilter.EXCLUDE_INTERNAL_ID)
-
-        cases_query = apply_customer_filter(
-            customers=cases_query,
-            filter_functions=customer_filters,
-            customer_internal_id=customer_id,
-            exclude_customer_internal_id=exclude_customer_id,
-        )
-
-        # sample filters
-        if sample_id:
-            cases_query = cases_query.join(Case.links).join(CaseSample.sample)
-            cases_query = apply_sample_filter(
-                samples=cases_query,
-                filter_functions=[SampleFilter.BY_INTERNAL_ID_PATTERN],
-                internal_id_pattern=sample_id,
-            )
-        else:
-            cases_query = cases_query.outerjoin(Case.links).outerjoin(CaseSample.sample)
-
-        # other joins
-        cases_query = (
-            cases_query.outerjoin(Case.analyses)
-            .outerjoin(Sample.invoice)
-            .outerjoin(Sample.flowcells)
-        )
-        return cases_query
-
-    def _get_join_application_limitations_query(self) -> Query:
-        """Return a join query for all application limitations."""
-        return self._get_query(table=ApplicationLimitations).join(
-            ApplicationLimitations.application
-        )
+    assert case_query.count() == 1
+    assert case_query.first().priority_human == priority
```

### Comparing `cg-59.9.1/cg/store/crud/create.py` & `cg-60.0.0/cg/store/crud/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         created_at: datetime = datetime.now(),
         updated_at: datetime = datetime.now(),
         **kwargs,
     ) -> ApplicationLimitations:
         """Build a new application limitations record."""
         return ApplicationLimitations(
             application=application,
-            pipeline=workflow,
+            workflow=workflow,
             limitations=limitations,
             comment=comment,
             created_at=created_at,
             updated_at=updated_at,
             **kwargs,
         )
 
@@ -171,16 +171,18 @@
         self,
         name: str,
         sex: str,
         comment: str = None,
         control: str = None,
         downsampled_to: int = None,
         internal_id: str = None,
+        last_sequenced_at: datetime = None,
         order: str = None,
         ordered: datetime = None,
+        prepared_at: datetime = None,
         priority: Priority = None,
         received: datetime = None,
         original_ticket: str = None,
         tumour: bool = False,
         **kwargs,
     ) -> Sample:
         """Build a new Sample record."""
@@ -189,18 +191,20 @@
         priority = priority or (Priority.research if downsampled_to else Priority.standard)
         return Sample(
             comment=comment,
             control=control,
             downsampled_to=downsampled_to,
             internal_id=internal_id,
             is_tumour=tumour,
+            last_sequenced_at=last_sequenced_at,
             name=name,
             order=order,
             ordered_at=ordered or datetime.now(),
             original_ticket=original_ticket,
+            prepared_at=prepared_at,
             priority=priority,
             received_at=received,
             sex=sex,
             **kwargs,
         )
 
     def add_case(
```

### Comparing `cg-59.9.1/cg/store/crud/delete.py` & `cg-60.0.0/cg/store/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/crud/update.py` & `cg-60.0.0/cg/store/crud/update.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Handler to update data objects"""
 
 from sqlalchemy.orm import Session
 
 from cg.store.base import BaseHandler
-from cg.store.models import Flowcell, Sample
+from cg.store.models import Flowcell, Order, Sample
 
 
 class UpdateHandler(BaseHandler):
     """Contains methods to update database objects."""
 
     def __init__(self, session: Session):
         super().__init__(session=session)
@@ -20,7 +20,14 @@
     def update_sample_comment(self, sample: Sample, comment: str) -> None:
         """Update comment on sample with the provided comment."""
         if sample.comment:
             sample.comment = sample.comment + " " + comment
         else:
             sample.comment = comment
         self.session.commit()
+
+    def update_order_delivery(self, order_id: int, delivered: bool) -> Order:
+        """Update the delivery status of an order."""
+        order: Order = self.get_order_by_id(order_id)
+        order.is_delivered = delivered
+        self.session.commit()
+        return order
```

### Comparing `cg-59.9.1/cg/store/database.py` & `cg-60.0.0/cg/store/database.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_analysis_filters.py` & `cg-60.0.0/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_application_filters.py` & `cg-60.0.0/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_application_limitations_filters.py` & `cg-60.0.0/cg/store/filters/status_application_limitations_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     return application_limitations.filter(Application.tag == tag)
 
 
 def filter_application_limitations_by_workflow(
     application_limitations: Query, workflow: Workflow, **kwargs
 ) -> Query:
     """Return application limitations by workflow."""
-    return application_limitations.filter(ApplicationLimitations.pipeline == workflow)
+    return application_limitations.filter(ApplicationLimitations.workflow == workflow)
 
 
 def apply_application_limitations_filter(
     filter_functions: list[Callable],
     application_limitations: Query,
     tag: str = None,
     workflow: Workflow = None,
```

### Comparing `cg-59.9.1/cg/store/filters/status_application_version_filters.py` & `cg-60.0.0/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_bed_filters.py` & `cg-60.0.0/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_bed_version_filters.py` & `cg-60.0.0/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_case_filters.py` & `cg-60.0.0/cg/store/filters/status_case_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 
 
 def filter_case_by_internal_id(cases: Query, internal_id: str, **kwargs) -> Query:
     """Filter cases with matching internal id."""
     return cases.filter(Case.internal_id == internal_id)
 
 
+def filter_cases_by_internal_ids(cases: Query, internal_ids: list[str], **kwargs) -> Query:
+    """Filter cases with internal ids."""
+    return cases.filter(Case.internal_id.in_(internal_ids))
+
+
 def filter_cases_by_internal_id_search(cases: Query, internal_id_search: str, **kwargs) -> Query:
     """Filter cases with internal ids matching the search pattern."""
     return cases.filter(Case.internal_id.contains(internal_id_search))
 
 
 def filter_cases_by_name(cases: Query, name: str, **kwargs) -> Query:
     """Filter cases with matching name."""
@@ -206,55 +211,60 @@
     action: str | None = None,
     case_search: str | None = None,
     creation_date: datetime | None = None,
     customer_entry_id: int | None = None,
     customer_entry_ids: list[int] | None = None,
     entry_id: int | None = None,
     internal_id: str | None = None,
+    internal_ids: list[str] | None = None,
     internal_id_search: str | None = None,
     name: str | None = None,
     name_search: str | None = None,
     order_date: datetime | None = None,
     workflow: Workflow | None = None,
     workflow_search: str | None = None,
     priority: str | None = None,
     ticket_id: str | None = None,
+    order_id: int | None = None,
 ) -> Query:
     """Apply filtering functions and return filtered results."""
     for function in filter_functions:
         cases: Query = function(
             action=action,
             case_search=case_search,
             cases=cases,
             creation_date=creation_date,
             customer_entry_id=customer_entry_id,
             customer_entry_ids=customer_entry_ids,
             entry_id=entry_id,
             internal_id=internal_id,
+            internal_ids=internal_ids,
             internal_id_search=internal_id_search,
             name=name,
             name_search=name_search,
             order_date=order_date,
             workflow=workflow,
             workflow_search=workflow_search,
             priority=priority,
             ticket_id=ticket_id,
+            order_id=order_id,
         )
     return cases
 
 
 class CaseFilter(Enum):
     """Define case filters."""
 
     BY_ACTION: Callable = filter_cases_by_action
     BY_CASE_SEARCH: Callable = filter_cases_by_case_search
     BY_CUSTOMER_ENTRY_ID: Callable = filter_cases_by_customer_entry_id
     BY_CUSTOMER_ENTRY_IDS: Callable = filter_cases_by_customer_entry_ids
     BY_ENTRY_ID: Callable = filter_cases_by_entry_id
     BY_INTERNAL_ID: Callable = filter_case_by_internal_id
+    BY_INTERNAL_IDS: Callable = filter_cases_by_internal_ids
     BY_INTERNAL_ID_SEARCH: Callable = filter_cases_by_internal_id_search
     BY_NAME: Callable = filter_cases_by_name
     BY_NAME_SEARCH: Callable = filter_cases_by_name_search
     BY_WORKFLOW_SEARCH: Callable = filter_cases_by_workflow_search
     BY_PRIORITY: Callable = filter_cases_by_priority
     BY_TICKET: Callable = filter_cases_by_ticket_id
     FOR_ANALYSIS: Callable = filter_cases_for_analysis
```

### Comparing `cg-59.9.1/cg/store/filters/status_collaboration_filters.py` & `cg-60.0.0/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_customer_filters.py` & `cg-60.0.0/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_flow_cell_filters.py` & `cg-60.0.0/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_invoice_filters.py` & `cg-60.0.0/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_metrics_filters.py` & `cg-60.0.0/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_order_filters.py` & `cg-60.0.0/cg/store/filters/status_order_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import Callable
-from sqlalchemy import asc, desc
 
+from sqlalchemy import asc, desc, or_
 from sqlalchemy.orm import Query
-from cg.server.dto.orders.orders_request import OrderSortField, SortOrder
 
-from cg.store.models import Order
+from cg.server.dto.orders.orders_request import OrderSortField, SortOrder
+from cg.store.models import Customer, Order
 
 
 def filter_orders_by_workflow(orders: Query, workflow: str | None, **kwargs) -> Query:
     return orders.filter(Order.workflow == workflow) if workflow else orders
 
 
 def filter_orders_by_id(orders: Query, id: int | None, **kwargs) -> Query:
@@ -24,52 +24,76 @@
     return orders.limit(page_size).offset((page - 1) * page_size) if page and page_size else orders
 
 
 def filter_orders_by_ticket_id(orders: Query, ticket_id: int | None, **kwargs) -> Query:
     return orders.filter(Order.ticket_id == ticket_id) if ticket_id else orders
 
 
+def filter_orders_by_search(orders: Query, search: str | None, **kwargs) -> Query:
+    if not search:
+        return orders
+
+    orders = orders.join(Order.customer)
+    return orders.filter(
+        or_(
+            Order.id == search,
+            Order.ticket_id == search,
+            Customer.internal_id.icontains(search),
+        )
+    )
+
+
+def filter_orders_by_delivered(orders: Query, delivered: bool | None, **kwargs) -> Query:
+    return orders.filter(Order.is_delivered == delivered) if delivered is not None else orders
+
+
 def apply_sorting(
     orders: Query, sort_field: OrderSortField | None, sort_order: SortOrder | None, **kwargs
 ) -> Query:
     if sort_field:
         column = getattr(Order, sort_field)
         if sort_order == "asc":
             return orders.order_by(asc(column))
         return orders.order_by(desc(column))
     return orders
 
 
 class OrderFilter(Enum):
     BY_ID: Callable = filter_orders_by_id
     BY_IDS: Callable = filter_orders_by_ids
+    BY_SEARCH: Callable = filter_orders_by_search
     BY_TICKET_ID: Callable = filter_orders_by_ticket_id
     BY_WORKFLOW: Callable = filter_orders_by_workflow
+    BY_DELIVERED: Callable = filter_orders_by_delivered
     PAGINATE: Callable = apply_pagination
     SORT: Callable = apply_sorting
 
 
 def apply_order_filters(
     filters: list[OrderFilter],
     orders: Query,
     id: int = None,
     ids: list[int] = None,
     ticket_id: int = None,
     workflow: SortOrder = None,
     page: int = None,
     page_size: int = None,
-    sort_field: str = None,
-    sort_order: str = None,
+    sort_field: OrderSortField = None,
+    sort_order: SortOrder = None,
+    search: str = None,
+    delivered: bool = None,
 ) -> Query:
     for filter in filters:
         orders: Query = filter(
             orders=orders,
             id=id,
             ids=ids,
             workflow=workflow,
             page=page,
             page_size=page_size,
             ticket_id=ticket_id,
             sort_field=sort_field,
             sort_order=sort_order,
+            search=search,
+            delivered=delivered,
         )
     return orders
```

### Comparing `cg-59.9.1/cg/store/filters/status_organism_filters.py` & `cg-60.0.0/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_panel_filters.py` & `cg-60.0.0/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_pool_filters.py` & `cg-60.0.0/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_sample_filters.py` & `cg-60.0.0/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/filters/status_user_filters.py` & `cg-60.0.0/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/store/models.py` & `cg-60.0.0/cg/store/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
     String,
     Table,
 )
 from sqlalchemy import Text as SLQText
 from sqlalchemy import UniqueConstraint, orm, types
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
 from sqlalchemy.orm.attributes import InstrumentedAttribute
-from sqlalchemy.util import deprecated
 
 from cg.constants import DataDelivery, FlowCellStatus, Priority, Workflow
 from cg.constants.archiving import PDC_ARCHIVE_LOCATION
 from cg.constants.constants import (
     CaseActions,
     ControlOptions,
     PrepCategory,
     SexOptions,
     StatusOptions,
 )
 from cg.constants.priority import SlurmQos
+from cg.constants.symbols import EMPTY_STRING
 
 BigInt = Annotated[int, None]
 Blob = Annotated[bytes, None]
 Decimal = Annotated[float, None]
 Num_6_2 = Annotated[float, 6]
 Str32 = Annotated[str, 32]
 Str64 = Annotated[str, 64]
@@ -67,22 +67,14 @@
         return {
             column.name: getattr(model_instance, column.name)
             for column in model_instance.__table__.columns
             if not isinstance(getattr(model_instance, column.name), InstrumentedAttribute)
         }
 
 
-flowcell_sample = Table(
-    "flowcell_sample",
-    Base.metadata,
-    Column("flowcell_id", types.Integer, ForeignKey("flowcell.id"), nullable=False),
-    Column("sample_id", types.Integer, ForeignKey("sample.id"), nullable=False),
-    UniqueConstraint("flowcell_id", "sample_id", name="_flowcell_sample_uc"),
-)
-
 customer_user = Table(
     "customer_user",
     Base.metadata,
     Column("customer_id", types.Integer, ForeignKey("customer.id"), nullable=False),
     Column("user_id", types.Integer, ForeignKey("user.id"), nullable=False),
     UniqueConstraint("customer_id", "user_id", name="_customer_user_uc"),
 )
@@ -236,24 +228,24 @@
 
 
 class ApplicationLimitations(Base):
     __tablename__ = "application_limitations"
 
     id: Mapped[PrimaryKeyInt]
     application_id: Mapped[int] = mapped_column(ForeignKey(Application.id))
-    pipeline: Mapped[str] = mapped_column(types.Enum(*(workflow.value for workflow in Workflow)))
+    workflow: Mapped[str] = mapped_column(types.Enum(*(workflow.value for workflow in Workflow)))
     limitations: Mapped[Text | None]
     comment: Mapped[Text | None]
     created_at: Mapped[datetime | None] = mapped_column(default=datetime.now)
     updated_at: Mapped[datetime | None] = mapped_column(onupdate=datetime.now)
 
     application: Mapped[Application] = orm.relationship(back_populates="pipeline_limitations")
 
     def __str__(self):
-        return f"{self.application.tag} – {self.pipeline}"
+        return f"{self.application.tag} – {self.workflow}"
 
     def to_dict(self):
         return to_dict(model_instance=self)
 
 
 class Analysis(Base):
     __tablename__ = "analysis"
@@ -458,15 +450,14 @@
     data_delivery: Mapped[str | None] = mapped_column(
         types.Enum(*(delivery.value for delivery in DataDelivery))
     )
     id: Mapped[PrimaryKeyInt]
     internal_id: Mapped[UniqueStr]
     is_compressible: Mapped[bool] = mapped_column(default=True)
     name: Mapped[Str128]
-    order_id: Mapped[int | None] = mapped_column(ForeignKey("order.id"))
     ordered_at: Mapped[datetime | None] = mapped_column(default=datetime.now)
     _panels: Mapped[Text | None]
 
     priority: Mapped[Priority] = mapped_column(
         default=Priority.standard,
     )
     synopsis: Mapped[Text | None]
@@ -538,14 +529,19 @@
 
     @property
     def samples(self) -> list["Sample"]:
         """Return case samples."""
         return self._get_samples
 
     @property
+    def sample_ids(self) -> list[str]:
+        """Return a list of internal ids of the case samples."""
+        return [sample.internal_id for sample in self._get_samples]
+
+    @property
     def _get_samples(self) -> list["Sample"]:
         """Extract samples from a case."""
         return [link.sample for link in self.links]
 
     @property
     def tumour_samples(self) -> list["Sample"]:
         """Return tumour samples."""
@@ -644,14 +640,24 @@
         if family:
             data["family"] = self.case.to_dict()
         return data
 
     def __str__(self) -> str:
         return f"{self.case.internal_id} | {self.sample.internal_id}"
 
+    @property
+    def get_maternal_sample_id(self) -> str:
+        """Return parental id."""
+        return self.mother.internal_id if self.mother else EMPTY_STRING
+
+    @property
+    def get_paternal_sample_id(self) -> str:
+        """Return parental id."""
+        return self.father.internal_id if self.father else EMPTY_STRING
+
 
 class Flowcell(Base):
     __tablename__ = "flowcell"
     id: Mapped[PrimaryKeyInt]
     name: Mapped[UniqueStr]
     sequencer_type: Mapped[str | None] = mapped_column(
         types.Enum("hiseqga", "hiseqx", "novaseq", "novaseqx")
@@ -660,23 +666,24 @@
     sequenced_at: Mapped[datetime | None]
     status: Mapped[str | None] = mapped_column(
         types.Enum(*(status.value for status in FlowCellStatus)), default="ondisk"
     )
     archived_at: Mapped[datetime | None]
     has_backup: Mapped[bool] = mapped_column(default=False)
     updated_at: Mapped[datetime | None] = mapped_column(onupdate=datetime.now)
-
-    samples: Mapped[list["Sample"]] = orm.relationship(
-        secondary=flowcell_sample, back_populates="flowcells"
-    )
     sequencing_metrics: Mapped[list["SampleLaneSequencingMetrics"]] = orm.relationship(
         back_populates="flowcell",
         cascade="all, delete, delete-orphan",
     )
 
+    @property
+    def samples(self) -> list["Sample"]:
+        """Return samples sequenced on the flow cell."""
+        return list({metric.sample for metric in self.sequencing_metrics})
+
     def __str__(self):
         return self.name
 
     def to_dict(self, samples: bool = False):
         """Represent as dictionary"""
         data = to_dict(model_instance=Flowcell)
         if samples:
@@ -768,16 +775,14 @@
     delivered_at: Mapped[datetime | None]
     deliveries: Mapped[list[Delivery]] = orm.relationship(backref="sample")
     downsampled_to: Mapped[BigInt | None]
     from_sample: Mapped[Str128 | None]
     id: Mapped[PrimaryKeyInt]
     internal_id: Mapped[UniqueStr]
     invoice_id: Mapped[int | None] = mapped_column(ForeignKey("invoice.id"))
-    invoiced_at: Mapped[datetime | None]  # DEPRECATED
-    _is_external: Mapped[bool | None] = mapped_column("is_external")  # DEPRECATED
     is_tumour: Mapped[bool | None] = mapped_column(default=False)
     loqusdb_id: Mapped[Str64 | None]
     name: Mapped[Str128]
     no_invoice: Mapped[bool] = mapped_column(default=False)
     order: Mapped[Str64 | None]
     ordered_at: Mapped[datetime]
     organism_id: Mapped[int | None] = mapped_column(ForeignKey("organism.id"))
@@ -788,46 +793,38 @@
     prepared_at: Mapped[datetime | None]
 
     priority: Mapped[Priority] = mapped_column(default=Priority.standard)
     reads: Mapped[BigInt | None] = mapped_column(default=0)
     last_sequenced_at: Mapped[datetime | None]
     received_at: Mapped[datetime | None]
     reference_genome: Mapped[Str255 | None]
-    sequence_start: Mapped[datetime | None]
     sex: Mapped[str] = mapped_column(types.Enum(*(option.value for option in SexOptions)))
     subject_id: Mapped[Str128 | None]
 
     links: Mapped[list[CaseSample]] = orm.relationship(
         foreign_keys=[CaseSample.sample_id], back_populates="sample"
     )
     mother_links: Mapped[list[CaseSample]] = orm.relationship(
         foreign_keys=[CaseSample.mother_id], back_populates="mother"
     )
     father_links: Mapped[list[CaseSample]] = orm.relationship(
         foreign_keys=[CaseSample.father_id], back_populates="father"
     )
-    flowcells: Mapped[list[Flowcell]] = orm.relationship(
-        secondary=flowcell_sample, back_populates="samples"
-    )
     sequencing_metrics: Mapped[list["SampleLaneSequencingMetrics"]] = orm.relationship(
         back_populates="sample"
     )
     invoice: Mapped["Invoice | None"] = orm.relationship(back_populates="samples")
 
     def __str__(self) -> str:
         return f"{self.internal_id} ({self.name})"
 
     @property
-    @deprecated(
-        version="1.4.0",
-        message="This field is deprecated, use sample.application_version.application.is_external",
-    )
-    def is_external(self):
-        """Return if this is an externally sequenced sample."""
-        return self._is_external
+    def flow_cells(self) -> list[Flowcell]:
+        """Return the flow cells a sample has been sequenced on."""
+        return list({metric.flowcell for metric in self.sequencing_metrics})
 
     @property
     def sequencing_qc(self) -> bool:
         """Return sequencing qc passed or failed."""
         application = self.application_version.application
         # Express priority needs to be analyzed at a lower threshold for primary analysis
         if self.priority == Priority.express:
@@ -863,16 +860,14 @@
     @property
     def state(self) -> str:
         """Get the current sample state."""
         if self.delivered_at:
             return f"Delivered {self.delivered_at.date()}"
         if self.last_sequenced_at:
             return f"Sequenced {self.last_sequenced_at.date()}"
-        if self.sequence_start:
-            return f"Sequencing {self.sequence_start.date()}"
         if self.received_at:
             return f"Received {self.received_at.date()}"
 
         return f"Ordered {self.ordered_at.date()}"
 
     @property
     def archive_location(self) -> str:
@@ -889,15 +884,15 @@
         data["priority"] = self.priority_human
         data["customer"] = self.customer.to_dict()
         data["application_version"] = self.application_version.to_dict()
         data["application"] = self.application_version.application.to_dict()
         if links:
             data["links"] = [link_obj.to_dict(family=True, parents=True) for link_obj in self.links]
         if flowcells:
-            data["flowcells"] = [flowcell_obj.to_dict() for flowcell_obj in self.flowcells]
+            data["flowcells"] = [flow_cell.to_dict() for flow_cell in self.flow_cells]
         return data
 
 
 class Invoice(Base):
     __tablename__ = "invoice"
     id: Mapped[PrimaryKeyInt]
     customer_id: Mapped[int] = mapped_column(ForeignKey("customer.id"))
@@ -985,10 +980,11 @@
     id: Mapped[PrimaryKeyInt]
     cases: Mapped[list[Case]] = orm.relationship(secondary=order_case, back_populates="orders")
     customer_id: Mapped[int] = mapped_column(ForeignKey("customer.id"))
     customer: Mapped[Customer] = orm.relationship(foreign_keys=[customer_id])
     order_date: Mapped[datetime] = mapped_column(default=datetime.now())
     ticket_id: Mapped[int] = mapped_column(unique=True, index=True)
     workflow: Mapped[str] = mapped_column(types.Enum(*(workflow.value for workflow in Workflow)))
+    is_delivered: Mapped[bool] = mapped_column(default=False)
 
     def to_dict(self):
         return to_dict(model_instance=self)
```

### Comparing `cg-59.9.1/cg/store/store.py` & `cg-60.0.0/cg/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/checksum/checksum.py` & `cg-60.0.0/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/click/EnumChoice.py` & `cg-60.0.0/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/commands.py` & `cg-60.0.0/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/date.py` & `cg-60.0.0/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/dict.py` & `cg-60.0.0/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/dispatcher.py` & `cg-60.0.0/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/email.py` & `cg-60.0.0/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/files.py` & `cg-60.0.0/cg/utils/files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/flask/enum.py` & `cg-60.0.0/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/time.py` & `cg-60.0.0/cg/utils/time.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/cg/utils/utils.py` & `cg-60.0.0/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/pyproject.toml` & `cg-60.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cg"
-version = "59.9.1"
+version = "60.0.0"
 description = "Clinical Genomics command center"
 authors = ["Clinical Genomics <support@clinicalgenomics.se>"]
 readme = "README.md"
 homepage = "https://github.com/Clinical-Genomics/cg"
 repository = "https://github.com/Clinical-Genomics/cg"
 classifiers = [
   "Programming Language :: Python",
@@ -45,14 +45,15 @@
 gunicorn = "*"
 requests = "*"
 sendmail-container = "*"
 werkzeug = "*"
 
 # Utils
 cachetools = "*"
+cryptography = "*"
 coloredlogs = "*"
 Jinja2 = ">=3.1.3"
 lxml = "*"
 marshmallow = "*"
 MarkupSafe = "*"
 openpyxl = "*"
 packaging = "*"
```

### Comparing `cg-59.9.1/tests/apps/conftest.py` & `cg-60.0.0/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/coverage/test_coverage.py` & `cg-60.0.0/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/crunchy/conftest.py` & `cg-60.0.0/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/crunchy/test_compress_fastq.py` & `cg-60.0.0/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/crunchy/test_config.py` & `cg-60.0.0/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/crunchy/test_crunchy.py` & `cg-60.0.0/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/crunchy/test_spring_decompression.py` & `cg-60.0.0/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/demultiplex/conftest.py` & `cg-60.0.0/tests/apps/demultiplex/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import pytest
 
 from cg.apps.demultiplex.sample_sheet.override_cycles_validator import OverrideCyclesValidator
 from cg.apps.demultiplex.sample_sheet.sample_models import (
     FlowCellSampleBcl2Fastq,
     FlowCellSampleBCLConvert,
 )
-from cg.apps.demultiplex.sample_sheet.sample_sheet_creator import SampleSheetCreatorBcl2Fastq
-from cg.constants.demultiplexing import SampleSheetBcl2FastqSections
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.constants.demultiplexing import SampleSheetBcl2FastqSections, SampleSheetBCLConvertSections
 
 
 @pytest.fixture
 def bcl_convert_samples_similar_index1() -> list[FlowCellSampleBCLConvert]:
     """Return a list of three FlowCellSampleBCLConvert with updated indexes."""
     sample_1 = FlowCellSampleBCLConvert(
         lane=1, sample_id="ACC123", index="CAGAAGAT", index2="GCGCAAGC"
@@ -38,26 +36,14 @@
     )
     sample_3 = FlowCellSampleBCLConvert(
         lane=2, sample_id="ACC789", index="AAGCGATA", index2="AACCGCAA"
     )
     return [sample_1, sample_2, sample_3]
 
 
-@pytest.fixture
-def bcl2fastq_sample_sheet_creator(
-    novaseq_6000_pre_1_5_kits_flow_cell_bcl2fastq: FlowCellDirectoryData,
-    novaseq_6000_pre_1_5_kits_bcl2fastq_lims_samples: list[FlowCellSampleBcl2Fastq],
-) -> SampleSheetCreatorBcl2Fastq:
-    """Returns a sample sheet creator for version 1 sample sheets with bcl2fastq format."""
-    return SampleSheetCreatorBcl2Fastq(
-        flow_cell=novaseq_6000_pre_1_5_kits_flow_cell_bcl2fastq,
-        lims_samples=novaseq_6000_pre_1_5_kits_bcl2fastq_lims_samples,
-    )
-
-
 # Sample sheet validation
 
 
 @pytest.fixture
 def sample_sheet_line_sample_1() -> list[str]:
     """Return the line in the sample sheet corresponding to a sample."""
     return [
@@ -105,14 +91,35 @@
             SampleSheetBcl2FastqSections.Data.SAMPLE_REFERENCE.value,
             SampleSheetBcl2FastqSections.Data.INDEX_1.value,
             SampleSheetBcl2FastqSections.Data.INDEX_2.value,
             SampleSheetBcl2FastqSections.Data.SAMPLE_NAME.value,
             SampleSheetBcl2FastqSections.Data.CONTROL.value,
             SampleSheetBcl2FastqSections.Data.RECIPE.value,
             SampleSheetBcl2FastqSections.Data.OPERATOR.value,
+            SampleSheetBcl2FastqSections.Data.SAMPLE_PROJECT_BCL2FASTQ.value,
+        ],
+    ]
+
+
+@pytest.fixture
+def sample_sheet_bcl2fastq_data_header_with_replaced_sample_id() -> list[list[str]]:
+    """Return the content of a Bcl2fastq sample sheet data header without samples."""
+    return [
+        [SampleSheetBcl2FastqSections.Data.HEADER],
+        [
+            SampleSheetBcl2FastqSections.Data.FLOW_CELL_ID.value,
+            SampleSheetBcl2FastqSections.Data.LANE.value,
+            SampleSheetBCLConvertSections.Data.SAMPLE_INTERNAL_ID.value,
+            SampleSheetBcl2FastqSections.Data.SAMPLE_REFERENCE.value,
+            SampleSheetBcl2FastqSections.Data.INDEX_1.value,
+            SampleSheetBcl2FastqSections.Data.INDEX_2.value,
+            SampleSheetBcl2FastqSections.Data.SAMPLE_NAME.value,
+            SampleSheetBcl2FastqSections.Data.CONTROL.value,
+            SampleSheetBcl2FastqSections.Data.RECIPE.value,
+            SampleSheetBcl2FastqSections.Data.OPERATOR.value,
             SampleSheetBcl2FastqSections.Data.SAMPLE_PROJECT_BCL2FASTQ.value,
         ],
     ]
 
 
 @pytest.fixture
 def sample_sheet_samples_no_header(
```

### Comparing `cg-59.9.1/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-60.0.0/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,38 +52,14 @@
     # WHEN testing if the sample sheet is in Housekeeper
     result: bool = demux_api.is_sample_sheet_in_housekeeper(flow_cell_id=tmp_bcl2fastq_flow_cell.id)
 
     # THEN the sample sheet should be in Housekeeper
     assert not result
 
 
-def test_create_demultiplexing_output_dir_for_bcl2fastq(
-    tmp_bcl2fastq_flow_cell: FlowCellDirectoryData,
-    tmp_path: Path,
-    demultiplexing_api: DemultiplexingAPI,
-):
-    """Test that the correct demultiplexing output directory is created."""
-    # GIVEN a Bcl2Fastq FlowCellDirectoryData object
-
-    # GIVEN that the demultiplexing output directory does not exist
-    demultiplexing_api.demultiplexed_runs_dir = tmp_path
-    output_directory: Path = demultiplexing_api.flow_cell_out_dir_path(tmp_bcl2fastq_flow_cell)
-    unaligned_dir: Path = demultiplexing_api.get_flow_cell_unaligned_dir(tmp_bcl2fastq_flow_cell)
-
-    assert not output_directory.exists()
-    assert not unaligned_dir.exists()
-
-    # WHEN creating the demultiplexing output directory for a bcl2fastq flow cell
-    demultiplexing_api.create_demultiplexing_output_dir(tmp_bcl2fastq_flow_cell)
-
-    # THEN the demultiplexing output directory should exist
-    assert output_directory.exists()
-    assert unaligned_dir.exists()
-
-
 def test_create_demultiplexing_output_dir_for_bcl_convert(
     tmp_bcl_convert_flow_cell: FlowCellDirectoryData,
     tmp_path: Path,
     demultiplexing_api: DemultiplexingAPI,
 ):
     """Test that the correct demultiplexing output directory is created."""
     # GIVEN BCL Convert FlowCellDirectoryData object
```

### Comparing `cg-59.9.1/tests/apps/demultiplex/test_index.py` & `cg-60.0.0/tests/apps/demultiplex/test_index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,19 @@
 """Tests for functions related to indexes."""
 
 import pytest
 
 from cg.apps.demultiplex.sample_sheet.index import (
-    Index,
     get_hamming_distance_index_1,
     get_hamming_distance_index_2,
     get_reverse_complement_dna_seq,
-    get_valid_indexes,
     is_padding_needed,
 )
 
 
-def test_get_valid_indexes():
-    """Test that the function get_valid_indexes returns a list of Index objects."""
-    # GIVEN a sample sheet API
-
-    # WHEN fetching the indexes
-    indexes: list[Index] = get_valid_indexes()
-
-    # THEN assert that the indexes are correct
-    assert indexes
-    assert isinstance(indexes[0], Index)
-
-
 @pytest.mark.parametrize(
     "index1_cycles, index2_cycles, sample_index_length, expected_is_padding_needed",
     [
         (10, 10, 8, True),
         (10, 10, 10, False),
         (17, 8, 17, False),
         (8, 8, 10, False),
```

### Comparing `cg-59.9.1/tests/apps/demultiplex/test_override_cycles_validator.py` & `cg-60.0.0/tests/apps/demultiplex/test_override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-60.0.0/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files 12% similar despite different names*

```diff
@@ -137,29 +137,7 @@
     content: list[list[str]] = ReadFile.get_content_from_file(
         file_format=FileFormat.CSV, file_path=bcl2fastq_sample_sheet_path
     )
     sample_type: Type[FlowCellSample] = get_sample_type_from_content(content)
 
     # THEN the sample type is FlowCellSampleBCLConvert
     assert sample_type is FlowCellSampleBcl2Fastq
-
-
-def test_validate_sample_sheet_bcl2fastq_duplicate_same_lane(
-    sample_sheet_bcl2fastq_duplicate_same_lane: list[list[str]],
-):
-    """Test that creating a Bcl2fastq sample sheet with duplicated samples in a lane fails."""
-    # GIVEN a Bcl2fastq sample sheet with a sample duplicated in a lane
-
-    # WHEN creating the sample sheet object
-
-    # THEN a sample sheet error is raised
-
-
-def test_validate_sample_sheet_bcl2fastq_duplicate_different_lanes(
-    sample_sheet_bcl2fastq_duplicate_different_lane: list[list[str]],
-):
-    """Test that Bcl2fastq a sample sheet created with duplicated samples in different lanes has samples."""
-    # GIVEN a Bcl2fastq sample sheet with same sample duplicated in different lanes
-
-    # WHEN creating the sample sheet object
-
-    # THEN a sample sheet is returned with samples in it
```

### Comparing `cg-59.9.1/tests/apps/demultiplex/test_sample_models.py` & `cg-60.0.0/tests/apps/demultiplex/test_sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,101 @@
-"""Tests for the SampleSheetCreator classes."""
+"""Fixtures for parsed raw LIMS samples for demultiplexing and sample sheet creation."""
 
 from pathlib import Path
 
 import pytest
 
-from cg.apps.demultiplex.sample_sheet.read_sample_sheet import get_flow_cell_samples_from_content
 from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSample,
     FlowCellSampleBcl2Fastq,
     FlowCellSampleBCLConvert,
 )
-from cg.apps.demultiplex.sample_sheet.sample_sheet_creator import (
-    SampleSheetCreator,
-    SampleSheetCreatorBcl2Fastq,
-    SampleSheetCreatorBCLConvert,
-)
-from cg.constants.demultiplexing import BclConverter
-from cg.exc import SampleSheetError
+from cg.apps.demultiplex.sample_sheet.sample_sheet_creator import SampleSheetCreator
+from cg.constants import FileExtensions
+from cg.io.json import read_json
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 
 
-def test_bcl_convert_sample_sheet_fails_with_bcl2fastq(
-    novaseq_x_flow_cell: FlowCellDirectoryData,
-    novaseq_x_lims_samples: list[FlowCellSampleBCLConvert],
-):
-    """Test that creating a BCL Convert sample sheet fails if the bcl converter is Bcl2fastq."""
-    # GIVEN a NovaSeqX flow cell and samples and the bcl converter is Bcl2fastq
-    novaseq_x_flow_cell.bcl_converter = BclConverter.BCL2FASTQ
-
-    # WHEN trying to instantiate a SampleSheetCreatorBCLConvert with Bcl2fastq as bcl_converter
-    with pytest.raises(SampleSheetError) as exc_info:
-        SampleSheetCreatorBCLConvert(
-            flow_cell=novaseq_x_flow_cell,
-            lims_samples=novaseq_x_lims_samples,
-        )
-        # THEN an error is raised
-        assert (
-            str(exc_info.value)
-            == f"Can't use {BclConverter.BCL2FASTQ} with BCL Convert sample sheet"
-        )
-
-
-def test_construct_bcl2fastq_sheet(
-    bcl2fastq_sample_sheet_creator: SampleSheetCreatorBcl2Fastq, project_dir: Path
-):
-    """Test that a created Bcl2fastq sample sheet has samples."""
-    # GIVEN a Bcl2fastq sample sheet creator populated with Bcl2fastq samples
-    assert bcl2fastq_sample_sheet_creator.lims_samples
-
-    # WHEN building the sample sheet content
-    content: list[list[str]] = bcl2fastq_sample_sheet_creator.construct_sample_sheet()
-
-    # THEN a correctly formatted sample sheet was created
-    samples: list[FlowCellSample] = get_flow_cell_samples_from_content(
-        sample_sheet_content=content, sample_type=FlowCellSampleBcl2Fastq
+@pytest.fixture
+def hiseq_x_single_index_bcl_convert_lims_samples(
+    hiseq_x_single_index_flow_cell_dir: Path,
+) -> list[FlowCellSampleBCLConvert]:
+    """Return a list of BCLConvert samples parsed from LIMS for a HiSeqX single index flow cell."""
+    path = Path(
+        hiseq_x_single_index_flow_cell_dir, f"HJCFFALXX_bcl_convert_raw{FileExtensions.JSON}"
     )
-    assert samples
+    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
 
 
-def test_construct_bcl_convert_sheet(
-    bcl_convert_sample_sheet_creator: SampleSheetCreator, project_dir: Path
-):
-    """Test that a created BCL Convert sample sheet has samples."""
-    # GIVEN a BCL convert sample sheet creator populated with BCL convert samples
-    assert bcl_convert_sample_sheet_creator.lims_samples
-
-    # WHEN building the sample sheet content
-    content: list[list[str]] = bcl_convert_sample_sheet_creator.construct_sample_sheet()
-
-    # THEN a correctly formatted sample sheet was created
-    samples: list[FlowCellSample] = get_flow_cell_samples_from_content(
-        sample_sheet_content=content, sample_type=FlowCellSampleBCLConvert
-    )
-    assert samples
+@pytest.fixture
+def hiseq_x_dual_index_bcl_convert_lims_samples(
+    hiseq_x_dual_index_flow_cell_dir: Path,
+) -> list[FlowCellSampleBCLConvert]:
+    """Return a list of BCLConvert samples parsed from LIMS for a HiSeqX dual index flow cell."""
+    path = Path(hiseq_x_dual_index_flow_cell_dir, f"HL32LCCXY_bcl_convert_raw{FileExtensions.JSON}")
+    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
 
 
-def test_remove_unwanted_samples_dual_index(
-    novaseq6000_flow_cell_sample_before_adapt_indexes: FlowCellSampleBcl2Fastq,
-    hiseq_x_single_index_flow_cell: FlowCellDirectoryData,
-):
-    """Test that a sample with dual index is not removed."""
-    # GIVEN a sample sheet creator with a sample with dual index
-    sample_sheet_creator: SampleSheetCreatorBcl2Fastq = SampleSheetCreatorBcl2Fastq(
-        flow_cell=hiseq_x_single_index_flow_cell,
-        lims_samples=[novaseq6000_flow_cell_sample_before_adapt_indexes],
-    )
+@pytest.fixture
+def hiseq_2500_dual_index_bcl_convert_lims_samples(
+    hiseq_2500_dual_index_flow_cell_dir: Path,
+) -> list[FlowCellSampleBCLConvert]:
+    """Return a list of BCLConvert samples parsed from LIMS for a HiSeq2500 dual index flow cell."""
+    path = Path(hiseq_2500_dual_index_flow_cell_dir, "HM2LNBCX2_bcl_convert_raw.json")
+    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
 
-    # WHEN removing unwanted samples
-    sample_sheet_creator.remove_samples_with_simple_index()
 
-    # THEN the sample is not removed
-    assert len(sample_sheet_creator.lims_samples) == 1
+@pytest.fixture
+def hiseq_2500_custom_index_bcl_convert_lims_samples(
+    hiseq_2500_custom_index_flow_cell_dir: Path,
+) -> list[FlowCellSampleBCLConvert]:
+    """Return a list of BCLConvert samples parsed from LIMS for a HiSeq2500 custom index flow cell."""
+    path = Path(hiseq_2500_custom_index_flow_cell_dir, "HGYFNBCX2_bcl_convert_raw.json")
+    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
 
 
-def test_remove_unwanted_samples_no_dual_index(
-    novaseq6000_flow_cell_sample_no_dual_index: FlowCellSampleBcl2Fastq,
-    novaseq_6000_post_1_5_kits_flow_cell: FlowCellDirectoryData,
-    caplog,
-):
-    """Test that samples with no dual index are removed."""
-    # GIVEN a sample sheet creator with a sample without dual indexes
-    sample_sheet_creator: SampleSheetCreatorBcl2Fastq = SampleSheetCreatorBcl2Fastq(
-        flow_cell=novaseq_6000_post_1_5_kits_flow_cell,
-        lims_samples=[novaseq6000_flow_cell_sample_no_dual_index],
-    )
+@pytest.fixture
+def novaseq_6000_pre_1_5_kits_bcl2fastq_lims_samples(
+    novaseq_6000_pre_1_5_kits_flow_cell_path: Path,
+) -> list[FlowCellSampleBcl2Fastq]:
+    """Return a list of Bcl2Fastq samples parsed from LIMS for a NovaSeq6000 pre 1.5 flow cell."""
+    path = Path(novaseq_6000_pre_1_5_kits_flow_cell_path, "HLYWYDSXX_bcl2fastq_raw.json")
+    return [FlowCellSampleBcl2Fastq.model_validate(sample) for sample in read_json(path)]
+
+
+@pytest.fixture
+def novaseq_6000_pre_1_5_kits_bcl_convert_lims_samples(
+    novaseq_6000_pre_1_5_kits_flow_cell_path: Path,
+) -> list[FlowCellSampleBCLConvert]:
+    """Return a list of BCLConvert samples parsed from LIMS for a NovaSeq6000 pre 1.5 flow cell."""
+    path = Path(novaseq_6000_pre_1_5_kits_flow_cell_path, "HLYWYDSXX_bcl_convert_raw.json")
+    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
 
-    # WHEN removing unwanted samples
-    sample_sheet_creator.remove_samples_with_simple_index()
 
-    # THEN the only sample is removed
-    assert len(sample_sheet_creator.lims_samples) == 0
-    assert (
-        f"Removing sample {novaseq6000_flow_cell_sample_no_dual_index.sample_id} since it does not have dual index"
-        in caplog.text
+@pytest.fixture
+def novaseq_6000_post_1_5_kits_bcl_convert_lims_samples(
+    novaseq_6000_post_1_5_kits_flow_cell_path: Path,
+) -> list[FlowCellSampleBCLConvert]:
+    """Return a list of BCLConvert samples parsed from LIMS for a NovaSeq6000 post 1.5 flow cell."""
+    path = Path(novaseq_6000_post_1_5_kits_flow_cell_path, "HK33MDRX3_bcl_convert_raw.json")
+    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
+
+
+@pytest.fixture
+def novaseq_x_lims_samples(novaseq_x_flow_cell_directory: Path) -> list[FlowCellSampleBCLConvert]:
+    """Return a list of BCLConvert samples parsed from LIMS for a NovaSeqX flow cell."""
+    path = Path(novaseq_x_flow_cell_directory, "22F52TLT3_raw.json")
+    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
+
+
+# Sample sheet creators
+
+
+@pytest.fixture
+def bcl_convert_sample_sheet_creator(
+    novaseq_x_flow_cell: FlowCellDirectoryData,
+    novaseq_x_lims_samples: list[FlowCellSampleBCLConvert],
+) -> SampleSheetCreator:
+    """Returns a sample sheet creator for sample sheet v2."""
+    return SampleSheetCreator(
+        flow_cell=novaseq_x_flow_cell,
+        lims_samples=novaseq_x_lims_samples,
     )
```

### Comparing `cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_creator_factory.py` & `cg-60.0.0/tests/apps/demultiplex/test_validate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,32 @@
-"""Tests for the creation of the sample sheet"""
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBcl2Fastq
+from cg.apps.demultiplex.sample_sheet.validators import is_valid_sample_internal_id
 
-from cg.apps.demultiplex.sample_sheet.create import get_sample_sheet_creator
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
-from cg.apps.demultiplex.sample_sheet.sample_sheet_creator import (
-    SampleSheetCreator,
-    SampleSheetCreatorBcl2Fastq,
-    SampleSheetCreatorBCLConvert,
-)
-from cg.constants.demultiplexing import BclConverter
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
-
-
-def test_sample_sheet_creator_factory_novaseq_6000(
-    novaseq_6000_pre_1_5_kits_flow_cell_bcl2fastq: FlowCellDirectoryData,
-    novaseq_6000_pre_1_5_kits_bcl2fastq_lims_samples: list[FlowCellSampleBcl2Fastq],
-):
-    """Test that a sample sheet creator defined with NovaSeq6000 data is V1."""
-    # GIVEN a NovaSeq6000 flow cell and a list of NovaSeq6000 samples
-
-    # GIVEN that the flow cell is demultiplexed with bcl2fastq
-    assert novaseq_6000_pre_1_5_kits_flow_cell_bcl2fastq.bcl_converter == BclConverter.BCL2FASTQ
 
-    # WHEN defining the sample sheet creator
-    sample_sheet_creator: SampleSheetCreator = get_sample_sheet_creator(
-        flow_cell=novaseq_6000_pre_1_5_kits_flow_cell_bcl2fastq,
-        lims_samples=novaseq_6000_pre_1_5_kits_bcl2fastq_lims_samples,
-    )
+def test_is_valid_sample_internal_id(
+    novaseq6000_flow_cell_sample_1: FlowCellSampleBcl2Fastq,
+    novaseq6000_flow_cell_sample_2: FlowCellSampleBcl2Fastq,
+):
+    """Test that validating two different samples finishes successfully."""
+    # GIVEN two different NovaSeq samples with valid internal IDs
 
-    # THEN no error is raised and the sample sheet creator is a Bcl2Fastq sample sheet creator
-    assert isinstance(sample_sheet_creator, SampleSheetCreatorBcl2Fastq)
+    # WHEN validating the sample internal ids
+    for sample in [novaseq6000_flow_cell_sample_1, novaseq6000_flow_cell_sample_2]:
+        # THEN no error is raised
+        assert is_valid_sample_internal_id(sample_internal_id=sample.sample_id)
 
 
-def test_sample_sheet_creator_factory_bcl_convert(
-    novaseq_x_flow_cell: FlowCellDirectoryData,
-    novaseq_x_lims_samples: list[FlowCellSampleBCLConvert],
+def test_is_valid_sample_internal_id_invalid_sample_internal_ids(
+    novaseq6000_flow_cell_sample_1: FlowCellSampleBcl2Fastq,
+    novaseq6000_flow_cell_sample_2: FlowCellSampleBcl2Fastq,
 ):
-    """Test that a sample sheet creator defined with BCL convert data is BCL Convert."""
-
-    # GIVEN a NovaSeqX flow cell and a list of NovaSeqX BCL Convert samples
-    assert novaseq_x_flow_cell.bcl_converter == BclConverter.BCLCONVERT
-
-    # WHEN defining the sample sheet creator
-    sample_sheet_creator: SampleSheetCreator = get_sample_sheet_creator(
-        flow_cell=novaseq_x_flow_cell,
-        lims_samples=novaseq_x_lims_samples,
-    )
+    """Test that validating two different samples finishes successfully."""
+    # GIVEN two different NovaSeq samples with valid internal IDs
 
-    # THEN the sample sheet creator is a BCL Convert sample sheet creator
-    assert isinstance(sample_sheet_creator, SampleSheetCreatorBCLConvert)
+    # WHEN setting the sample internal ids to invalid values
+    novaseq6000_flow_cell_sample_1.sample_id = "invalid_sample_id"
+    novaseq6000_flow_cell_sample_2.sample_id = "invalid_sample_id"
+
+    # WHEN validating the sample internal ids
+    # THEN no error is raised
+    for sample in [novaseq6000_flow_cell_sample_1, novaseq6000_flow_cell_sample_2]:
+        assert not is_valid_sample_internal_id(sample_internal_id=sample.sample_id)
```

### Comparing `cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_models.py` & `cg-60.0.0/tests/apps/demultiplex/test_sample_sheet_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from pathlib import Path
-
 from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBCLConvert
 from cg.apps.demultiplex.sample_sheet.sample_sheet_models import SampleSheet
 from cg.apps.demultiplex.sample_sheet.sample_sheet_validator import SampleSheetValidator
 from cg.apps.demultiplex.sample_sheet.validators import is_valid_sample_internal_id
 
 
 def test_get_non_pooled_samples_when_no_samples():
```

### Comparing `cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_validator.py` & `cg-60.0.0/tests/apps/demultiplex/test_sample_sheet_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,41 +247,35 @@
         sample_sheet_validator._validate_override_cycles()
 
 
 @pytest.mark.parametrize(
     "sample_sheet_content",
     [
         "hiseq_x_single_index_sample_sheet_content",
-        "hiseq_x_single_index_bcl2fastq_sample_sheet_content",
         "hiseq_x_dual_index_sample_sheet_content",
-        "hiseq_x_dual_index_bcl2fastq_sample_sheet_content",
         "hiseq_2500_dual_index_sample_sheet_content",
-        "hiseq_2500_dual_index_bcl2fastq_sample_sheet_content",
         "hiseq_2500_custom_index_sample_sheet_content",
-        "hiseq_2500_custom_index_bcl2fastq_sample_sheet_content",
         "novaseq_6000_pre_1_5_kits_sample_sheet_content",
         "novaseq_6000_post_1_5_kits_sample_sheet_content",
         "novaseq_x_sample_sheet_content",
     ],
     ids=[
         "HiSeqXSingleIndex",
-        "HiSeqXSingleIndexBcl2Fastq",
         "HiSeqXDualIndex",
-        "HiSeqXDualIndexBcl2Fastq",
         "HiSeq2500DualIndex",
-        "HiSeq2500DualIndexBcl2Fastq",
         "HiSeq2500CustomIndex",
-        "HiSeq2500CustomIndexBcl2Fastq",
         "NovaSeq6000Pre1.5Kits",
         "NovaSeq6000Post1.5Kits",
         "NovaSeqX",
     ],
 )
 def test_validate_sample_sheet_from_content(
-    sample_sheet_validator: SampleSheetValidator, sample_sheet_content: str, request: FixtureRequest
+    sample_sheet_validator: SampleSheetValidator,
+    sample_sheet_content: str,
+    request: FixtureRequest,
 ):
     """Test that a correct sample sheet passes validation."""
     # GIVEN sample sheet validator and a correct sample sheet content
     content: list[list[str]] = request.getfixturevalue(sample_sheet_content)
 
     # WHEN validating the sample sheet
     sample_sheet_validator.validate_sample_sheet_from_content(content)
```

### Comparing `cg-59.9.1/tests/apps/downsample/test_downsample.py` & `cg-60.0.0/tests/apps/downsample/test_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/downsample/test_downsample_utils.py` & `cg-60.0.0/tests/apps/downsample/test_downsample_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/gens/test_gens_api.py` & `cg-60.0.0/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/gt/conftest.py` & `cg-60.0.0/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/gt/test_gt_api.py` & `cg-60.0.0/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/hk/conftest.py` & `cg-60.0.0/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/hk/test__getattr__.py` & `cg-60.0.0/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/hk/test_add_file.py` & `cg-60.0.0/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/hk/test_bundles.py` & `cg-60.0.0/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/hk/test_core.py` & `cg-60.0.0/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/hk/test_file.py` & `cg-60.0.0/tests/apps/hk/test_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -660,7 +660,166 @@
     # GIVEN the path of a file in Housekeeper API
 
     # WHEN getting the file though the path
     file: File = populated_housekeeper_api.get_file_insensitive_path(path=bed_file)
 
     # THEN the file is fetched correctly
     assert file
+
+
+def test_get_files_containing_tags(
+    populated_housekeeper_api: HousekeeperAPI, sample_id: str, fastq_file: Path, spring_file: Path
+):
+    """Test get files containing specific tags."""
+
+    # GIVEN a populated Housekeeper API and a list of sample files
+    files: list[File] = populated_housekeeper_api.get_files_from_latest_version(sample_id)
+    files_names: list[str] = [Path(file.full_path).name for file in files]
+    assert spring_file.name in files_names
+    assert fastq_file.name in files_names
+
+    # GIVEN a list of fastq file tags
+    tags: list[set[str]] = [{SequencingFileTag.FASTQ}]
+
+    # WHEN getting a list of files with tags
+    filtered_files: list[File] = populated_housekeeper_api.get_files_containing_tags(
+        files=files, tags=tags
+    )
+
+    # THEN only the expected fastq sample files should be retrieved
+    filtered_files_names: list[str] = [Path(file.full_path).name for file in filtered_files]
+    assert fastq_file.name in filtered_files_names
+    assert spring_file.name not in filtered_files_names
+
+
+def test_get_files_when_using_no_tags(
+    populated_housekeeper_api: HousekeeperAPI, sample_id: str, empty_list: list
+):
+    """Test get files containing an empty list of tags."""
+
+    # GIVEN a populated Housekeeper API and a list of sample files
+    files: list[File] = populated_housekeeper_api.get_files_from_latest_version(sample_id)
+
+    # WHEN getting a list of files providing an empty list of tags
+    filtered_files: list[File] = populated_housekeeper_api.get_files_containing_tags(
+        files=files, tags=empty_list
+    )
+
+    # THEN an empty list should be returned
+    assert filtered_files == empty_list
+
+
+def test_filter_files_without_tags(
+    populated_housekeeper_api: HousekeeperAPI, sample_id: str, fastq_file: Path, spring_file: Path
+):
+    """Test get files without specific tags."""
+
+    # GIVEN a populated Housekeeper API and a list of sample files
+    files: list[File] = populated_housekeeper_api.get_files_from_latest_version(sample_id)
+    files_names: list[str] = [Path(file.full_path).name for file in files]
+    assert spring_file.name in files_names
+    assert fastq_file.name in files_names
+
+    # GIVEN a list of fastq file tags to exclude
+    excluded_tags: list[str] = [SequencingFileTag.FASTQ]
+
+    # WHEN getting a list of files lacking excluded tags
+    filtered_files: list[File] = populated_housekeeper_api.get_files_without_excluded_tags(
+        files=files, excluded_tags=excluded_tags
+    )
+
+    # THEN only the expected sample spring files should be retrieved
+    filtered_files_names: list[str] = [Path(file.full_path).name for file in filtered_files]
+    assert spring_file.name in filtered_files_names
+    assert fastq_file.name not in filtered_files_names
+
+
+def test_get_files_without_excluded_tags_using_no_tags(
+    populated_housekeeper_api: HousekeeperAPI,
+    sample_id: str,
+    fastq_file: Path,
+    spring_file: Path,
+    empty_list: list,
+):
+    """Test get files without tags for an empty tag input."""
+
+    # GIVEN a populated Housekeeper API and a list of sample files
+    files: list[File] = populated_housekeeper_api.get_files_from_latest_version(sample_id)
+
+    # WHEN getting a list of files without tags when providing an empty list of tags
+    filtered_files: list[File] = populated_housekeeper_api.get_files_without_excluded_tags(
+        files=files, excluded_tags=empty_list
+    )
+
+    # THEN the complete list of original files should be returned
+    assert filtered_files == files
+
+
+def test_get_files_from_latest_version_containing_tags(
+    populated_housekeeper_api: HousekeeperAPI, sample_id: str, fastq_file: Path, spring_file: Path
+):
+    """Test get files from latest version by tags."""
+
+    # GIVEN a populated Housekeeper API
+
+    # GIVEN a list of fastq file tags
+    tags: list[set[str]] = [{SequencingFileTag.FASTQ}]
+
+    # WHEN getting a list of files that match specific tags
+    filtered_files: list[File] = (
+        populated_housekeeper_api.get_files_from_latest_version_containing_tags(
+            bundle_name=sample_id, tags=tags
+        )
+    )
+
+    # THEN only the expected fastq sample files should be returned
+    filtered_files_names: list[str] = [Path(file.full_path).name for file in filtered_files]
+    assert fastq_file.name in filtered_files_names
+    assert spring_file.name not in filtered_files_names
+
+
+def test_get_files_from_latest_version_using_no_tags(
+    populated_housekeeper_api: HousekeeperAPI,
+    sample_id: str,
+    fastq_file: Path,
+    spring_file: Path,
+    empty_list: list,
+):
+    """Test get files from the latest version by empty list of tags."""
+
+    # GIVEN a populated Housekeeper API
+
+    # WHEN getting a list of files that match empty tags
+    filtered_files: list[File] = (
+        populated_housekeeper_api.get_files_from_latest_version_containing_tags(
+            bundle_name=sample_id, tags=empty_list
+        )
+    )
+
+    # THEN an empty list should be returned
+    assert filtered_files == empty_list
+
+
+def test_get_files_from_latest_version_containing_tags_and_excluded_tags(
+    populated_housekeeper_api: HousekeeperAPI, sample_id: str, fastq_file: Path, spring_file: Path
+):
+    """Test get files from the latest version by tags and excluded tags."""
+
+    # GIVEN a populated Housekeeper API
+
+    # GIVEN a list of sample id tags
+    tags: list[set[str]] = [{sample_id}]
+
+    # GIVEN a list of fastq file tags to exclude
+    excluded_tags: list[str] = [SequencingFileTag.FASTQ]
+
+    # WHEN getting a list of files that match the sample ID tag and exclude the fastq files
+    filtered_files: list[File] = (
+        populated_housekeeper_api.get_files_from_latest_version_containing_tags(
+            bundle_name=sample_id, tags=tags, excluded_tags=excluded_tags
+        )
+    )
+
+    # THEN only the expected fastq sample files should be returned
+    filtered_files_names: list[str] = [Path(file.full_path).name for file in filtered_files]
+    assert spring_file.name in filtered_files_names
+    assert fastq_file.name not in filtered_files_names
```

### Comparing `cg-59.9.1/tests/apps/hk/test_version.py` & `cg-60.0.0/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/lims/conftest.py` & `cg-60.0.0/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/lims/test_api.py` & `cg-60.0.0/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/lims/test_sample_sheet.py` & `cg-60.0.0/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/loqus/conftest.py` & `cg-60.0.0/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/loqus/test_loqusdb_api.py` & `cg-60.0.0/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/madeline/conftest.py` & `cg-60.0.0/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/madeline/test_madeline.py` & `cg-60.0.0/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/mip/conftest.py` & `cg-60.0.0/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/mip/test_config_mip.py` & `cg-60.0.0/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/mutacc_auto/conftest.py` & `cg-60.0.0/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-60.0.0/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/orderform/conftest.py` & `cg-60.0.0/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-60.0.0/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/orderform/test_excel_sample_schema.py` & `cg-60.0.0/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/orderform/test_json_orderform_parser.py` & `cg-60.0.0/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/orderform/test_orderform_parser.py` & `cg-60.0.0/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/orderform/validators/test_excel_sample_validators.py` & `cg-60.0.0/tests/apps/orderform/validators/test_excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/scout/conftest.py` & `cg-60.0.0/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/scout/test_get_causative_variants.py` & `cg-60.0.0/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/scout/test_get_scout_cases.py` & `cg-60.0.0/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/scout/test_scout_load_config.py` & `cg-60.0.0/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/scout/test_scout_models.py` & `cg-60.0.0/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-60.0.0/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py` & `cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py` & `cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py` & `cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-60.0.0/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py` & `cg-60.0.0/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/slurm/conftest.py` & `cg-60.0.0/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/slurm/test_slurm_api.py` & `cg-60.0.0/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/test_apps_environ.py` & `cg-60.0.0/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/apps/test_osticket.py` & `cg-60.0.0/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/add/test_cli_add.py` & `cg-60.0.0/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/add/test_cli_add_customer.py` & `cg-60.0.0/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/add/test_cli_add_family.py` & `cg-60.0.0/tests/cli/set/test_cli_set_case.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,235 +1,199 @@
-"""Tests the CLI methods to add cases to the status database."""
+"""This script tests the cli methods to set values of a case in status-db."""
 
 from click.testing import CliRunner
 
-from cg.cli.add import add
-from cg.constants import DataDelivery, Workflow
+from cg.cli.set.case import set_case
+from cg.constants import EXIT_SUCCESS, DataDelivery, Workflow
 from cg.models.cg_config import CGConfig
-from cg.store.models import Case, Customer, Panel
+from cg.store.models import Case
 from cg.store.store import Store
 from tests.store_helpers import StoreHelpers
 
-CLI_OPTION_ANALYSIS = Workflow.BALSAMIC_UMI
-CLI_OPTION_DELIVERY = DataDelivery.FASTQ_QC
+
+def test_set_case_without_options(
+    cli_runner: CliRunner,
+    base_context: CGConfig,
+    base_store: Store,
+    helpers: StoreHelpers,
+):
+    """Test to set a case using only the required arguments."""
+    # GIVEN a database with a case
+    case_id: str = helpers.add_case(store=base_store).internal_id
+    assert base_store._get_query(table=Case).count() == 1
+
+    # WHEN setting a case
+    result = cli_runner.invoke(set_case, [case_id], obj=base_context)
+
+    # THEN it should abort
+    assert result.exit_code != EXIT_SUCCESS
 
 
-def test_add_case_required(
-    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers, ticket_id: str
+def test_set_case_bad_family(
+    cli_runner: CliRunner, base_context: CGConfig, case_id_does_not_exist: str
 ):
-    """Test to add a case using only the required arguments"""
-    # GIVEN a database with a customer and an panel
-    disk_store: Store = base_context.status_db
-
-    customer: Customer = helpers.ensure_customer(store=disk_store)
-    customer_id = customer.internal_id
-    panel: Panel = helpers.ensure_panel(store=disk_store)
-    panel_id = panel.name
-    name = "case_name"
-
-    # WHEN adding a panel
-    result = cli_runner.invoke(
-        add,
-        [
-            "case",
-            "--panel",
-            panel_id,
-            "--analysis",
-            CLI_OPTION_ANALYSIS,
-            "--data-delivery",
-            CLI_OPTION_DELIVERY,
-            "--ticket",
-            ticket_id,
-            customer_id,
-            name,
-        ],
-        obj=base_context,
+    """Test to set a case using a non-existing case id."""
+    # GIVEN an empty database
+
+    # WHEN setting a case
+    result = cli_runner.invoke(set_case, [case_id_does_not_exist], obj=base_context)
+
+    # THEN it should complain on missing case
+    assert result.exit_code != EXIT_SUCCESS
+
+
+def test_set_case_bad_panel(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
+):
+    """Test to set a case using a non-existing panel."""
+    # GIVEN a database with a case
+
+    # WHEN setting a case
+    panel_id: str = "dummy_panel"
+    case_id: str = helpers.add_case(store=base_store).internal_id
+    result = cli_runner.invoke(set_case, [case_id, "--panel", panel_id], obj=base_context)
+
+    # THEN it should complain in missing panel instead of setting a value
+    assert result.exit_code != EXIT_SUCCESS
+    assert panel_id not in base_store._get_query(table=Case).first().panels
+
+
+def test_set_case_panel(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
+):
+    """Test to set a case using an existing panel."""
+    # GIVEN a database with a case and a panel not yet added to the case
+    panel_id: str = helpers.ensure_panel(store=base_store, panel_abbreviation="a_panel").name
+    case_id: str = helpers.add_case(store=base_store).internal_id
+    case_query = base_store._get_query(table=Case)
+
+    assert panel_id not in case_query.first().panels
+
+    # WHEN setting a panel of a case
+    result = cli_runner.invoke(set_case, [case_id, "--panel", panel_id], obj=base_context)
+
+    # THEN it should set panel on the case
+    assert result.exit_code == EXIT_SUCCESS
+    assert panel_id in case_query.first().panels
+
+
+def test_set_case_priority(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
+):
+    """Test that the added case gets the priority we send in."""
+    # GIVEN a database with a case
+    case_id: str = helpers.add_case(base_store).internal_id
+    priority: str = "priority"
+    case_query = base_store._get_query(table=Case)
+
+    assert case_query.first().priority_human != priority
+
+    # WHEN setting a case
+    result = cli_runner.invoke(
+        set_case, [case_id, "--priority", priority], obj=base_context, catch_exceptions=False
     )
 
-    # THEN it should be added
-    assert result.exit_code == 0
-    case_query = disk_store._get_query(table=Case)
+    # THEN it should have been set
+    assert result.exit_code == EXIT_SUCCESS
     assert case_query.count() == 1
-    assert case_query.first().name == name
-    assert case_query.first().panels == [panel_id]
+    assert case_query.first().priority_human == priority
 
 
-def test_add_case_bad_workflow(
-    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers, ticket_id: str
+def test_set_case_customer(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
 ):
-    """Test to add a case using only the required arguments"""
-    # GIVEN a database with a customer and a panel
-
-    # WHEN adding a case
-    disk_store: Store = base_context.status_db
-
-    customer: Customer = helpers.ensure_customer(store=disk_store)
-    customer_id = customer.internal_id
-    panel: Panel = helpers.ensure_panel(store=disk_store)
-    panel_id = panel.name
-    non_existing_analysis = "epigenentic_alterations"
-    name = "case_name"
-
-    result = cli_runner.invoke(
-        add,
-        [
-            "case",
-            "--panel",
-            panel_id,
-            "--analysis",
-            non_existing_analysis,
-            "--data-delivery",
-            CLI_OPTION_DELIVERY,
-            "--ticket",
-            ticket_id,
-            customer_id,
-            name,
-        ],
-    )
-
-    # THEN it should not be added
-    assert result.exit_code != 0
-    assert disk_store._get_query(table=Case).count() == 0
-
-
-def test_add_case_bad_data_delivery(
-    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers
-):
-    """Test to add a case using only the required arguments"""
-    # GIVEN a database with a customer and an panel
-
-    # WHEN adding a case without data delivery
-    disk_store: Store = base_context.status_db
-
-    customer: Customer = helpers.ensure_customer(store=disk_store)
-    customer_id = customer.internal_id
-    panel: Panel = helpers.ensure_panel(store=disk_store)
-    panel_id = panel.name
-    name = "case_name"
-    non_existing_data_delivery = "aws"
-
-    result = cli_runner.invoke(
-        add,
-        [
-            "case",
-            "--panel",
-            panel_id,
-            "--analysis",
-            CLI_OPTION_ANALYSIS,
-            "--data-delivery",
-            non_existing_data_delivery,
-            customer_id,
-            name,
-        ],
-        obj=base_context,
+    """Test to set a case using an existing customer."""
+    # GIVEN a database with a case and a customer not yet on the case
+    customer_id: str = helpers.ensure_customer(
+        store=base_store, customer_id="a_customer"
+    ).internal_id
+    case_to_alter: Case = helpers.add_case(store=base_store)
+    assert customer_id != case_to_alter.customer.internal_id
+
+    # WHEN setting a customer of a case
+    result = cli_runner.invoke(
+        set_case, [case_to_alter.internal_id, "--customer-id", customer_id], obj=base_context
     )
 
-    # THEN it should not be added
-    assert result.exit_code != 0
-    assert disk_store._get_query(table=Case).count() == 0
+    # THEN it should set customer on the case
+    assert result.exit_code == EXIT_SUCCESS
+    assert customer_id == case_to_alter.customer.internal_id
 
 
-def test_add_case_bad_customer(cli_runner: CliRunner, base_context: CGConfig, ticket_id: str):
-    """Test to add a case using a non-existing customer"""
-    # GIVEN an empty database
-    disk_store: Store = base_context.status_db
-    # WHEN adding a case
-    panel_id = "dummy_panel"
-    customer_id = "dummy_customer"
-    name = "dummy_name"
-    result = cli_runner.invoke(
-        add,
-        [
-            "case",
-            "--panel",
-            panel_id,
-            "--analysis",
-            CLI_OPTION_ANALYSIS,
-            "--data-delivery",
-            CLI_OPTION_DELIVERY,
-            "--ticket",
-            ticket_id,
-            customer_id,
-            name,
-        ],
-        obj=base_context,
+def test_set_case_bad_data_analysis(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
+):
+    """Test to set a case using a non-existing data_analysis."""
+    # GIVEN a database with a case
+
+    # WHEN setting a data_analysis on a case
+    data_analysis: str = "dummy_workflow"
+    case_id: str = helpers.add_case(store=base_store).internal_id
+    result = cli_runner.invoke(
+        set_case, [case_id, "--data-analysis", data_analysis], obj=base_context
     )
 
-    # THEN it should complain about missing customer instead of adding a case
-    assert result.exit_code == 1
-    assert disk_store._get_query(table=Case).count() == 0
-
-
-def test_add_case_bad_panel(
-    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers, ticket_id: str
-):
-    """Test to add a case using a non-existing panel"""
-    # GIVEN a database with a customer
-    disk_store: Store = base_context.status_db
-    # WHEN adding a case
-    customer: Customer = helpers.ensure_customer(store=disk_store)
-    customer_id = customer.internal_id
-    panel_id = "dummy_panel"
-    name = "dummy_name"
-    result = cli_runner.invoke(
-        add,
-        [
-            "case",
-            "--panel",
-            panel_id,
-            "--analysis",
-            CLI_OPTION_ANALYSIS,
-            "--data-delivery",
-            CLI_OPTION_DELIVERY,
-            "--ticket",
-            ticket_id,
-            customer_id,
-            name,
-        ],
+    # THEN it should complain in invalid data_analysis instead of setting a value
+    assert result.exit_code != EXIT_SUCCESS
+    assert str(data_analysis) != base_store._get_query(table=Case).first().data_analysis
+
+
+def test_set_case_data_analysis(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
+):
+    """Test to set a case using an existing data_analysis."""
+
+    # GIVEN a database with a case and a data_analysis not yet set on the case
+    data_analysis: str = Workflow.FASTQ
+    case_to_alter: str = helpers.add_case(base_store)
+    assert str(data_analysis) != case_to_alter.data_analysis
+
+    # WHEN setting a data_analysis of a case
+    result = cli_runner.invoke(
+        set_case,
+        [case_to_alter.internal_id, "--data-analysis", str(data_analysis)],
         obj=base_context,
     )
 
-    # THEN it should complain about missing panel instead of adding a case
-    assert result.exit_code == 1
-    assert disk_store._get_query(table=Case).count() == 0
-
-
-def test_add_case_priority(
-    cli_runner: CliRunner, base_context: CGConfig, helpers: StoreHelpers, ticket_id: str
-):
-    """Test that the added case get the priority we send in"""
-    # GIVEN a database with a customer and an panel
-    disk_store: Store = base_context.status_db
-    # WHEN adding a case
-    customer: Customer = helpers.ensure_customer(store=disk_store)
-    customer_id = customer.internal_id
-    panel: Panel = helpers.ensure_panel(store=disk_store)
-    panel_id = panel.name
-    name = "case_name"
-    priority = "priority"
-
-    result = cli_runner.invoke(
-        add,
-        [
-            "case",
-            "--panel",
-            panel_id,
-            "--priority",
-            priority,
-            "--analysis",
-            CLI_OPTION_ANALYSIS,
-            "--data-delivery",
-            CLI_OPTION_DELIVERY,
-            "--ticket",
-            ticket_id,
-            customer_id,
-            name,
-        ],
-        obj=base_context,
+    # THEN it should set data_analysis on the case
+    assert result.exit_code == EXIT_SUCCESS
+    assert str(data_analysis) == case_to_alter.data_analysis
+
+
+def test_set_case_bad_data_delivery(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
+):
+    """Test to set a case using a non-existing data_delivery."""
+    # GIVEN a database with a case
+
+    # WHEN setting a data_delivery on a case
+    data_delivery: str = "dummy_delivery"
+    case_id: str = helpers.add_case(base_store).internal_id
+    result = cli_runner.invoke(
+        set_case, [case_id, "--data-delivery", data_delivery], obj=base_context
     )
 
-    # THEN it should be added
-    assert result.exit_code == 0
-    case_query = disk_store._get_query(table=Case)
+    # THEN it should complain in invalid data_delivery instead of setting a value
+    assert result.exit_code != EXIT_SUCCESS
+    assert str(data_delivery) != base_store._get_query(table=Case).first().data_delivery
 
-    assert case_query.count() == 1
-    assert case_query.first().priority_human == priority
+
+def test_set_case_data_delivery(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
+):
+    """Test to set a case using an existing data_delivery."""
+
+    # GIVEN a database with a case and a data_delivery not yet set on the case
+    data_delivery: str = DataDelivery.FASTQ
+    case_to_alter: str = helpers.add_case(base_store)
+    assert str(data_delivery) != case_to_alter.data_delivery
+
+    # WHEN setting a data_delivery of a case
+    result = cli_runner.invoke(
+        set_case,
+        [case_to_alter.internal_id, "--data-delivery", str(data_delivery)],
+        obj=base_context,
+    )
+
+    # THEN it should set data_delivery on the case
+    assert result.exit_code == EXIT_SUCCESS
+    assert str(data_delivery) == case_to_alter.data_delivery
```

### Comparing `cg-59.9.1/tests/cli/add/test_cli_add_relationship.py` & `cg-60.0.0/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/add/test_cli_add_sample.py` & `cg-60.0.0/tests/cli/add/test_cli_add_sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,25 @@
     # GIVEN an empty database
     disk_store: Store = base_context.status_db
 
     # WHEN adding a sample
     application = "dummy_application"
     customer_id = "dummy_customer"
     name = "dummy_name"
+    original_ticket = "dummy ticket"
     result = cli_runner.invoke(
         add,
         [
             "sample",
             "--sex",
             Sex.MALE,
             "--application-tag",
             application,
+            "--original-ticket",
+            original_ticket,
             customer_id,
             name,
         ],
         obj=base_context,
     )
 
     # THEN it should complain about missing customer instead of adding a sample
@@ -44,22 +47,25 @@
     # GIVEN a database with a customer
     disk_store: Store = base_context.status_db
 
     # WHEN adding a sample
     application = "dummy_application"
     customer: Customer = helpers.ensure_customer(store=disk_store)
     name = "dummy_name"
+    original_ticket = "dummy ticket"
     result = cli_runner.invoke(
         add,
         [
             "sample",
             "--sex",
             Sex.MALE,
             "--application-tag",
             application,
+            "--original-ticket",
+            original_ticket,
             customer.internal_id,
             name,
         ],
         obj=base_context,
     )
 
     # THEN it should complain about missing application instead of adding a sample
@@ -72,24 +78,26 @@
     # GIVEN a database with a customer and an application
     disk_store: Store = base_context.status_db
     application_tag = "dummy_tag"
     helpers.ensure_application(store=disk_store, tag=application_tag)
     helpers.ensure_application_version(store=disk_store, application_tag=application_tag)
     customer: Customer = helpers.ensure_customer(store=disk_store)
     name = "sample_name"
-
+    original_ticket = "dummy ticket"
     # WHEN adding a sample
     result = cli_runner.invoke(
         add,
         [
             "sample",
             "--sex",
             Sex.MALE,
             "--application-tag",
             application_tag,
+            "--original-ticket",
+            original_ticket,
             customer.internal_id,
             name,
         ],
         obj=base_context,
     )
 
     # THEN it should be added
@@ -107,23 +115,25 @@
     application_tag = "dummy_tag"
     helpers.ensure_application(store=disk_store, tag=application_tag)
     helpers.ensure_application_version(store=disk_store, application_tag=application_tag)
     # WHEN adding a sample
     customer: Customer = helpers.ensure_customer(store=disk_store)
     name = "sample_name"
     lims_id = "sample_lims_id"
-
+    original_ticket = "dummy ticket"
     result = cli_runner.invoke(
         add,
         [
             "sample",
             "--sex",
             Sex.MALE,
             "--application-tag",
             application_tag,
+            "--original-ticket",
+            original_ticket,
             "--lims",
             lims_id,
             customer.internal_id,
             name,
         ],
         obj=base_context,
     )
@@ -145,24 +155,26 @@
     """Test adding a sample using an external sample id."""
     # GIVEN a database with a customer and an application
     helpers.ensure_application(store=disk_store, tag=application_tag)
     helpers.ensure_application_version(store=disk_store, application_tag=application_tag)
     customer: Customer = helpers.ensure_customer(store=disk_store)
     name = "sample_name"
     order = "sample_order"
-
+    original_ticket = "dummy ticket"
     # WHEN adding a sample
     result = cli_runner.invoke(
         add,
         [
             "sample",
             "--sex",
             Sex.MALE,
             "--application-tag",
             application_tag,
+            "--original-ticket",
+            original_ticket,
             "--order",
             order,
             customer.internal_id,
             name,
         ],
         obj=base_context,
     )
@@ -184,24 +196,26 @@
     """Test adding a sample when down sampled"""
     # GIVEN a database with a customer and an application
     helpers.ensure_application(store=disk_store, tag=application_tag)
     helpers.ensure_application_version(store=disk_store, application_tag=application_tag)
     customer: Customer = helpers.ensure_customer(store=disk_store)
     name = "sample_name"
     down_sampled_to = "123"
-
+    original_ticket = "dummy ticket"
     # WHEN adding a sample
     result = cli_runner.invoke(
         add,
         [
             "sample",
             "--sex",
             Sex.MALE,
             "--application-tag",
             application_tag,
+            "--original-ticket",
+            original_ticket,
             "--down-sampled",
             down_sampled_to,
             customer.internal_id,
             name,
         ],
         obj=base_context,
     )
@@ -222,24 +236,26 @@
 ):
     """Test adding a sample with priority."""
     # GIVEN a database with a customer and an application
     helpers.ensure_application(store=disk_store, tag=application_tag)
     helpers.ensure_application_version(store=disk_store, application_tag=application_tag)
     customer: Customer = helpers.ensure_customer(store=disk_store)
     name = "sample_name"
-
+    original_ticket = "dummy ticket"
     # WHEN adding a sample
     result = cli_runner.invoke(
         add,
         [
             "sample",
             "--sex",
             Sex.MALE,
             "--application-tag",
             application_tag,
+            "--original-ticket",
+            original_ticket,
             "--priority",
             Priority.priority.name,
             customer.internal_id,
             name,
         ],
         obj=base_context,
     )
```

### Comparing `cg-59.9.1/tests/cli/backup/conftest.py` & `cg-60.0.0/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/backup/test_backup_command.py` & `cg-60.0.0/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/clean/conftest.py` & `cg-60.0.0/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/clean/test_balsamic_clean.py` & `cg-60.0.0/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/clean/test_clean_flow_cell.py` & `cg-60.0.0/tests/cli/clean/test_clean_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-60.0.0/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/clean/test_hk_bundle_files.py` & `cg-60.0.0/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-60.0.0/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/clean/test_microbial_clean.py` & `cg-60.0.0/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-60.0.0/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/compress/conftest.py` & `cg-60.0.0/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/compress/test_cli_compress_fastq.py` & `cg-60.0.0/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/compress/test_cli_decompress_spring.py` & `cg-60.0.0/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/compress/test_compress_helpers.py` & `cg-60.0.0/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/compress/test_store_fastq.py` & `cg-60.0.0/tests/cli/compress/test_store_fastq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests for the compress fastq cli"""
 
 import logging
 
 from click.testing import CliRunner
 
-from cg.cli.store.fastq import store_case
+from cg.cli.store.store import store_case
 from cg.models.cg_config import CGConfig
 
 
 def test_store_fastq_cli_no_family(compress_context: CGConfig, cli_runner: CliRunner, caplog):
     """Test to run the compress command without providing any case id"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context
```

### Comparing `cg-59.9.1/tests/cli/conftest.py` & `cg-60.0.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/delete/test_cli_delete_case.py` & `cg-60.0.0/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/delete/test_cli_delete_cases.py` & `cg-60.0.0/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/deliver/conftest.py` & `cg-60.0.0/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/deliver/test_deliver_base.py` & `cg-60.0.0/tests/cli/deliver/test_deliver_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 
 from click.testing import CliRunner
 
 from cg.cli.deliver.base import deliver as deliver_cmd
 from cg.constants import EXIT_SUCCESS
-from cg.meta.deliver_ticket import DeliverTicketAPI
+from cg.meta.deliver import DeliverTicketAPI
 from cg.models.cg_config import CGConfig
 
 
 def test_run_base_help(cli_runner: CliRunner):
     """Test to run the deliver base command with --help"""
     # GIVEN a cli runner
 
@@ -108,18 +108,14 @@
 
     # GIVEN a cli runner
 
     # GIVEN uploading data to the delivery server is needed
     mocker.patch.object(DeliverTicketAPI, "check_if_upload_is_needed")
     DeliverTicketAPI.check_if_upload_is_needed.return_value = True
 
-    # GIVEN data needs to be concatenated
-    mocker.patch.object(DeliverTicketAPI, "check_if_concatenation_is_needed")
-    DeliverTicketAPI.check_if_concatenation_is_needed.return_value = True
-
     # WHEN running cg deliver ticket
     cli_runner.invoke(
         deliver_cmd,
         ["ticket", "--dry-run", "--ticket", ticket_id, "--delivery-type", "fastq"],
         obj=cg_context,
     )
```

### Comparing `cg-59.9.1/tests/cli/deliver/test_rsync_base.py` & `cg-60.0.0/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-60.0.0/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-60.0.0/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,62 @@
 from pathlib import Path
 
 import pytest
 from _pytest.fixtures import FixtureRequest
-from click import testing
-from pydantic import BaseModel, ValidationError
+from click.testing import CliRunner, Result
+from pydantic import BaseModel
 
 from cg.apps.demultiplex.sample_sheet.api import SampleSheetAPI
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBCLConvert
 from cg.cli.demultiplex.sample_sheet import create_sheet
 from cg.constants.demultiplexing import BclConverter
 from cg.constants.process import EXIT_SUCCESS
-from cg.exc import SampleSheetError
 from cg.io.txt import read_txt
 from cg.models.cg_config import CGConfig
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 
-FLOW_CELL_FUNCTION_NAME: str = "cg.apps.demultiplex.sample_sheet.api.get_flow_cell_samples"
+GET_FLOW_CELL_SAMPLES: str = "cg.apps.demultiplex.sample_sheet.api.get_flow_cell_samples"
 
 
 def test_create_sample_sheet_no_run_parameters_fails(
-    cli_runner: testing.CliRunner,
+    cli_runner: CliRunner,
     tmp_flow_cell_without_run_parameters_path: Path,
     sample_sheet_context_broken_flow_cells: CGConfig,
     hiseq_2500_custom_index_bcl_convert_lims_samples: list[FlowCellSampleBCLConvert],
     caplog,
     mocker,
 ):
     """Test that creating a flow cell sample sheet fails if there is no run parameters file."""
-    # GIVEN a folder with a non-existing sample sheet nor RunParameters file
-    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
-        flow_cell_path=tmp_flow_cell_without_run_parameters_path
-    )
+    # GIVEN a flow cell directory with a non-existing sample sheet nor RunParameters file
+    flow_cell = FlowCellDirectoryData(tmp_flow_cell_without_run_parameters_path)
 
     # GIVEN that the context's flow cell directory holds the given flow cell
     assert (
         sample_sheet_context_broken_flow_cells.illumina_demultiplexed_runs_directory
         == flow_cell.path.parent.as_posix()
     )
 
     # GIVEN flow cell samples
     mocker.patch(
-        FLOW_CELL_FUNCTION_NAME,
+        GET_FLOW_CELL_SAMPLES,
         return_value=hiseq_2500_custom_index_bcl_convert_lims_samples,
     )
 
     # WHEN running the create sample sheet command
-    result: testing.Result = cli_runner.invoke(
+    result: Result = cli_runner.invoke(
         create_sheet, [flow_cell.full_name], obj=sample_sheet_context_broken_flow_cells
     )
 
     # THEN the process exits with a non-zero exit code
     assert result.exit_code != EXIT_SUCCESS
 
     # THEN the correct information is communicated
     assert "No run parameters file found in flow cell" in caplog.text
 
 
-def test_create_bcl2fastq_sample_sheet(
-    cli_runner: testing.CliRunner,
-    tmp_novaseq_6000_pre_1_5_kits_flow_cell_without_sample_sheet_path: Path,
-    sample_sheet_context: CGConfig,
-    novaseq_6000_pre_1_5_kits_bcl2fastq_lims_samples: list[FlowCellSampleBcl2Fastq],
-    mocker,
-):
-    """Test that creating a Bcl2fastq sample sheet works."""
-    # GIVEN a flowcell directory with some run parameters
-    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
-        flow_cell_path=tmp_novaseq_6000_pre_1_5_kits_flow_cell_without_sample_sheet_path,
-        bcl_converter=BclConverter.BCL2FASTQ,
-    )
-    assert flow_cell.run_parameters_path.exists()
-
-    # GIVEN that there is no sample sheet in the flow cell dir
-    assert not flow_cell.sample_sheet_exists()
-
-    # GIVEN that there are no sample sheet in Housekeeper
-    assert not sample_sheet_context.housekeeper_api.get_sample_sheets_from_latest_version(
-        flow_cell.id
-    )
-
-    # GIVEN flow cell samples
-    mocker.patch(
-        FLOW_CELL_FUNCTION_NAME,
-        return_value=novaseq_6000_pre_1_5_kits_bcl2fastq_lims_samples,
-    )
-    # GIVEN a sample sheet API and a lims API that returns some samples
-    sample_sheet_api: SampleSheetAPI = sample_sheet_context.sample_sheet_api
-
-    # WHEN creating a sample sheet
-    result = cli_runner.invoke(
-        create_sheet,
-        [
-            str(tmp_novaseq_6000_pre_1_5_kits_flow_cell_without_sample_sheet_path),
-            "--bcl-converter",
-            BclConverter.BCL2FASTQ,
-        ],
-        obj=sample_sheet_context,
-    )
-
-    # THEN the process finishes successfully
-    assert result.exit_code == EXIT_SUCCESS
-
-    # THEN the sample sheet was created
-    assert flow_cell.sample_sheet_exists()
-
-    # THEN the sample sheet passes validation
-    sample_sheet_api.validate_sample_sheet(
-        sample_sheet_path=flow_cell.sample_sheet_path, bcl_converter=BclConverter.BCL2FASTQ
-    )
-
-    # THEN the sample sheet is in Housekeeper
-    assert sample_sheet_context.housekeeper_api.get_sample_sheets_from_latest_version(flow_cell.id)
-
-
 class SampleSheetScenario(BaseModel):
     flow_cell_directory: str
     lims_samples: str
     correct_sample_sheet: str
 
 
 @pytest.mark.parametrize(
@@ -140,15 +77,15 @@
             lims_samples="novaseq_x_lims_samples",
             correct_sample_sheet="novaseq_x_correct_sample_sheet",
         ),
     ],
     ids=["Old NovaSeq 6000 flow cell", "New NovaSeq 6000 flow cell", "NovaSeq X flow cell"],
 )
 def test_create_v2_sample_sheet(
-    cli_runner: testing.CliRunner,
+    cli_runner: CliRunner,
     scenario: SampleSheetScenario,
     sample_sheet_context: CGConfig,
     mocker,
     request: FixtureRequest,
 ):
     """Test that creating a v2 sample sheet works."""
     # GIVEN a sample sheet context with a sample sheet api
@@ -167,83 +104,35 @@
     # GIVEN that there are no sample sheet in Housekeeper
     assert not sample_sheet_context.housekeeper_api.get_sample_sheets_from_latest_version(
         flow_cell.id
     )
 
     # GIVEN flow cell samples
     mocker.patch(
-        FLOW_CELL_FUNCTION_NAME,
+        GET_FLOW_CELL_SAMPLES,
         return_value=request.getfixturevalue(scenario.lims_samples),
     )
     # GIVEN a LIMS API that returns samples
 
     # WHEN creating a sample sheet
-    result = cli_runner.invoke(
+    result: Result = cli_runner.invoke(
         create_sheet,
-        [str(flow_cell_directory), "-b", BclConverter.BCLCONVERT],
+        [str(flow_cell_directory)],
         obj=sample_sheet_context,
     )
 
     # THEN the process finishes successfully
     assert result.exit_code == EXIT_SUCCESS
 
     # THEN the sample sheet was created
     assert flow_cell.sample_sheet_exists()
 
     # THEN the sample sheet passes validation
-    sample_sheet_api.validate_sample_sheet(
-        sample_sheet_path=flow_cell.sample_sheet_path, bcl_converter=BclConverter.BCLCONVERT
-    )
+    sample_sheet_api.validate_sample_sheet(flow_cell.sample_sheet_path)
 
     # THEN the sample sheet is in Housekeeper
     assert sample_sheet_context.housekeeper_api.get_sample_sheets_from_latest_version(flow_cell.id)
 
     # THEN the sample sheet should have the exact structure
     generated_content: str = read_txt(flow_cell.sample_sheet_path)
     correct_content: str = read_txt(Path(request.getfixturevalue(scenario.correct_sample_sheet)))
     assert generated_content == correct_content
-
-
-def test_incorrect_bcl2fastq_samplesheet_is_regenerated(
-    cli_runner: testing.CliRunner,
-    tmp_flow_cells_directory_malformed_sample_sheet: Path,
-    sample_sheet_context: CGConfig,
-    novaseq_6000_pre_1_5_kits_bcl2fastq_lims_samples: list[FlowCellSampleBcl2Fastq],
-    mocker,
-    caplog,
-):
-    """Test that when a flow cell has a malformed sample sheet it is regenerated correctly."""
-    # GIVEN a flowcell directory with some run parameters
-    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
-        flow_cell_path=tmp_flow_cells_directory_malformed_sample_sheet,
-        bcl_converter=BclConverter.BCL2FASTQ,
-    )
-
-    # GIVEN a sample sheet API and an invalid sample sheet
-    sample_sheet_api: SampleSheetAPI = sample_sheet_context.sample_sheet_api
-    with pytest.raises(SampleSheetError):
-        sample_sheet_api.validate_sample_sheet(
-            sample_sheet_path=flow_cell.sample_sheet_path, bcl_converter=BclConverter.BCL2FASTQ
-        )
-
-    # GIVEN flow cell samples
-    mocker.patch(
-        FLOW_CELL_FUNCTION_NAME,
-        return_value=novaseq_6000_pre_1_5_kits_bcl2fastq_lims_samples,
-    )
-    # GIVEN a lims api that returns some samples
-
-    # WHEN creating a sample sheet
-    cli_runner.invoke(
-        create_sheet,
-        [
-            str(tmp_flow_cells_directory_malformed_sample_sheet),
-            "--bcl-converter",
-            BclConverter.BCL2FASTQ,
-        ],
-        obj=sample_sheet_context,
-    )
-
-    # THEN the sample sheet was re-created and passes validation
-    sample_sheet_api.validate_sample_sheet(
-        sample_sheet_path=flow_cell.sample_sheet_path, bcl_converter=BclConverter.BCL2FASTQ
-    )
```

### Comparing `cg-59.9.1/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-60.0.0/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,112 +11,14 @@
 from cg.meta.demultiplex.housekeeper_storage_functions import (
     add_and_include_sample_sheet_path_to_housekeeper,
 )
 from cg.models.cg_config import CGConfig
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 
 
-def test_demultiplex_bcl2fastq_flow_cell_dry_run(
-    cli_runner: testing.CliRunner,
-    tmp_flow_cells_directory_ready_for_demultiplexing_bcl2fastq: Path,
-    demultiplexing_context_for_demux: CGConfig,
-    caplog,
-):
-    caplog.set_level(logging.INFO)
-
-    # GIVEN that all files are present for demultiplexing
-    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
-        tmp_flow_cells_directory_ready_for_demultiplexing_bcl2fastq,
-        bcl_converter=BclConverter.BCL2FASTQ,
-    )
-    add_and_include_sample_sheet_path_to_housekeeper(
-        flow_cell_directory=tmp_flow_cells_directory_ready_for_demultiplexing_bcl2fastq,
-        flow_cell_name=flow_cell.id,
-        hk_api=demultiplexing_context_for_demux.housekeeper_api,
-    )
-
-    # GIVEN an out dir that does not exist
-    demux_api: DemultiplexingAPI = demultiplexing_context_for_demux.demultiplex_api
-    assert demux_api.is_demultiplexing_possible(flow_cell=flow_cell)
-    demux_dir: Path = demux_api.flow_cell_out_dir_path(flow_cell)
-    unaligned_dir: Path = Path(demux_dir, DemultiplexingDirsAndFiles.UNALIGNED_DIR_NAME)
-    assert demux_dir.exists() is False
-    assert unaligned_dir.exists() is False
-
-    # WHEN starting demultiplexing from the CLI with dry run flag
-    result: testing.Result = cli_runner.invoke(
-        demultiplex_flow_cell,
-        [
-            str(tmp_flow_cells_directory_ready_for_demultiplexing_bcl2fastq),
-            "--dry-run",
-            "-b",
-            BclConverter.BCL2FASTQ,
-        ],
-        obj=demultiplexing_context_for_demux,
-    )
-
-    # THEN assert the command exits without problems
-    assert result.exit_code == 0
-
-    # THEN assert no results folder was created since it is run in dry run mode
-    assert demux_dir.exists() is False
-    assert unaligned_dir.exists() is False
-
-
-def test_demultiplex_bcl2fastq_flow_cell(
-    cli_runner: testing.CliRunner,
-    tmp_flow_cells_directory_ready_for_demultiplexing_bcl2fastq: Path,
-    demultiplexing_context_for_demux: CGConfig,
-    caplog,
-    mocker,
-):
-    caplog.set_level(logging.INFO)
-
-    # GIVEN that all files are present for bcl2fastq demultiplexing
-    flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
-        tmp_flow_cells_directory_ready_for_demultiplexing_bcl2fastq,
-        bcl_converter=BclConverter.BCL2FASTQ,
-    )
-    add_and_include_sample_sheet_path_to_housekeeper(
-        flow_cell_directory=tmp_flow_cells_directory_ready_for_demultiplexing_bcl2fastq,
-        flow_cell_name=flow_cell.id,
-        hk_api=demultiplexing_context_for_demux.housekeeper_api,
-    )
-
-    # GIVEN a flow cell that is ready for demultiplexing
-    demux_api: DemultiplexingAPI = demultiplexing_context_for_demux.demultiplex_api
-    demux_dir: Path = demux_api.flow_cell_out_dir_path(flow_cell)
-    unaligned_dir: Path = Path(demux_dir, DemultiplexingDirsAndFiles.UNALIGNED_DIR_NAME)
-    assert demux_api.is_demultiplexing_possible(flow_cell=flow_cell)
-
-    mocker.patch("cg.apps.tb.TrailblazerAPI.add_pending_analysis")
-
-    # WHEN starting demultiplexing from the CLI with dry run flag
-    result: testing.Result = cli_runner.invoke(
-        demultiplex_flow_cell,
-        [
-            str(tmp_flow_cells_directory_ready_for_demultiplexing_bcl2fastq),
-            "-b",
-            BclConverter.BCL2FASTQ,
-        ],
-        obj=demultiplexing_context_for_demux,
-    )
-
-    # THEN assert the command exits successfully
-
-    assert result.exit_code == 0
-
-    # THEN assert the results folder was created
-    assert demux_dir.exists()
-    assert unaligned_dir.exists()
-
-    # THEN assert that the sbatch script was created
-    assert demux_api.demultiplex_sbatch_path(flow_cell).exists()
-
-
 def test_demultiplex_dragen_flowcell(
     cli_runner: testing.CliRunner,
     tmp_flow_cell_directory_bclconvert: Path,
     demultiplexing_context_for_demux: CGConfig,
     caplog,
     mocker,
 ):
@@ -144,15 +46,15 @@
     marker_file = Path(demux_dir, "dummy_file_present_in_old_dir")
     marker_file.touch()
     assert marker_file.exists()
 
     # WHEN starting demultiplexing from the CLI
     result: testing.Result = cli_runner.invoke(
         demultiplex_flow_cell,
-        [str(tmp_flow_cell_directory_bclconvert), "-b", BclConverter.BCLCONVERT],
+        [str(tmp_flow_cell_directory_bclconvert)],
         obj=demultiplexing_context_for_demux,
     )
 
     # THEN assert the command exits without problems
     assert result.exit_code == 0
 
     # THEN assert the results folder was created
```

### Comparing `cg-59.9.1/tests/cli/demultiplex/test_finish_demux.py` & `cg-60.0.0/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-60.0.0/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from pathlib import Path
 
+import pytest
 from click.testing import CliRunner, Result
 
-from cg.apps.demultiplex.sample_sheet.sample_sheet_validator import SampleSheetValidator
 from cg.cli.demultiplex.sample_sheet import validate_sample_sheet
 from cg.constants import EXIT_SUCCESS, FileExtensions
-from cg.constants.demultiplexing import BclConverter
 from cg.models.cg_config import CGConfig
 
 
 def test_validate_non_existing_sample_sheet(
     cli_runner: CliRunner,
     sample_sheet_context: CGConfig,
 ):
@@ -55,57 +54,38 @@
     # THEN assert it exits with a non-zero exit code
     assert result.exit_code != EXIT_SUCCESS
 
     # THEN assert the correct information was communicated
     assert "seems to be in wrong format" in caplog.text
 
 
-def test_validate_correct_bcl2fastq_sample_sheet(
+@pytest.mark.parametrize(
+    "sample_sheet_path",
+    [
+        "hiseq_x_single_index_sample_sheet_path",
+        "hiseq_x_dual_index_sample_sheet_path",
+        "hiseq_2500_dual_index_sample_sheet_path",
+        "hiseq_2500_custom_index_sample_sheet_path",
+        "novaseq_6000_pre_1_5_kits_correct_sample_sheet_path",
+        "novaseq_6000_post_1_5_kits_correct_sample_sheet_path",
+        "novaseq_x_correct_sample_sheet",
+    ],
+)
+def test_validate_correct_bcl_convert_sample_sheet(
     cli_runner: CliRunner,
-    novaseq_bcl2fastq_sample_sheet_path: Path,
-    sample_sheet_context: CGConfig,
-):
-    """Test validate sample sheet when using a bcl2fastq sample sheet."""
-
-    # GIVEN the path to a bcl2fastq sample sheet that exists
-    sample_sheet: Path = novaseq_bcl2fastq_sample_sheet_path
-    assert sample_sheet.exists()
-
-    # GIVEN that the sample sheet is correct
-    SampleSheetValidator().validate_sample_sheet_from_file(
-        file_path=sample_sheet, bcl_converter=BclConverter.BCL2FASTQ
-    )
-
-    # WHEN validating the sample sheet
-    result: Result = cli_runner.invoke(
-        validate_sample_sheet,
-        [str(sample_sheet)],
-        obj=sample_sheet_context,
-    )
-
-    # THEN assert that it exits successfully
-    assert result.exit_code == EXIT_SUCCESS
-
-
-def test_validate_correct_dragen_sample_sheet(
-    cli_runner: CliRunner,
-    novaseq_6000_post_1_5_kits_correct_sample_sheet_path: Path,
+    sample_sheet_path: str,
     sample_sheet_context: CGConfig,
+    request: pytest.FixtureRequest,
 ):
     """Test validate sample sheet when using a BCLconvert sample sheet."""
 
-    # GIVEN the path to a Bcl2fastq sample sheet that exists
-    sample_sheet: Path = novaseq_6000_post_1_5_kits_correct_sample_sheet_path
+    # GIVEN the path to a correct BCLConvert sample sheet that exists
+    sample_sheet: Path = request.getfixturevalue(sample_sheet_path)
     assert sample_sheet.exists()
 
-    # GIVEN that the sample sheet is correct
-    SampleSheetValidator().validate_sample_sheet_from_file(
-        file_path=sample_sheet, bcl_converter=BclConverter.BCLCONVERT
-    )
-
     # WHEN validating the sample sheet
     result: Result = cli_runner.invoke(
         validate_sample_sheet, [str(sample_sheet)], obj=sample_sheet_context
     )
 
     # THEN assert that it exits successfully
     assert result.exit_code == EXIT_SUCCESS
```

### Comparing `cg-59.9.1/tests/cli/demultiplex/test_verify_syncing.py` & `cg-60.0.0/tests/cli/demultiplex/test_verify_syncing.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/downsample/test_cli_downsample.py` & `cg-60.0.0/tests/cli/downsample/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/generate/report/conftest.py` & `cg-60.0.0/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-60.0.0/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/generate/report/test_utils.py` & `cg-60.0.0/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/generate/test_cli_base.py` & `cg-60.0.0/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/get/test_cli_get.py` & `cg-60.0.0/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/get/test_cli_get_analysis.py` & `cg-60.0.0/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/get/test_cli_get_case.py` & `cg-60.0.0/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/get/test_cli_get_flow_cell.py` & `cg-60.0.0/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/get/test_cli_get_sample.py` & `cg-60.0.0/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/set/conftest.py` & `cg-60.0.0/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/set/test_cli_set_cases.py` & `cg-60.0.0/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/set/test_cli_set_flowcell.py` & `cg-60.0.0/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/set/test_cli_set_list_keys.py` & `cg-60.0.0/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/set/test_cli_set_sample.py` & `cg-60.0.0/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/set/test_cli_set_samples.py` & `cg-60.0.0/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/store/test_fastq.py` & `cg-60.0.0/tests/cli/store/test_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from click.testing import CliRunner
 
-from cg.cli.store.fastq import (
+from cg.cli.store.store import (
     store_case,
     store_demultiplexed_flow_cell,
     store_flow_cell,
     store_sample,
     store_ticket,
 )
 from cg.constants import EXIT_SUCCESS
@@ -192,15 +192,15 @@
     sample: Sample = real_populated_compress_context.status_db.get_sample_by_internal_id(sample_id)
 
     # GIVEN samples objects on a flow cell
     mocker.patch.object(Store, "get_samples_from_flow_cell")
     Store.get_samples_from_flow_cell.return_value = [sample]
 
     # GIVEN an updated metadata file
-    mocker.patch("cg.cli.store.fastq.update_metadata_paths", return_value=None)
+    mocker.patch("cg.cli.store.store.update_metadata_paths", return_value=None)
 
     # WHEN running the store demultiplexed flow cell command
     res = cli_runner.invoke(
         store_demultiplexed_flow_cell, [bcl2fastq_flow_cell_id], obj=real_populated_compress_context
     )
 
     # THEN assert that the command exits successfully
```

### Comparing `cg-59.9.1/tests/cli/test_base.py` & `cg-60.0.0/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/conftest.py` & `cg-60.0.0/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_scout.py` & `cg-60.0.0/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload_auto.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload_fastq.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload_genotype.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload_gens.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload_nipt.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/upload/test_cli_upload_observations.py` & `cg-60.0.0/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/balsamic/conftest.py` & `cg-60.0.0/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-60.0.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-60.0.0/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/balsamic/test_link.py` & `cg-60.0.0/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-60.0.0/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/balsamic/test_run.py` & `cg-60.0.0/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-60.0.0/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/conftest.py` & `cg-60.0.0/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-60.0.0/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/fluffy/conftest.py` & `cg-60.0.0/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-60.0.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-60.0.0/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-60.0.0/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-60.0.0/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-60.0.0/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/microsalt/conftest.py` & `cg-60.0.0/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-60.0.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-60.0.0/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/conftest.py` & `cg-60.0.0/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-60.0.0/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py` & `cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,141 @@
 """Tests CLI common methods to create the report_deliver for NF analyses."""
 
 import logging
-import pytest
 from pathlib import Path
 
-from click.testing import CliRunner
+import pytest
+from _pytest.fixtures import FixtureRequest
 from _pytest.logging import LogCaptureFixture
+from click.testing import CliRunner
 
+from cg.cli.workflow.base import workflow as workflow_cli
+from cg.constants import EXIT_SUCCESS, Workflow
+from cg.constants.constants import FileFormat
+from cg.io.controller import ReadFile
 from cg.meta.workflow.nf_analysis import NfAnalysisAPI
-from cg.cli.workflow.rnafusion.base import report_deliver
 from cg.models.cg_config import CGConfig
-from cg.constants import EXIT_SUCCESS
-from cg.io.controller import ReadFile
-from cg.constants.constants import FileFormat
 
 LOG = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize(
-    "context",
-    ["rnafusion_context", "taxprofiler_context"],
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
 )
-def test_report_deliver_without_options(cli_runner: CliRunner, context: CGConfig, request):
+def test_report_deliver_without_options(
+    cli_runner: CliRunner, workflow: Workflow, request: FixtureRequest
+):
     """Test report-deliver for workflow without options."""
     # GIVEN a NextFlow analysis context
-    context = request.getfixturevalue(context)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
-    # WHEN dry running without anything specified
-    result = cli_runner.invoke(report_deliver, obj=context)
+    # WHEN invoking the command without additional parameters
+    result = cli_runner.invoke(workflow_cli, [workflow, "report-deliver"], obj=context)
 
     # THEN command should not exit successfully
     assert result.exit_code != EXIT_SUCCESS
 
     # THEN command log should inform about missing arguments
     assert "Missing argument" in result.output
 
 
 @pytest.mark.parametrize(
-    "context",
-    ["rnafusion_context", "taxprofiler_context"],
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
 )
 def test_report_deliver_with_missing_case(
     cli_runner: CliRunner,
-    context: CGConfig,
+    workflow: Workflow,
     caplog: LogCaptureFixture,
     case_id_does_not_exist: str,
-    request,
+    request: FixtureRequest,
 ):
     """Test report-deliver command for workflow with invalid case to start with."""
     caplog.set_level(logging.WARNING)
-    context = request.getfixturevalue(context)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
-    # GIVEN case_id not in database
+    # GIVEN a case id not present in StatusDB
     assert not context.status_db.get_case_by_internal_id(internal_id=case_id_does_not_exist)
 
     # WHEN generating deliverables file
-    result = cli_runner.invoke(report_deliver, [case_id_does_not_exist], obj=context)
+    result = cli_runner.invoke(
+        workflow_cli, [workflow, "report-deliver", case_id_does_not_exist], obj=context
+    )
 
     # THEN command should NOT succeed
     assert result.exit_code != EXIT_SUCCESS
 
     # THEN ERROR log should be printed containing the invalid case id
     assert case_id_does_not_exist in caplog.text
     assert "could not be found" in caplog.text
 
 
 @pytest.mark.parametrize(
-    "context",
-    ["rnafusion_context", "taxprofiler_context"],
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
 )
 def test_report_deliver_without_samples(
     cli_runner: CliRunner,
-    context: CGConfig,
+    workflow: Workflow,
     caplog: LogCaptureFixture,
     no_sample_case_id: str,
-    request,
+    request: FixtureRequest,
 ):
     """Test report-deliver command for workflow with case id and no samples."""
     caplog.set_level(logging.ERROR)
-    context = request.getfixturevalue(context)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
-    # GIVEN case-id
+    # GIVEN a case id
     case_id: str = no_sample_case_id
 
-    # WHEN generating deliverables with dry specified
-    result = cli_runner.invoke(report_deliver, [case_id, "--dry-run"], obj=context)
+    # WHEN generating deliverables with dry-run specified
+    result = cli_runner.invoke(
+        workflow_cli, [workflow, "report-deliver", case_id, "--dry-run"], obj=context
+    )
 
     # THEN command should NOT execute successfully
     assert result.exit_code != EXIT_SUCCESS
 
     # THEN warning should be printed that no samples exist in case
     assert "no samples" in caplog.text
 
 
 @pytest.mark.parametrize(
-    ("context", "case_id", "deliverables_file_path", "mock_analysis_finish"),
-    [
-        (
-            "taxprofiler_context",
-            "taxprofiler_case_id",
-            "taxprofiler_deliverables_file_path",
-            "taxprofiler_mock_analysis_finish",
-        ),
-        (
-            "rnafusion_context",
-            "rnafusion_case_id",
-            "rnafusion_deliverables_file_path",
-            "rnafusion_mock_analysis_finish",
-        ),
-    ],
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
 )
 def test_report_deliver_successful(
     cli_runner: CliRunner,
-    context: CGConfig,
-    case_id: str,
-    deliverables_file_path: Path,
-    deliverables_template_content: list[dict],
-    mock_analysis_finish,
+    workflow: Workflow,
     caplog: LogCaptureFixture,
+    deliverables_template_content: list[dict],
     mocker,
-    request,
+    request: FixtureRequest,
 ):
     """Test that deliverable files is properly created on a valid and successful run for workflow."""
     caplog.set_level(logging.INFO)
 
-    # GIVEN each fixture is being initialised
-    context: CGConfig = request.getfixturevalue(context)
-    deliverables_file_path: dict = request.getfixturevalue(deliverables_file_path)
-    case_id: str = request.getfixturevalue(case_id)
-    request.getfixturevalue(mock_analysis_finish)
+    # GIVEN deliverable files for a case and workflow
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
+    case_id: str = request.getfixturevalue(f"{workflow}_case_id")
+    deliverables_file_path: Path = request.getfixturevalue(f"{workflow}_deliverables_file_path")
+    request.getfixturevalue(f"{workflow}_mock_analysis_finish")
 
     # GIVEN a successful run
 
     # GIVEN a mocked deliverables template
     mocker.patch.object(
         NfAnalysisAPI,
         "get_deliverables_template_content",
         return_value=deliverables_template_content,
     )
 
     # WHEN running the command
-    result = cli_runner.invoke(report_deliver, [case_id], obj=context)
+    result = cli_runner.invoke(workflow_cli, [workflow, "report-deliver", case_id], obj=context)
 
     # THEN command should execute successfully
     assert result.exit_code == EXIT_SUCCESS
 
     # THEN deliverables file should be written
     assert deliverables_file_path.is_file()
```

### Comparing `cg-59.9.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py` & `cg-60.0.0/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,22 @@
 from pathlib import Path
 
 from click.testing import CliRunner
 from mock import mock
 
-from cg.cli.workflow.raredisease.base import managed_variants, panel, raredisease
-from cg.constants import EXIT_SUCCESS
+from cg.cli.workflow.raredisease.base import managed_variants, panel
 from cg.constants.scout import ScoutExportFileName
 from cg.io.txt import read_txt
 from cg.meta.workflow.raredisease import RarediseaseAnalysisAPI
 from cg.models.cg_config import CGConfig
 from tests.conftest import create_process_response
 
 SUBPROCESS_RUN_FUNCTION_NAME: str = "cg.utils.commands.subprocess.run"
 
 
-def test_raredisease_no_args(cli_runner: CliRunner, raredisease_context: CGConfig):
-    """Test to see that running RAREDISEASE without options prints help and doesn't result in an error."""
-    # GIVEN no arguments or options besides the command call
-
-    # WHEN running command
-    result = cli_runner.invoke(raredisease, [], obj=raredisease_context)
-
-    # THEN command runs successfully
-    assert result.exit_code == EXIT_SUCCESS
-
-    # THEN help should be printed
-    assert "help" in result.output
-
-
 def test_panel_dry_run(
     raredisease_case_id: str,
     cli_runner: CliRunner,
     raredisease_context: CGConfig,
     scout_panel_output: str,
 ):
     # GIVEN a case
```

### Comparing `cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_config_case.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,254 +1,198 @@
-"""This script tests the run cli command"""
+"""Tests CLI common methods to create the case config for NF analyses."""
 
 import logging
+from pathlib import Path
 
 import pytest
+from _pytest.fixtures import FixtureRequest
 from _pytest.logging import LogCaptureFixture
 from click.testing import CliRunner
 
-from cg.cli.workflow.rnafusion.base import run
-from cg.constants import EXIT_SUCCESS
+from cg.cli.workflow.base import workflow as workflow_cli
+from cg.constants import EXIT_SUCCESS, Workflow
+from cg.constants.constants import FileFormat
+from cg.io.controller import ReadFile
 from cg.models.cg_config import CGConfig
+from cg.models.nf_analysis import WorkflowParameters
 
-
-def test_without_options(cli_runner: CliRunner, rnafusion_context: CGConfig):
-    """Test command without case_id argument."""
-    # GIVEN no case_id
-    # WHEN dry running without anything specified
-    result = cli_runner.invoke(run, obj=rnafusion_context)
-    # THEN command should NOT execute successfully
-    assert result.exit_code != EXIT_SUCCESS
-    # THEN command should mention argument
-    assert "Missing argument" in result.output
+LOG = logging.getLogger(__name__)
 
 
-def test_with_missing_case(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    caplog: LogCaptureFixture,
-    case_id_does_not_exist: str,
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RAREDISEASE, Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
+)
+def test_config_case_without_options(
+    cli_runner: CliRunner, workflow: Workflow, request: FixtureRequest
 ):
-    """Test command with invalid case to start with."""
-    caplog.set_level(logging.ERROR)
-    # GIVEN case_id not in database
-    assert not rnafusion_context.status_db.get_case_by_internal_id(
-        internal_id=case_id_does_not_exist
-    )
-    # WHEN running
-    result = cli_runner.invoke(run, [case_id_does_not_exist], obj=rnafusion_context)
-    # THEN command should NOT successfully call the command it creates
-    assert result.exit_code != EXIT_SUCCESS
-    # THEN ERROR log should be printed containing invalid case_id
-    assert case_id_does_not_exist in caplog.text
-    assert "could not be found" in caplog.text
+    """Test config_case for workflow without options."""
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
+    # WHEN invoking the command without additional parameters
+    result = cli_runner.invoke(workflow_cli, [workflow, "config-case"], obj=context)
 
-def test_without_samples(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    caplog: LogCaptureFixture,
-    no_sample_case_id: str,
-):
-    """Test command with case_id and no samples."""
-    caplog.set_level(logging.ERROR)
-    # GIVEN case-id
-    case_id: str = no_sample_case_id
-    # WHEN dry running with dry specified
-    result = cli_runner.invoke(run, [case_id, "--dry-run"], obj=rnafusion_context)
-    # THEN command should NOT execute successfully
+    # THEN command should not exit successfully
     assert result.exit_code != EXIT_SUCCESS
-    # THEN warning should be printed that no config file is found
-    assert case_id in caplog.text
-    assert "no samples" in caplog.text
 
-
-def test_without_config_dry_run(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
-):
-    """Test command dry-run with case_id and no config file."""
-    caplog.set_level(logging.ERROR)
-    # GIVEN case-id
-    case_id: str = rnafusion_case_id
-    # WHEN dry running with dry specified
-    result = cli_runner.invoke(run, [case_id, "--from-start", "--dry-run"], obj=rnafusion_context)
-    # THEN command should execute successfully (dry-run)
-    assert result.exit_code == EXIT_SUCCESS
+    # THEN command log should inform about missing arguments
+    assert "Missing argument" in result.output
 
 
-def test_without_config(
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RAREDISEASE, Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
+)
+def test_config_with_missing_case(
     cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
     caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
+    case_id_does_not_exist: str,
+    workflow: Workflow,
+    request: FixtureRequest,
 ):
-    """Test command with case_id and no config file."""
+    """Test config_case for workflow with a missing case."""
     caplog.set_level(logging.ERROR)
-    # GIVEN case-id
-    case_id: str = rnafusion_case_id
-    # WHEN dry running with dry specified
-    result = cli_runner.invoke(run, [case_id], obj=rnafusion_context)
-    # THEN command should NOT execute successfully
-    assert result.exit_code != EXIT_SUCCESS
-    # THEN warning should be printed that no config file is found
-    assert "No config file found" in caplog.text
-
-
-def test_with_config_use_nextflow(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
-    mock_config,
-):
-    """Test command with case_id and config file using nextflow."""
-    caplog.set_level(logging.INFO)
-    # GIVEN case-id
-    case_id: str = rnafusion_case_id
-
-    # GIVEN a mocked config
-
-    # WHEN dry running with dry specified
-    result = cli_runner.invoke(run, [case_id, "--dry-run", "--use-nextflow"], obj=rnafusion_context)
-
-    # THEN command should execute successfully
-    assert result.exit_code == EXIT_SUCCESS
-
-    # THEN command should use nextflow
-    assert "using Nextflow" in caplog.text
-    assert "path/to/bin/nextflow" in caplog.text
-    assert "-work-dir" in caplog.text
-
-    # THEN command should include resume flag
-    assert "-resume" in caplog.text
-
-
-def test_with_config(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
-    mock_config,
-):
-    """Test command with case_id and config file using tower."""
-    caplog.set_level(logging.INFO)
-    # GIVEN case-id
-    case_id: str = rnafusion_case_id
-
-    # GIVEN a mocked config
-
-    # WHEN dry running with dry specified
-    result = cli_runner.invoke(run, [case_id, "--from-start", "--dry-run"], obj=rnafusion_context)
-
-    # THEN command should execute successfully
-    assert result.exit_code == EXIT_SUCCESS
-
-    # THEN command should use tower
-    assert "using Tower" in caplog.text
-    assert "path/to/bin/tw launch" in caplog.text
-    assert "--work-dir" in caplog.text
-
-
-def test_with_revision(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
-    mock_config,
-):
-    """Test command with case_id and config file using tower and specifying a revision."""
-    caplog.set_level(logging.INFO)
-    # GIVEN case-id
-    case_id: str = rnafusion_case_id
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
-    # GIVEN a mocked config
+    # GIVEN a case not in the StatusDB database
+    assert not context.status_db.get_case_by_internal_id(internal_id=case_id_does_not_exist)
 
-    # WHEN dry running with dry specified
+    # WHEN running
     result = cli_runner.invoke(
-        run, [case_id, "--dry-run", "--from-start", "--revision", "2.1.0"], obj=rnafusion_context
+        workflow_cli, [workflow, "config-case", case_id_does_not_exist], obj=context
     )
 
-    # THEN command should execute successfully
-    assert result.exit_code == EXIT_SUCCESS
+    # THEN command should not exit successfully
+    assert result.exit_code != EXIT_SUCCESS
 
-    # THEN command should use tower
-    assert "--revision 2.1.0" in caplog.text
+    # THEN the error log should indicate that the case is invalid
+    assert "could not be found in Status DB!" in caplog.text
 
 
-def test_resume_with_id(
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.RAREDISEASE, Workflow.TOMTE],
+)
+def test_config_case_without_samples(
     cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
+    workflow: Workflow,
+    no_sample_case_id: str,
     caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
-    mock_config,
-    tower_id,
+    request: FixtureRequest,
 ):
-    """Test resume command given a NF-Tower run ID using Tower."""
-    caplog.set_level(logging.INFO)
-
-    # GIVEN a case-id
+    """Test command with a case lacking linked samples."""
+    caplog.set_level(logging.ERROR)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
-    # GIVEN a mocked config
+    # GIVEN a case without linked samples
 
-    # WHEN dry running with dry specified
+    # WHEN invoking the command
     result = cli_runner.invoke(
-        run, [rnafusion_case_id, "--nf-tower-id", tower_id, "--dry-run"], obj=rnafusion_context
+        workflow_cli, [workflow, "config-case", no_sample_case_id], obj=context
     )
 
-    # THEN command should execute successfully
-    assert result.exit_code == EXIT_SUCCESS
-
-    # THEN command should use tower for relaunch
-    assert "Workflow will be resumed from run" in caplog.text
-    assert "tw runs relaunch" in caplog.text
-
-
-def test_resume_without_id(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
-    mock_config,
-    rnafusion_mock_analysis_finish,
-):
-    """Test resume command without providing NF-Tower ID when a Trailblazer Tower config file from a previous run
-    exist."""
-    caplog.set_level(logging.INFO)
-
-    # GIVEN case-id
-
-    # GIVEN a mocked config
-
-    # WHEN dry running with dry specified
-    result = cli_runner.invoke(run, [rnafusion_case_id, "--dry-run"], obj=rnafusion_context)
-
-    # THEN command should execute successfully
-    assert result.exit_code == EXIT_SUCCESS
-
-    # THEN command should use tower for relaunch
-    assert "Workflow will be resumed from run" in caplog.text
-    assert "tw runs relaunch" in caplog.text
-
-
-def test_resume_without_id_error(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
-    mock_config,
-):
-    """Test resume command without providing NF-Tower ID and without existing Trailblazer Tower config file."""
-    caplog.set_level(logging.INFO)
-
-    # GIVEN case-id
-
-    # GIVEN a mocked config
+    # THEN command should not exit successfully
+    assert result.exit_code != EXIT_SUCCESS
 
-    # WHEN dry running with dry specified
-    cli_runner.invoke(run, [rnafusion_case_id, "--dry-run"], obj=rnafusion_context)
+    # THEN warning should be printed that no sample is found
+    assert no_sample_case_id in caplog.text
+    assert "has no samples" in caplog.text
+
+
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.RAREDISEASE, Workflow.TOMTE],
+)
+def test_config_case_default_parameters(
+    cli_runner: CliRunner,
+    workflow: Workflow,
+    caplog: LogCaptureFixture,
+    request: FixtureRequest,
+):
+    """Test that command generates config files."""
+    caplog.set_level(logging.DEBUG)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
+    case_id: str = request.getfixturevalue(f"{workflow}_case_id")
+    sample_sheet_path: Path = request.getfixturevalue(f"{workflow}_sample_sheet_path")
+    params_file_path: Path = request.getfixturevalue(f"{workflow}_params_file_path")
+    nexflow_config_file_path: Path = request.getfixturevalue(f"{workflow}_nexflow_config_file_path")
+    sample_sheet_content_expected: str = request.getfixturevalue(f"{workflow}_sample_sheet_content")
+
+    # GIVEN a valid case
+
+    # WHEN running config case
+    result = cli_runner.invoke(workflow_cli, [workflow, "config-case", case_id], obj=context)
+
+    # THEN command should exit successfully
+    assert result.exit_code == EXIT_SUCCESS
+
+    # THEN logs should be as expected
+    expected_logs: list[str] = [
+        "Getting sample sheet information",
+        "Writing sample sheet",
+        "Getting parameters information",
+        "Writing parameters file",
+        "Writing nextflow config file",
+    ]
+    for expected_log in expected_logs:
+        assert expected_log in caplog.text
+
+    # THEN config files should be generated
+    assert sample_sheet_path.is_file()
+    assert params_file_path.is_file()
+    assert nexflow_config_file_path.is_file()
+
+    # THEN the sample sheet content should match the expected values
+    sample_sheet_content_created: list[list[str]] = ReadFile.get_content_from_file(
+        file_format=FileFormat.TXT, file_path=sample_sheet_path, read_to_string=True
+    )
+    assert sample_sheet_content_expected in sample_sheet_content_created
 
-    # THEN command should raise error
-    assert "Could not resume analysis: No NF-Tower ID found for case" in caplog.text
-    pytest.raises(FileNotFoundError)
+    # WHEN workflow is not raredisease
+    # Note this will need to be unified once all workflows are standarised
+    if workflow not in {Workflow.RAREDISEASE, Workflow.TOMTE}:
+        # THEN the params file should contain all parameters
+        parameters_default = vars(request.getfixturevalue(f"{workflow}_parameters_default"))
+        params_content: list[list[str]] = ReadFile.get_content_from_file(
+            file_format=FileFormat.TXT, file_path=params_file_path, read_to_string=True
+        )
+        for parameter in parameters_default:
+            assert parameter in params_content
+
+
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.RAREDISEASE, Workflow.TOMTE],
+)
+def test_config_case_dry_run(
+    cli_runner: CliRunner,
+    workflow: Workflow,
+    caplog: LogCaptureFixture,
+    request: FixtureRequest,
+):
+    """Test dry-run."""
+    caplog.set_level(logging.DEBUG)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
+    case_id: str = request.getfixturevalue(f"{workflow}_case_id")
+    sample_sheet_path: Path = request.getfixturevalue(f"{workflow}_sample_sheet_path")
+    params_file_path: Path = request.getfixturevalue(f"{workflow}_params_file_path")
+    nexflow_config_file_path: Path = request.getfixturevalue(f"{workflow}_nexflow_config_file_path")
+
+    # GIVEN a valid case
+
+    # WHEN invoking the command with dry-run specified
+    result = cli_runner.invoke(workflow_cli, [workflow, "config-case", case_id, "-d"], obj=context)
+
+    # THEN command should exit successfully
+    assert result.exit_code == EXIT_SUCCESS
+
+    # THEN sample sheet and parameters information should be collected
+    assert "Getting sample sheet information" in caplog.text
+    assert "Getting parameters information" in caplog.text
+
+    # THEN sample sheet and parameters information files should not be written
+    assert "Dry run: Config files will not be written" in caplog.text
+    assert "Writing sample sheet" not in caplog.text
+    assert "Writing parameters file" not in caplog.text
+    assert not sample_sheet_path.is_file()
+    assert not params_file_path.is_file()
+    assert not nexflow_config_file_path.is_file()
```

### Comparing `cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_store.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,240 +1,248 @@
 import logging
-from pathlib import Path
 
 import pytest
+from _pytest.fixtures import FixtureRequest
 from _pytest.logging import LogCaptureFixture
 from click.testing import CliRunner
-from pydantic import ValidationError
-from pytest_mock import MockFixture
 
 from cg.apps.hermes.hermes_api import HermesApi
 from cg.apps.hermes.models import CGDeliverables
 from cg.apps.housekeeper.hk import HousekeeperAPI
-from cg.cli.workflow.rnafusion.base import store_housekeeper
-from cg.constants import EXIT_SUCCESS
-from cg.constants.constants import FileFormat
-from cg.io.controller import WriteStream
-from cg.meta.workflow.rnafusion import RnafusionAnalysisAPI
+from cg.cli.workflow.base import workflow as workflow_cli
+from cg.constants import EXIT_FAIL, EXIT_SUCCESS, Workflow
+from cg.constants.constants import CaseActions
+from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.cg_config import CGConfig
-from cg.utils import Process
 
 
-def test_without_options(cli_runner: CliRunner, rnafusion_context: CGConfig):
-    """Test command without case_id argument."""
-    # GIVEN no case_id
-
-    # WHEN running without anything specified
-    result = cli_runner.invoke(store_housekeeper, obj=rnafusion_context)
-
-    # THEN command should NOT execute successfully
-    assert result.exit_code != EXIT_SUCCESS
-
-    # THEN command should mention argument
-    assert "Missing argument" in result.output
-
-
-def test_with_missing_case(
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
+)
+def test_store_success(
     cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
+    real_housekeeper_api: HousekeeperAPI,
+    workflow: Workflow,
     caplog: LogCaptureFixture,
-    case_id_does_not_exist: str,
+    deliverables_template_content: list[dict],
+    request: FixtureRequest,
+    mocker,
 ):
-    """Test command with invalid case to start with."""
-    caplog.set_level(logging.ERROR)
+    """Test to ensure all parts of store command are run successfully given ideal conditions."""
+    caplog.set_level(logging.INFO)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
-    # GIVEN case_id not in database
-    assert not rnafusion_context.status_db.get_case_by_internal_id(
-        internal_id=case_id_does_not_exist
+    # GIVEN a case for which we mocked files created after a successful run
+    case_id: str = request.getfixturevalue(f"{workflow}_case_id")
+    hermes_deliverables: dict = request.getfixturevalue(f"{workflow}_hermes_deliverables")
+    request.getfixturevalue(f"{workflow}_mock_deliverable_dir")
+    request.getfixturevalue(f"{workflow}_mock_analysis_finish")
+    deliverables_response_data = request.getfixturevalue(f"{workflow}_deliverables_response_data")
+
+    # GIVEN a mocked deliverables template
+    mocker.patch.object(
+        NfAnalysisAPI,
+        "get_deliverables_template_content",
+        return_value=deliverables_template_content,
     )
 
-    # WHEN running
-    result = cli_runner.invoke(store_housekeeper, [case_id_does_not_exist], obj=rnafusion_context)
-
-    # THEN command should NOT successfully call the command it creates
-    assert result.exit_code != EXIT_SUCCESS
+    # GIVEN that the Housekeeper store is empty
+    context.housekeeper_api_: HousekeeperAPI = real_housekeeper_api
+    context.meta_apis["analysis_api"].housekeeper_api = real_housekeeper_api
 
-    # THEN ERROR log should be printed containing invalid case_id
-    assert case_id_does_not_exist in caplog.text
-    assert "could not be found" in caplog.text
+    # GIVEN that the bundle is not present in Housekeeper
+    assert not context.housekeeper_api.bundle(case_id)
 
+    # GIVEN that the analysis is not already stored in status_db
+    assert not context.status_db.get_case_by_internal_id(internal_id=case_id).analyses
 
-def test_case_not_finished(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
-):
-    """Test command with case_id and config file but no analysis_finish."""
-    caplog.set_level(logging.ERROR)
-    # GIVEN case-id
-    case_id: str = rnafusion_case_id
+    # GIVEN that HermesAPI returns a deliverables output
+    mocker.patch.object(HermesApi, "convert_deliverables")
+    HermesApi.convert_deliverables.return_value = CGDeliverables.model_validate(hermes_deliverables)
 
-    # WHEN running
-    result = cli_runner.invoke(store_housekeeper, [case_id], obj=rnafusion_context)
+    # GIVEN Hermes parses deliverables and generates a valid response
+    mocker.patch.object(HermesApi, "create_housekeeper_bundle")
+    HermesApi.create_housekeeper_bundle.return_value = deliverables_response_data
 
-    # THEN command should NOT execute successfully
-    assert result.exit_code != EXIT_SUCCESS
+    # WHEN storing the case files
+    result = cli_runner.invoke(workflow_cli, [workflow, "store", case_id], obj=context)
 
-    # THEN warning should be printed that no deliverables file has been found
-    assert "No deliverables file found for case" in caplog.text
+    # THEN bundle should be successfully added to Housekeeper and StatusDB
+    assert result.exit_code == EXIT_SUCCESS
+    assert "Analysis successfully stored in Housekeeper" in caplog.text
+    assert "Analysis successfully stored in StatusDB" in caplog.text
+    assert context.status_db.get_case_by_internal_id(internal_id=case_id).analyses
+    assert context.housekeeper_api.bundle(case_id)
 
 
-def test_case_with_malformed_deliverables_file(
-    cli_runner,
-    mocker,
-    rnafusion_context: CGConfig,
-    malformed_hermes_deliverables: dict,
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
+)
+def test_store_fail(
+    cli_runner: CliRunner,
+    workflow: Workflow,
+    real_housekeeper_api: HousekeeperAPI,
+    deliverables_template_content: list[dict],
     caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
+    request: FixtureRequest,
+    mocker,
 ):
-    """Test command with case_id and config file and analysis_finish but malformed deliverables output."""
-    caplog.set_level(logging.WARNING)
-    # GIVEN a malformed output from hermes
-    analysis_api: RnafusionAnalysisAPI = rnafusion_context.meta_apis["analysis_api"]
-
-    # GIVEN that HermesAPI returns a malformed deliverables output
-    mocker.patch.object(Process, "run_command")
-    Process.run_command.return_value = WriteStream.write_stream_from_content(
-        content=malformed_hermes_deliverables, file_format=FileFormat.JSON
-    )
+    """Test store command fails when a case did not finish for a workflow."""
+    caplog.set_level(logging.INFO)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
+
+    # GIVEN a case id where analysis finish is not mocked
+    case_id_fail: str = request.getfixturevalue(f"{workflow}_case_id")
 
-    # GIVEN that the output is malformed
-    with pytest.raises(ValidationError):
-        analysis_api.hermes_api.convert_deliverables(
-            deliverables_file=Path("a_file"), workflow="rnafusion"
-        )
+    # GIVEN a mocked deliverables template
+    mocker.patch.object(
+        NfAnalysisAPI,
+        "get_deliverables_template_content",
+        return_value=deliverables_template_content,
+    )
 
-        # GIVEN case-id
-        case_id: str = rnafusion_case_id
+    # GIVEN that the Housekeeper store is empty
+    context.housekeeper_api_: HousekeeperAPI = real_housekeeper_api
+    context.meta_apis["analysis_api"].housekeeper_api = real_housekeeper_api
 
-        # WHEN running
-        result = cli_runner.invoke(store_housekeeper, [case_id], obj=rnafusion_context)
+    # GIVEN that the bundle is not present in Housekeeper
+    assert not context.housekeeper_api.bundle(case_id_fail)
 
-        # THEN command should NOT execute successfully
-        assert result.exit_code != EXIT_SUCCESS
+    # WHEN running command
+    result_fail = cli_runner.invoke(workflow_cli, [workflow, "store", case_id_fail], obj=context)
 
-        # THEN information that the file is malformed should be communicated
-        assert "Deliverables file is malformed" in caplog.text
-        assert "field required" in caplog.text
+    # THEN bundle exist status should be
+    assert result_fail.exit_code != EXIT_SUCCESS
 
 
-def test_valid_case(
-    cli_runner,
-    mocker,
-    hermes_deliverables,
-    rnafusion_context: CGConfig,
-    mock_deliverable,
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
+)
+def test_store_available_success(
+    cli_runner: CliRunner,
+    workflow: Workflow,
+    real_housekeeper_api: HousekeeperAPI,
+    deliverables_template_content: list[dict],
+    request: FixtureRequest,
     caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
-    workflow_version: str,
+    mocker,
 ):
+    """
+    Test to ensure all parts of the compound store-available command are executed given ideal
+    conditions.
+    """
     caplog.set_level(logging.INFO)
-    # GIVEN case-id
-    case_id: str = rnafusion_case_id
-
-    # Make sure nothing is currently stored in Housekeeper
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
-    # Make sure analysis not already stored in StatusDB
-    assert not rnafusion_context.status_db.get_case_by_internal_id(internal_id=case_id).analyses
+    # GIVEN a case for which we mocked files created after a successful run
+    hermes_deliverables: dict = request.getfixturevalue(f"{workflow}_hermes_deliverables")
+    case_id: str = request.getfixturevalue(f"{workflow}_case_id")
+    request.getfixturevalue(f"{workflow}_mock_deliverable_dir")
+    request.getfixturevalue(f"{workflow}_mock_analysis_finish")
+
+    # GIVEN that the Housekeeper store is empty
+    context.housekeeper_api_: HousekeeperAPI = real_housekeeper_api
+    context.meta_apis["analysis_api"].housekeeper_api = real_housekeeper_api
 
     # GIVEN that HermesAPI returns a deliverables output
     mocker.patch.object(HermesApi, "convert_deliverables")
-    HermesApi.convert_deliverables.return_value = CGDeliverables(**hermes_deliverables)
+    HermesApi.convert_deliverables.return_value = CGDeliverables.model_validate(hermes_deliverables)
+
+    # GIVEN there is available cases to store
+    context.status_db.get_case_by_internal_id(case_id).action = CaseActions.RUNNING
+    context.status_db.session.commit()
 
     # WHEN running command
-    result = cli_runner.invoke(store_housekeeper, [case_id], obj=rnafusion_context)
+    result = cli_runner.invoke(workflow_cli, [workflow, "store-available"], obj=context)
 
-    # THEN a bundle should be successfully added to HK and StatusDB
+    # THEN command exits successfully
     assert result.exit_code == EXIT_SUCCESS
-    assert "Analysis successfully stored in Housekeeper" in caplog.text
-    assert "Analysis successfully stored in StatusDB" in caplog.text
-    assert rnafusion_context.status_db.get_case_by_internal_id(internal_id=case_id).analyses
-    assert rnafusion_context.meta_apis["analysis_api"].housekeeper_api.bundle(case_id)
 
-    # THEN a workflow version should be correctly stored
-    assert (
-        rnafusion_context.status_db.get_case_by_internal_id(internal_id=case_id)
-        .analyses[0]
-        .workflow_version
-        == workflow_version
-    )
+    # THEN all expected cases are picked up for storing
+    assert f"Storing deliverables for {case_id}" in caplog.text
 
+    # THEN case has an associated analysis
+    assert len(context.status_db.get_case_by_internal_id(case_id).analyses) == 1
 
-def test_valid_case_already_added(
-    cli_runner,
-    mocker,
-    hermes_deliverables,
-    rnafusion_context: CGConfig,
+    # THEN bundle can be found in Housekeeper
+    assert context.housekeeper_api.bundle(case_id)
+
+    # THEN StatusDB action is set to None
+    assert context.status_db.get_case_by_internal_id(case_id).action is None
+
+
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
+)
+def test_store_available_fail(
+    cli_runner: CliRunner,
+    workflow: Workflow,
     real_housekeeper_api: HousekeeperAPI,
-    mock_deliverable,
+    deliverables_template_content: list[dict],
+    case_id_not_enough_reads: str,
+    sample_id: str,
+    request: FixtureRequest,
     caplog: LogCaptureFixture,
-    rnafusion_case_id: str,
+    mocker,
 ):
+    """
+    Test that store-available picks up eligible cases and does not stop after failing to store a case.
+    """
     caplog.set_level(logging.INFO)
-    # GIVEN case-id
-    case_id: str = rnafusion_case_id
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
-    # Make sure nothing is currently stored in Housekeeper
-    rnafusion_context.housekeeper_api_: HousekeeperAPI = real_housekeeper_api
-    rnafusion_context.meta_apis["analysis_api"].housekeeper_api = real_housekeeper_api
+    # GIVEN a case for which we mocked files created after a successful run
+    hermes_deliverables: dict = request.getfixturevalue(f"{workflow}_hermes_deliverables")
+    case_id: str = request.getfixturevalue(f"{workflow}_case_id")
+    request.getfixturevalue(f"{workflow}_mock_deliverable_dir")
+    request.getfixturevalue(f"{workflow}_mock_analysis_finish")
+
+    # GIVEN a case where analysis finish is not mocked
+    failed_case_id: str = case_id_not_enough_reads
+
+    # GIVEN that the Housekeeper store is empty
+    context.housekeeper_api_: HousekeeperAPI = real_housekeeper_api
+    context.meta_apis["analysis_api"].housekeeper_api = real_housekeeper_api
 
-    # Make sure  analysis not already stored in ClinicalDB
-    assert not rnafusion_context.status_db.get_case_by_internal_id(internal_id=case_id).analyses
     # GIVEN that HermesAPI returns a deliverables output
     mocker.patch.object(HermesApi, "convert_deliverables")
-    HermesApi.convert_deliverables.return_value = CGDeliverables(**hermes_deliverables)
-
-    # Ensure bundles exist by creating them first
-    result_first = cli_runner.invoke(store_housekeeper, [case_id], obj=rnafusion_context)
+    HermesApi.convert_deliverables.return_value = CGDeliverables.model_validate(hermes_deliverables)
 
-    # GIVEN that the first command executed successfully
-    assert result_first.exit_code == EXIT_SUCCESS
+    # GIVEN there is available cases to store
+    context.status_db.get_case_by_internal_id(case_id).action = CaseActions.RUNNING
+    context.status_db.get_case_by_internal_id(failed_case_id).action = CaseActions.RUNNING
+    context.status_db.session.commit()
 
     # WHEN running command
-    result = cli_runner.invoke(store_housekeeper, [case_id], obj=rnafusion_context)
+    result = cli_runner.invoke(workflow_cli, [workflow, "store-available"], obj=context)
 
-    # THEN command should NOT execute successfully
-    assert result.exit_code != EXIT_SUCCESS
+    # THEN command should not exit successfully
+    assert result.exit_code == EXIT_FAIL
 
-    # THEN user should be informed that bundle was already added
-    assert "Bundle already added" in caplog.text
+    # THEN all expected cases are picked up for storing
+    for case in [failed_case_id, case_id]:
+        assert f"Storing deliverables for {case}" in caplog.text
 
+    # THEN one case failed to store
+    assert f"Error storing {failed_case_id}" in caplog.text
 
-def test_dry_run(
-    cli_runner: CliRunner,
-    rnafusion_context: CGConfig,
-    mock_deliverable: None,
-    caplog: LogCaptureFixture,
-    mocker: MockFixture,
-    rnafusion_case_id: str,
-    hermes_deliverables: dict,
-    real_housekeeper_api: HousekeeperAPI,
-):
-    """Test dry run given a successfully finished and delivered case."""
-    caplog.set_level(logging.INFO)
+    # THEN case failing store does not have an associated analysis
+    assert not context.status_db.get_case_by_internal_id(failed_case_id).analyses
 
-    # GIVEN case-id for which we created a config file, deliverables file, and analysis_finish file
-    case_id: str = rnafusion_case_id
+    # THEN case with successful store has an associated analysis
+    assert len(context.status_db.get_case_by_internal_id(case_id).analyses) == 1
 
-    # Set Housekeeper to an empty real Housekeeper store
-    rnafusion_context.housekeeper_api_: HousekeeperAPI = real_housekeeper_api
-    rnafusion_context.meta_apis["analysis_api"].housekeeper_api = real_housekeeper_api
+    # THEN case failing store does not have an associated Housekeeper bundle
+    assert not context.housekeeper_api.bundle(failed_case_id)
 
-    # GIVEN that HermesAPI returns a deliverables output
-    mocker.patch.object(HermesApi, "convert_deliverables")
-    HermesApi.convert_deliverables.return_value = CGDeliverables(**hermes_deliverables)
-
-    # Make sure the bundle was not present in hk
-    assert not rnafusion_context.housekeeper_api.bundle(case_id)
+    # THEN bundle can be found in Housekeeper for successful case
+    assert context.housekeeper_api.bundle(case_id)
 
-    # Make sure analysis not already stored in status_db
-    assert not rnafusion_context.status_db.get_case_by_internal_id(internal_id=case_id).analyses
+    # THEN StatusDB action remains as running for case failing store
+    assert context.status_db.get_case_by_internal_id(failed_case_id).action == CaseActions.RUNNING
 
-    # WHEN running command
-    result = cli_runner.invoke(store_housekeeper, [case_id, "--dry-run"], obj=rnafusion_context)
-
-    # THEN bundle should not be added to HK nor STATUSDB
-    assert result.exit_code == EXIT_SUCCESS
-    assert "Dry-run: Housekeeper changes will not be commited" in caplog.text
-    assert "Dry-run: StatusDB changes will not be commited" in caplog.text
-    assert not rnafusion_context.housekeeper_api.bundle(case_id)
+    # THEN StatusDB action is set to None for successful case
+    assert not context.status_db.get_case_by_internal_id(case_id).action
```

### Comparing `cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_run.py` & `cg-60.0.0/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,107 @@
-"""This module tests the run CLI command."""
+"""Tests CLI common methods to create the case config for NF analyses."""
 
 import logging
+from pathlib import Path
 
+import pytest
+from _pytest.fixtures import FixtureRequest
 from _pytest.logging import LogCaptureFixture
 from click.testing import CliRunner
 
-from cg.cli.workflow.taxprofiler.base import run
-from cg.constants import EXIT_SUCCESS
+from cg.cli.workflow.base import workflow as workflow_cli
+from cg.constants import EXIT_SUCCESS, Workflow
+from cg.io.yaml import read_yaml
 from cg.models.cg_config import CGConfig
 
+LOG = logging.getLogger(__name__)
 
-def test_without_options(cli_runner: CliRunner, taxprofiler_context: CGConfig):
-    """Test command without case id argument."""
-    # GIVEN no case_id
-    # WHEN dry running without anything specified
-    result = cli_runner.invoke(run, obj=taxprofiler_context)
-    # THEN command should NOT execute successfully
+
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
+)
+def test_metrics_deliver_without_options(
+    cli_runner: CliRunner, workflow: Workflow, request: FixtureRequest
+):
+    """Test metrics-deliver for workflow without options."""
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
+
+    # WHEN invoking the command without additional parameters
+    result = cli_runner.invoke(workflow_cli, [workflow, "metrics-deliver"], obj=context)
+
+    # THEN command should not exit successfully
     assert result.exit_code != EXIT_SUCCESS
-    # THEN command should mention argument
+
+    # THEN command log should inform about missing arguments
     assert "Missing argument" in result.output
 
 
-def test_with_missing_case(
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
+)
+def test_metrics_deliver_with_missing_case(
     cli_runner: CliRunner,
-    taxprofiler_context: CGConfig,
     caplog: LogCaptureFixture,
     case_id_does_not_exist: str,
+    workflow: Workflow,
+    request: FixtureRequest,
 ):
-    """Test run command with invalid case."""
+    """Test metrics-deliver for workflow with a missing case."""
     caplog.set_level(logging.ERROR)
-    # GIVEN case_id not in database
-    assert not taxprofiler_context.status_db.get_case_by_internal_id(
-        internal_id=case_id_does_not_exist
-    )
-    # WHEN running
-    result = cli_runner.invoke(run, [case_id_does_not_exist], obj=taxprofiler_context)
-    # THEN command should NOT successfully call the command it creates
-    assert result.exit_code != EXIT_SUCCESS
-    # THEN ERROR log should be printed containing invalid case_id
-    assert case_id_does_not_exist in caplog.text
-    assert f"{case_id_does_not_exist} could not be found" in caplog.text
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
+    # GIVEN a case not in the StatusDB database
+    assert not context.status_db.get_case_by_internal_id(internal_id=case_id_does_not_exist)
 
-def test_with_config_use_nextflow(
-    cli_runner: CliRunner,
-    taxprofiler_context: CGConfig,
-    caplog: LogCaptureFixture,
-    taxprofiler_case_id: str,
-    taxprofiler_config,
-):
-    """Test command with case_id and config file using nextflow."""
-    caplog.set_level(logging.INFO)
-    # GIVEN case-id
-    case_id: str = taxprofiler_case_id
-
-    # GIVEN a mocked config
-
-    # WHEN dry running with dry specified
+    # WHEN running
     result = cli_runner.invoke(
-        run, [case_id, "--dry-run", "--use-nextflow"], obj=taxprofiler_context
+        workflow_cli, [workflow, "metrics-deliver", case_id_does_not_exist], obj=context
     )
 
-    # THEN command should execute successfully
-    assert result.exit_code == EXIT_SUCCESS
+    # THEN command should not exit successfully
+    assert result.exit_code != EXIT_SUCCESS
 
-    for message in [
-        "using Nextflow",
-        "path/to/bin/nextflow",
-        "-work-dir",
-        "-params-file",
-        "-resume",
-    ]:
-        assert message in caplog.text
+    # THEN ERROR log should be printed containing invalid case_id
+    assert case_id_does_not_exist in caplog.text
+    assert "could not be found" in caplog.text
 
 
-def test_with_config_use_tower(
+@pytest.mark.parametrize(
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
+)
+def test_metrics_deliver_case(
     cli_runner: CliRunner,
-    taxprofiler_context: CGConfig,
     caplog: LogCaptureFixture,
-    taxprofiler_case_id: str,
-    taxprofiler_config,
+    workflow: Workflow,
+    request: FixtureRequest,
 ):
-    """Test command with case_id and config file using tower."""
+    """Test command with a case id and a finished analysis which should execute successfully."""
     caplog.set_level(logging.INFO)
-    # GIVEN  a valid case
-    case_id: str = taxprofiler_case_id
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
 
-    # GIVEN a mocked config
+    # GIVEN a case for which we mocked files created after a successful run
+    case_id: str = request.getfixturevalue(f"{workflow}_case_id")
+    metrics_deliverables_path: Path = request.getfixturevalue(
+        f"{workflow}_metrics_deliverables_path"
+    )
+    request.getfixturevalue(f"{workflow}_mock_deliverable_dir")
+    request.getfixturevalue(f"{workflow}_mock_analysis_finish")
 
-    # WHEN dry running with dry specified
-    result = cli_runner.invoke(run, [case_id, "--from-start", "--dry-run"], obj=taxprofiler_context)
+    # WHEN invoking the command
+    result = cli_runner.invoke(workflow_cli, [workflow, "metrics-deliver", case_id], obj=context)
 
     # THEN command should execute successfully
     assert result.exit_code == EXIT_SUCCESS
 
-    # THEN command should use tower
-
-    for message in [
-        "using Tower",
-        "path/to/bin/tw launch",
-    ]:
-        assert message in caplog.text
-
-
-def test_with_config_use_tower_resume(
-    cli_runner: CliRunner,
-    taxprofiler_context: CGConfig,
-    caplog: LogCaptureFixture,
-    taxprofiler_case_id: str,
-    taxprofiler_config,
-    tower_id,
-):
-    """Test resume command with tower to use tw run instead of tw launch."""
-    caplog.set_level(logging.INFO)
-
-    # GIVEN a taxprofiler case-id and mocked config
-
-    # WHEN dry running with dry specified
-    result = cli_runner.invoke(
-        run, [taxprofiler_case_id, "--nf-tower-id", tower_id, "--dry-run"], obj=taxprofiler_context
-    )
-
-    # THEN command should execute successfully
-    assert result.exit_code == EXIT_SUCCESS
+    # THEN metrics deliverable file should be generated
+    assert "Writing metrics deliverables file to" in caplog.text
+    assert metrics_deliverables_path.is_file()
+
+    # WHEN reading metrics_deliverable_content as yaml
+    metrics_deliverables_content = read_yaml(file_path=metrics_deliverables_path)
+    assert isinstance(metrics_deliverables_content, dict)
 
-    # THEN command should use tower for relaunch
-    assert "Workflow will be resumed from run" in caplog.text
-    assert "path/to/bin/tw runs relaunch" in caplog.text
+    # THEN the metrics_deliverables file contains the key "metrics"
+    assert "metrics" in metrics_deliverables_content.keys()
```

### Comparing `cg-59.9.1/tests/cli/workflow/test_cli_workflow.py` & `cg-60.0.0/tests/cli/workflow/test_cli_workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,8 +17,10 @@
     assert result.exit_code == EXIT_SUCCESS
     assert "balsamic" in result.output
     assert "balsamic-qc" in result.output
     assert "balsamic-umi" in result.output
     assert "microsalt" in result.output
     assert "mip-dna" in result.output
     assert "mip-rna" in result.output
+    assert "raredisease" in result.output
     assert "rnafusion" in result.output
+    assert "taxprofiler" in result.output
```

### Comparing `cg-59.9.1/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-60.0.0/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/clients/conftest.py` & `cg-60.0.0/tests/clients/janus/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
 
 @pytest.fixture
 def mock_post_request_ok(janus_response: dict, mocker: MockFixture) -> MockFixture:
     mocked_response = mocker.Mock()
     mocked_response.status_code = HTTPStatus.OK
     mocked_response.json.return_value = janus_response
+    mocked_response.verify = False
     return mocked_response
 
 
 @pytest.fixture
 def mock_post_request_not_found(janus_response: dict, mocker: MockFixture) -> MockFixture:
     mocked_response = mocker.Mock()
     mocked_response.status_code = HTTPStatus.NOT_FOUND
```

### Comparing `cg-59.9.1/tests/clients/janus/test_janus_api_client.py` & `cg-60.0.0/tests/clients/janus/test_janus_api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,19 @@
     mocked_post.return_value = mock_post_request_ok
 
     # WHEN retrieving the qc metrics
     jobs_response: dict = janus_client.qc_metrics(collect_qc_request_balsamic_wgs)
 
     # THEN the qc metrics are deserialized without error
     assert jobs_response == janus_response
-
-    # Additional assertions for the mocked requests.post
     mocked_post.assert_called_once_with(
-        f"{janus_client.host}/collect_qc_metrics",
+        f"{janus_client.host}/collect_qc",
         data=collect_qc_request_balsamic_wgs.model_dump_json(),
+        verify=True,
     )
-    mock_post_request_ok.json.assert_called_once()
 
 
 def test_qc_metrics_not_successful(
     mocker: MockFixture,
     janus_client: JanusAPIClient,
     collect_qc_request_balsamic_wgs: CreateQCMetricsRequest,
     janus_response: dict,
```

### Comparing `cg-59.9.1/tests/conftest.py` & `cg-60.0.0/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.apps.demultiplex.sample_sheet.api import SampleSheetAPI
 from cg.apps.downsample.downsample import DownsampleAPI
 from cg.apps.gens import GensAPI
 from cg.apps.gt import GenotypeAPI
 from cg.apps.hermes.hermes_api import HermesApi
 from cg.apps.housekeeper.hk import HousekeeperAPI
+from cg.apps.housekeeper.models import InputBundle
 from cg.apps.lims import LimsAPI
 from cg.apps.slurm.slurm_api import SlurmAPI
 from cg.constants import FileExtensions, SequencingFileTag, Workflow
 from cg.constants.constants import CaseActions, FileFormat, Strandedness
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.constants.housekeeper_tags import HK_DELIVERY_REPORT_TAG
 from cg.constants.priority import SlurmQos
@@ -38,20 +39,23 @@
 from cg.meta.encryption.encryption import FlowCellEncryptionAPI
 from cg.meta.rsync import RsyncAPI
 from cg.meta.tar.tar import TarAPI
 from cg.meta.transfer.external_data import ExternalDataAPI
 from cg.meta.workflow.raredisease import RarediseaseAnalysisAPI
 from cg.meta.workflow.rnafusion import RnafusionAnalysisAPI
 from cg.meta.workflow.taxprofiler import TaxprofilerAnalysisAPI
+from cg.meta.workflow.tomte import TomteAnalysisAPI
 from cg.models import CompressionData
 from cg.models.cg_config import CGConfig, PDCArchivingDirectory
 from cg.models.downsample.downsample_data import DownsampleData
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
-from cg.models.rnafusion.rnafusion import RnafusionParameters
-from cg.models.taxprofiler.taxprofiler import TaxprofilerParameters
+from cg.models.raredisease.raredisease import RarediseaseSampleSheetHeaders
+from cg.models.rnafusion.rnafusion import RnafusionParameters, RnafusionSampleSheetEntry
+from cg.models.taxprofiler.taxprofiler import TaxprofilerParameters, TaxprofilerSampleSheetEntry
+from cg.models.tomte.tomte import TomteSampleSheetHeaders
 from cg.store.database import create_all_tables, drop_all_tables, initialize_database
 from cg.store.models import Bed, BedVersion, Case, Customer, Order, Organism, Sample
 from cg.store.store import Store
 from cg.utils import Process
 from tests.mocks.crunchy import MockCrunchyAPI
 from tests.mocks.hk_mock import MockHousekeeperAPI
 from tests.mocks.limsmock import MockLimsAPI
@@ -60,23 +64,28 @@
 from tests.mocks.process_mock import ProcessMock
 from tests.mocks.scout import MockScoutAPI
 from tests.mocks.tb_mock import MockTB
 from tests.small_helpers import SmallHelpers
 from tests.store_helpers import StoreHelpers
 
 LOG = logging.getLogger(__name__)
-
+multiqc_json_file = "multiqc_data.json"
+software_version_file = "software_versions.yml"
+deliverables_yaml = "_deliverables.yaml"
 pytest_plugins = [
     "tests.fixture_plugins.timestamp_fixtures",
     "tests.fixture_plugins.demultiplex_fixtures.flow_cell_fixtures",
     "tests.fixture_plugins.demultiplex_fixtures.name_fixtures",
     "tests.fixture_plugins.demultiplex_fixtures.path_fixtures",
     "tests.fixture_plugins.demultiplex_fixtures.run_parameters_fixtures",
     "tests.fixture_plugins.demultiplex_fixtures.sample_fixtures",
     "tests.fixture_plugins.demultiplex_fixtures.sample_sheet_fixtures",
+    "tests.fixture_plugins.delivery_fixtures.context_fixtures",
+    "tests.fixture_plugins.delivery_fixtures.bundle_fixtures",
+    "tests.fixture_plugins.delivery_fixtures.path_fixtures",
 ]
 
 # Case fixtures
 
 
 @pytest.fixture(scope="session")
 def any_string() -> str:
@@ -97,27 +106,32 @@
 
 @pytest.fixture(scope="session")
 def user_mail() -> str:
     """Return a user email."""
     return "paul@magnolia.com"
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture(scope="function")
 def email_address() -> str:
     """Return an email address."""
     return "user.name@scilifelab.se"
 
 
 @pytest.fixture(scope="session")
 def case_id() -> str:
     """Return a case id."""
     return "yellowhog"
 
 
 @pytest.fixture(scope="session")
+def case_name() -> str:
+    return "C12345"
+
+
+@pytest.fixture(scope="session")
 def case_id_does_not_exist() -> str:
     """Return a case id that should not exist."""
     return "case_does_not_exist"
 
 
 @pytest.fixture(scope="session")
 def another_case_id() -> str:
@@ -128,14 +142,20 @@
 @pytest.fixture(scope="session")
 def sample_id() -> str:
     """Return a sample id."""
     return "ADM1"
 
 
 @pytest.fixture(scope="session")
+def another_sample_id() -> str:
+    """Return another sample id."""
+    return "another_sample_id"
+
+
+@pytest.fixture(scope="session")
 def father_sample_id() -> str:
     """Return the sample id of the father."""
     return "ADM2"
 
 
 @pytest.fixture(scope="session")
 def mother_sample_id() -> str:
@@ -187,14 +207,19 @@
 
 @pytest.fixture(scope="session")
 def sbatch_job_number() -> int:
     return 123456
 
 
 @pytest.fixture(scope="session")
+def empty_list() -> list:
+    return []
+
+
+@pytest.fixture(scope="session")
 def sbatch_process(sbatch_job_number: int) -> ProcessMock:
     """Return a mocked process object."""
     slurm_process = ProcessMock(binary="sbatch")
     slurm_process.set_stdout(text=str(sbatch_job_number))
     return slurm_process
 
 
@@ -739,14 +764,26 @@
 @pytest.fixture
 def mip_dna_analysis_dir(mip_analysis_dir: Path) -> Path:
     """Return the path to the directory with mip dna analysis files."""
     return Path(mip_analysis_dir, "dna")
 
 
 @pytest.fixture
+def nf_analysis_analysis_dir(fixtures_dir: Path) -> Path:
+    """Return the path to the directory with nf-analysis files."""
+    return Path(fixtures_dir, "analysis", "nf-analysis")
+
+
+@pytest.fixture
+def raredisease_analysis_dir(analysis_dir: Path) -> Path:
+    """Return the path to the directory with raredisease analysis files."""
+    return Path(analysis_dir, "raredisease")
+
+
+@pytest.fixture
 def rnafusion_analysis_dir(analysis_dir: Path) -> Path:
     """Return the path to the directory with rnafusion analysis files."""
     return Path(analysis_dir, "rnafusion")
 
 
 @pytest.fixture
 def taxprofiler_analysis_dir(analysis_dir: Path) -> Path:
@@ -1187,23 +1224,23 @@
         store, flow_cell_name_demultiplexed_with_bcl_convert, sequencer_type="novaseq"
     )
     helpers.add_flow_cell(
         store, flow_cell_name_demultiplexed_with_bcl2fastq, sequencer_type="hiseqx"
     )
     for i, sample_internal_id in enumerate(bcl_convert_demultiplexed_flow_cell_sample_internal_ids):
         helpers.add_sample(store, internal_id=sample_internal_id, name=f"sample_bcl_convert_{i}")
-        helpers.add_sample_lane_sequencing_metrics(
+        helpers.ensure_sample_lane_sequencing_metrics(
             store,
             sample_internal_id=sample_internal_id,
             flow_cell_name=flow_cell_name_demultiplexed_with_bcl_convert,
         )
 
     for i, sample_internal_id in enumerate(bcl2fastq_demultiplexed_flow_cell_sample_internal_ids):
         helpers.add_sample(store, internal_id=sample_internal_id, name=f"sample_bcl2fastq_{i}")
-        helpers.add_sample_lane_sequencing_metrics(
+        helpers.ensure_sample_lane_sequencing_metrics(
             store,
             sample_internal_id=sample_internal_id,
             flow_cell_name=flow_cell_name_demultiplexed_with_bcl2fastq,
         )
     return store
 
 
@@ -1242,14 +1279,20 @@
 @pytest.fixture(name="wgs_application_tag")
 def wgs_application_tag() -> str:
     """Return the WGS application tag."""
     return "WGSPCFC030"
 
 
 @pytest.fixture
+def microbial_application_tag() -> str:
+    """Return the WGS microbial application tag."""
+    return "MWRNXTR003"
+
+
+@pytest.fixture
 def store() -> Generator[Store, None, None]:
     """Return a CG store."""
     initialize_database("sqlite:///")
     _store = Store()
     create_all_tables()
     yield _store
     drop_all_tables()
@@ -1646,14 +1689,26 @@
 def pdc_archiving_directory(pdc_archiving_dir: Path) -> PDCArchivingDirectory:
     """Returns different PDC archiving directories."""
     return PDCArchivingDirectory(
         current=f"/{pdc_archiving_dir.as_posix()}/", nas="/ENCRYPT/", pre_nas="/OLD_ENCRYPT/"
     )
 
 
+@pytest.fixture(scope="function")
+def nextflow_binary() -> Path:
+    """Return the path to the nextflow binary."""
+    return Path("path", "to", "bin", "nextflow")
+
+
+@pytest.fixture(scope="function")
+def conda_binary() -> Path:
+    """Return the path to the conda binary."""
+    return Path("path", "to", "bin", "conda")
+
+
 @pytest.fixture(name="cg_uri")
 def cg_uri() -> str:
     """Return a cg URI."""
     return "sqlite:///"
 
 
 @pytest.fixture(name="hk_uri")
@@ -1673,23 +1728,29 @@
     cg_uri: str,
     hk_uri: str,
     email_address: str,
     fluffy_dir: Path,
     housekeeper_dir: Path,
     mip_dir: Path,
     cg_dir: Path,
+    conda_binary: Path,
     balsamic_dir: Path,
     microsalt_dir: Path,
     raredisease_dir: Path,
     rnafusion_dir: Path,
     taxprofiler_dir: Path,
+    tomte_dir: Path,
     illumina_flow_cells_directory: Path,
     illumina_demultiplexed_runs_directory: Path,
     downsample_dir: Path,
     pdc_archiving_directory: PDCArchivingDirectory,
+    nextflow_binary: Path,
+    nf_analysis_platform_config_path: Path,
+    nf_analysis_pipeline_params_path: Path,
+    nf_analysis_pipeline_resource_optimisation_path: Path,
 ) -> dict:
     """Return a context config."""
     return {
         "database": cg_uri,
         "delivery_path": str(cg_dir),
         "illumina_flow_cells_directory": str(illumina_flow_cells_directory),
         "illumina_demultiplexed_runs_directory": str(illumina_demultiplexed_runs_directory),
@@ -1726,15 +1787,15 @@
             "gens_coverage_male_path": str(cg_dir),
             "conda_binary": "a_conda_binary",
             "conda_env": "S_balsamic",
             "loqusdb_path": str(cg_dir),
             "pon_path": str(cg_dir),
             "root": str(balsamic_dir),
             "slurm": {
-                "mail_user": "test.email@scilifelab.se",
+                "mail_user": email_address,
                 "account": "development",
                 "qos": SlurmQos.LOW,
             },
             "swegen_path": str(cg_dir),
         },
         "chanjo": {"binary_path": "echo", "config_path": "chanjo-stage.yaml"},
         "crunchy": {
@@ -1840,60 +1901,83 @@
         "mutant": {
             "binary_path": "echo",
             "conda_binary": "a_conda_binary",
             "conda_env": "S_mutant",
             "root": str(mip_dir),
         },
         "raredisease": {
+            "binary_path": nextflow_binary.as_posix(),
             "compute_env": "nf_tower_compute_env",
-            "conda_binary": Path("path", "to", "bin", "conda").as_posix(),
+            "conda_binary": conda_binary.as_posix(),
             "conda_env": "S_raredisease",
+            "config_platform": str(nf_analysis_platform_config_path),
+            "config_params": str(nf_analysis_pipeline_params_path),
+            "config_resources": str(nf_analysis_pipeline_resource_optimisation_path),
             "launch_directory": Path("path", "to", "launchdir").as_posix(),
             "workflow_path": Path("workflow", "path").as_posix(),
             "profile": "myprofile",
             "references": Path("path", "to", "references").as_posix(),
             "revision": "2.2.0",
             "root": str(raredisease_dir),
             "slurm": {
                 "account": "development",
-                "mail_user": "test.email@scilifelab.se",
+                "mail_user": email_address,
             },
             "tower_workflow": "raredisease",
         },
+        "tomte": {
+            "binary_path": nextflow_binary.as_posix(),
+            "compute_env": "nf_tower_compute_env",
+            "conda_binary": conda_binary.as_posix(),
+            "conda_env": "S_tomte",
+            "config_platform": str(nf_analysis_platform_config_path),
+            "config_params": str(nf_analysis_pipeline_params_path),
+            "config_resources": str(nf_analysis_pipeline_resource_optimisation_path),
+            "workflow_path": Path("workflow", "path").as_posix(),
+            "profile": "myprofile",
+            "references": Path("path", "to", "references").as_posix(),
+            "revision": "2.2.0",
+            "root": str(tomte_dir),
+            "slurm": {
+                "account": "development",
+                "mail_user": email_address,
+            },
+            "tower_workflow": "tomte",
+        },
         "rnafusion": {
-            "binary_path": Path("path", "to", "bin", "nextflow").as_posix(),
+            "binary_path": nextflow_binary.as_posix(),
             "compute_env": "nf_tower_compute_env",
-            "conda_binary": Path("path", "to", "bin", "conda").as_posix(),
+            "conda_binary": conda_binary.as_posix(),
             "conda_env": "S_RNAFUSION",
             "launch_directory": Path("path", "to", "launchdir").as_posix(),
             "workflow_path": Path("workflow", "path").as_posix(),
             "profile": "myprofile",
             "references": Path("path", "to", "references").as_posix(),
             "revision": "2.2.0",
             "root": str(rnafusion_dir),
             "slurm": {
                 "account": "development",
-                "mail_user": "test.email@scilifelab.se",
+                "mail_user": "test.rnafusion.email@scilifelab.se",
             },
             "tower_workflow": "rnafusion",
         },
         "pigz": {"binary_path": "/bin/pigz"},
         "pdc": {"binary_path": "/bin/dsmc"},
         "taxprofiler": {
-            "binary_path": Path("path", "to", "bin", "nextflow").as_posix(),
+            "binary_path": nextflow_binary.as_posix(),
             "compute_env": "nf_tower_compute_env",
-            "root": taxprofiler_dir.as_posix(),
-            "conda_binary": Path("path", "to", "bin", "conda").as_posix(),
+            "root": str(taxprofiler_dir),
+            "conda_binary": conda_binary.as_posix(),
             "conda_env": "S_taxprofiler",
             "launch_directory": Path("path", "to", "launchdir").as_posix(),
             "workflow_path": Path("workflow", "path").as_posix(),
             "databases": Path("path", "to", "databases").as_posix(),
             "profile": "myprofile",
             "hostremoval_reference": Path("path", "to", "hostremoval_reference").as_posix(),
-            "revision": "1.1.4",
+            "revision": "2.2.0",
             "slurm": {
                 "account": "development",
                 "mail_user": "taxprofiler.email@scilifelab.se",
             },
             "tower_workflow": "taxprofiler",
         },
         "scout": {
@@ -1910,14 +1994,16 @@
         },
         "tar": {"binary_path": "/bin/tar"},
         "trailblazer": {
             "host": "https://trailblazer.scilifelab.se/",
             "service_account": "SERVICE",
             "service_account_auth_file": "trailblazer-auth.json",
         },
+        "arnold": {"api_url": "https://arnold.scilifelab.se/"},
+        "janus": {"host": "https://janus.sys.scilifelab.se/"},
     }
 
 
 @pytest.fixture(name="cg_context")
 def cg_context(
     context_config: dict, base_store: Store, housekeeper_api: MockHousekeeperAPI
 ) -> CGConfig:
@@ -2131,26 +2217,14 @@
 @pytest.fixture(scope="session")
 def no_sample_case_id() -> str:
     """Returns a case id of a case with no samples."""
     return "no_sample_case"
 
 
 @pytest.fixture(scope="session")
-def strandedness() -> str:
-    """Return a default strandedness."""
-    return Strandedness.REVERSE
-
-
-@pytest.fixture(scope="session")
-def strandedness_not_permitted() -> str:
-    """Return a not permitted strandedness."""
-    return "double_stranded"
-
-
-@pytest.fixture(scope="session")
 def workflow_version() -> str:
     """Return a workflow version."""
     return "2.2.0"
 
 
 @pytest.fixture(scope="session")
 def fastq_forward_read_path(housekeeper_dir: Path) -> Path:
@@ -2182,21 +2256,224 @@
 
 @pytest.fixture(scope="session")
 def sequencing_platform() -> str:
     """Return a default sequencing platform."""
     return SequencingPlatform.ILLUMINA
 
 
+# Raredisease fixtures
 @pytest.fixture(scope="function")
-def raredisease_dir(tmpdir_factory, apps_dir: Path) -> str:
+def raredisease_dir(tmpdir_factory: Path) -> str:
     """Return the path to the raredisease apps dir."""
     raredisease_dir = tmpdir_factory.mktemp("raredisease")
     return Path(raredisease_dir).absolute().as_posix()
 
 
+@pytest.fixture(scope="session")
+def raredisease_case_id() -> str:
+    """Returns a raredisease case id."""
+    return "raredisease_case_enough_reads"
+
+
+@pytest.fixture(scope="function")
+def raredisease_sample_sheet_content(
+    sample_id: str,
+    raredisease_case_id: str,
+    fastq_forward_read_path: Path,
+    fastq_reverse_read_path: Path,
+    strandedness: str,
+) -> str:
+    """Return the expected sample sheet content  for raredisease."""
+    headers: str = ",".join(RarediseaseSampleSheetHeaders.list())
+    row: str = ",".join(
+        [
+            sample_id,
+            "1",
+            fastq_forward_read_path.as_posix(),
+            fastq_reverse_read_path.as_posix(),
+            "2",
+            "0",
+            "",
+            "",
+            raredisease_case_id,
+        ]
+    )
+    return "\n".join([headers, row])
+
+
+@pytest.fixture(scope="function")
+def hermes_deliverables(deliverable_data: dict, raredisease_case_id: str) -> dict:
+    hermes_output: dict = {"pipeline": "raredisease", "bundle_id": raredisease_case_id, "files": []}
+    for file_info in deliverable_data["files"]:
+        tags: list[str] = []
+        if "html" in file_info["format"]:
+            tags.append("multiqc-html")
+        hermes_output["files"].append({"path": file_info["path"], "tags": tags, "mandatory": True})
+    return hermes_output
+
+
+@pytest.fixture(scope="function")
+def malformed_hermes_deliverables(hermes_deliverables: dict) -> dict:
+    malformed_deliverable: dict = hermes_deliverables.copy()
+    malformed_deliverable.pop("pipeline")
+
+    return malformed_deliverable
+
+
+@pytest.fixture(scope="function")
+def raredisease_sample_sheet_path(raredisease_dir, raredisease_case_id) -> Path:
+    """Path to sample sheet."""
+    return Path(
+        raredisease_dir, raredisease_case_id, f"{raredisease_case_id}_samplesheet"
+    ).with_suffix(FileExtensions.CSV)
+
+
+@pytest.fixture(scope="function")
+def raredisease_params_file_path(raredisease_dir, raredisease_case_id) -> Path:
+    """Path to parameters file."""
+    return Path(
+        raredisease_dir, raredisease_case_id, f"{raredisease_case_id}_params_file"
+    ).with_suffix(FileExtensions.YAML)
+
+
+@pytest.fixture(scope="function")
+def raredisease_nexflow_config_file_path(raredisease_dir, raredisease_case_id) -> Path:
+    """Path to config file."""
+    return Path(
+        raredisease_dir, raredisease_case_id, f"{raredisease_case_id}_nextflow_config"
+    ).with_suffix(FileExtensions.JSON)
+
+
+@pytest.fixture(scope="function")
+def raredisease_deliverables_file_path(raredisease_dir, raredisease_case_id) -> Path:
+    """Path to deliverables file."""
+    return Path(
+        raredisease_dir, raredisease_case_id, f"{raredisease_case_id}_deliverables"
+    ).with_suffix(FileExtensions.YAML)
+
+
+@pytest.fixture(scope="function")
+def raredisease_context(
+    cg_context: CGConfig,
+    helpers: StoreHelpers,
+    nf_analysis_housekeeper: HousekeeperAPI,
+    trailblazer_api: MockTB,
+    raredisease_case_id: str,
+    sample_id: str,
+    no_sample_case_id: str,
+    total_sequenced_reads_pass: int,
+    apptag_rna: str,
+    case_id_not_enough_reads: str,
+    sample_id_not_enough_reads: str,
+    total_sequenced_reads_not_pass: int,
+) -> CGConfig:
+    """context to use in cli"""
+    cg_context.housekeeper_api_ = nf_analysis_housekeeper
+    cg_context.trailblazer_api_ = trailblazer_api
+    cg_context.meta_apis["analysis_api"] = RarediseaseAnalysisAPI(config=cg_context)
+    status_db: Store = cg_context.status_db
+
+    # Create ERROR case with NO SAMPLES
+    helpers.add_case(status_db, internal_id=no_sample_case_id, name=no_sample_case_id)
+
+    # Create textbook case with enough reads
+    case_enough_reads: Case = helpers.add_case(
+        store=status_db,
+        internal_id=raredisease_case_id,
+        name=raredisease_case_id,
+        data_analysis=Workflow.RAREDISEASE,
+    )
+
+    sample_raredisease_case_enough_reads: Sample = helpers.add_sample(
+        status_db,
+        internal_id=sample_id,
+        last_sequenced_at=datetime.now(),
+        reads=total_sequenced_reads_pass,
+        application_tag=apptag_rna,
+    )
+
+    helpers.add_relationship(
+        status_db,
+        case=case_enough_reads,
+        sample=sample_raredisease_case_enough_reads,
+    )
+
+    # Create case without enough reads
+    case_not_enough_reads: Case = helpers.add_case(
+        store=status_db,
+        internal_id=case_id_not_enough_reads,
+        name=case_id_not_enough_reads,
+        data_analysis=Workflow.RAREDISEASE,
+    )
+
+    sample_not_enough_reads: Sample = helpers.add_sample(
+        status_db,
+        internal_id=sample_id_not_enough_reads,
+        last_sequenced_at=datetime.now(),
+        reads=total_sequenced_reads_not_pass,
+        application_tag=apptag_rna,
+    )
+
+    helpers.add_relationship(status_db, case=case_not_enough_reads, sample=sample_not_enough_reads)
+
+    return cg_context
+
+
+@pytest.fixture(scope="function")
+def deliverable_data(raredisease_dir: Path, raredisease_case_id: str, sample_id: str) -> dict:
+    return {
+        "files": [
+            {
+                "path": f"{raredisease_dir}/{raredisease_case_id}/multiqc/multiqc_report.html",
+                "path_index": "",
+                "step": "report",
+                "tag": ["multiqc-html", "rna"],
+                "id": raredisease_case_id,
+                "format": "html",
+                "mandatory": True,
+            },
+        ]
+    }
+
+
+@pytest.fixture(scope="function")
+def mock_deliverable(
+    raredisease_dir: Path, deliverable_data: dict, raredisease_case_id: str
+) -> None:
+    """Create deliverable file with dummy data and files to deliver."""
+    Path.mkdir(
+        Path(raredisease_dir, raredisease_case_id),
+        parents=True,
+        exist_ok=True,
+    )
+    Path.mkdir(
+        Path(raredisease_dir, raredisease_case_id, "multiqc"),
+        parents=True,
+        exist_ok=True,
+    )
+    for report_entry in deliverable_data["files"]:
+        Path(report_entry["path"]).touch(exist_ok=True)
+    WriteFile.write_file_from_content(
+        content=deliverable_data,
+        file_format=FileFormat.JSON,
+        file_path=Path(
+            raredisease_dir, raredisease_case_id, raredisease_case_id + deliverables_yaml
+        ),
+    )
+
+
+@pytest.fixture(scope="function")
+def raredisease_mock_config(raredisease_dir: Path, raredisease_case_id: str) -> None:
+    """Create samplesheet.csv file for testing"""
+    Path.mkdir(Path(raredisease_dir, raredisease_case_id), parents=True, exist_ok=True)
+    Path(raredisease_dir, raredisease_case_id, f"{raredisease_case_id}_samplesheet").with_suffix(
+        FileExtensions.CSV
+    ).touch(exist_ok=True)
+
+
 # Rnafusion fixtures
 
 
 @pytest.fixture(scope="function")
 def rnafusion_dir(tmpdir_factory, apps_dir: Path) -> str:
     """Return the path to the rnafusion apps dir."""
     rnafusion_dir = tmpdir_factory.mktemp("rnafusion")
@@ -2206,54 +2483,74 @@
 @pytest.fixture(scope="session")
 def rnafusion_case_id() -> str:
     """Returns a rnafusion case id."""
     return "rnafusion_case_enough_reads"
 
 
 @pytest.fixture(scope="session")
+def rnafusion_workflow() -> str:
+    """Returns rnafusion workflow."""
+    return "rnafusion"
+
+
+@pytest.fixture(scope="function")
 def rnafusion_sample_sheet_content(
     rnafusion_case_id: str,
     fastq_forward_read_path: Path,
     fastq_reverse_read_path: Path,
     strandedness: str,
 ) -> str:
     """Return the expected sample sheet content  for rnafusion."""
-    return ",".join(
+    headers: str = ",".join(RnafusionSampleSheetEntry.headers())
+    row: str = ",".join(
         [
             rnafusion_case_id,
             fastq_forward_read_path.as_posix(),
             fastq_reverse_read_path.as_posix(),
             strandedness,
         ]
     )
+    return "\n".join([headers, row])
+
+
+@pytest.fixture(scope="session")
+def strandedness() -> str:
+    """Return a default strandedness."""
+    return Strandedness.REVERSE
+
+
+@pytest.fixture(scope="session")
+def strandedness_not_permitted() -> str:
+    """Return a not permitted strandedness."""
+    return "double_stranded"
 
 
 @pytest.fixture(scope="function")
-def hermes_deliverables(deliverable_data: dict, rnafusion_case_id: str) -> dict:
+def rnafusion_hermes_deliverables(rnafusion_deliverable_data: dict, rnafusion_case_id: str) -> dict:
     hermes_output: dict = {"workflow": "rnafusion", "bundle_id": rnafusion_case_id, "files": []}
-    for file_info in deliverable_data["files"]:
+    for file_info in rnafusion_deliverable_data["files"]:
         tags: list[str] = []
         if "html" in file_info["format"]:
             tags.append("multiqc-html")
         hermes_output["files"].append({"path": file_info["path"], "tags": tags, "mandatory": True})
     return hermes_output
 
 
 @pytest.fixture(scope="function")
-def malformed_hermes_deliverables(hermes_deliverables: dict) -> dict:
-    malformed_deliverable: dict = hermes_deliverables.copy()
+def rnafusion_malformed_hermes_deliverables(rnafusion_hermes_deliverables: dict) -> dict:
+    malformed_deliverable: dict = rnafusion_hermes_deliverables.copy()
     malformed_deliverable.pop("workflow")
 
     return malformed_deliverable
 
 
 @pytest.fixture(scope="function")
 def rnafusion_multiqc_json_metrics(rnafusion_analysis_dir) -> dict:
     """Returns the content of a mock Multiqc JSON file."""
-    return read_json(file_path=Path(rnafusion_analysis_dir, "multiqc_data.json"))
+    return read_json(file_path=Path(rnafusion_analysis_dir, multiqc_json_file))
 
 
 @pytest.fixture(scope="function")
 def rnafusion_sample_sheet_path(rnafusion_dir, rnafusion_case_id) -> Path:
     """Path to sample sheet."""
     return Path(rnafusion_dir, rnafusion_case_id, f"{rnafusion_case_id}_samplesheet").with_suffix(
         FileExtensions.CSV
@@ -2283,21 +2580,74 @@
         file_path=Path(
             rnafusion_analysis_dir, "rnafusion_case_enough_reads_metrics_deliverables.yaml"
         )
     )
 
 
 @pytest.fixture(scope="function")
+def rnafusion_metrics_deliverables_path(rnafusion_dir: Path, rnafusion_case_id: str) -> Path:
+    """Path to deliverables file."""
+    return Path(
+        rnafusion_dir, rnafusion_case_id, f"{rnafusion_case_id}_metrics_deliverables"
+    ).with_suffix(FileExtensions.YAML)
+
+
+@pytest.fixture(scope="function")
 def rnafusion_deliverables_file_path(rnafusion_dir, rnafusion_case_id) -> Path:
     """Path to deliverables file."""
     return Path(rnafusion_dir, rnafusion_case_id, f"{rnafusion_case_id}_deliverables").with_suffix(
         FileExtensions.YAML
     )
 
 
+@pytest.fixture(scope="function")
+def nf_analysis_platform_config_path(nf_analysis_analysis_dir) -> Path:
+    """Path to platform config file."""
+    return Path(nf_analysis_analysis_dir, "platform").with_suffix(FileExtensions.CONFIG)
+
+
+@pytest.fixture(scope="function")
+def nf_analysis_pipeline_params_path(nf_analysis_analysis_dir) -> Path:
+    """Path to pipeline params file."""
+    return Path(nf_analysis_analysis_dir, "pipeline_params").with_suffix(FileExtensions.CONFIG)
+
+
+@pytest.fixture(scope="function")
+def rnafusion_deliverables_response_data(
+    create_multiqc_html_file,
+    create_multiqc_json_file,
+    rnafusion_case_id,
+    timestamp_yesterday,
+) -> InputBundle:
+    return InputBundle(
+        **{
+            "files": [
+                {
+                    "path": create_multiqc_json_file.as_posix(),
+                    "tags": ["multiqc-json", rnafusion_case_id],
+                },
+                {
+                    "path": create_multiqc_html_file.as_posix(),
+                    "tags": ["multiqc-html", rnafusion_case_id],
+                },
+            ],
+            "created": timestamp_yesterday,
+            "name": rnafusion_case_id,
+        }
+    )
+
+
+@pytest.fixture(scope="function")
+def nf_analysis_pipeline_resource_optimisation_path(nf_analysis_analysis_dir) -> Path:
+    """Path to pipeline resource optimisation file."""
+    return Path(nf_analysis_analysis_dir, "pipeline_resource_optimisation").with_suffix(
+        FileExtensions.CONFIG
+    )
+
+
 @pytest.fixture(scope="session")
 def tower_id() -> int:
     """Returns a NF-Tower ID."""
     return 123456
 
 
 @pytest.fixture(scope="session")
@@ -2313,15 +2663,15 @@
     rnafusion_sample_sheet_path: Path,
     existing_directory: Path,
 ) -> RnafusionParameters:
     """Return Rnafusion parameters."""
     return RnafusionParameters(
         cluster_options="--qos=normal",
         genomes_base=existing_directory,
-        sample_sheet_path=rnafusion_sample_sheet_path,
+        input=rnafusion_sample_sheet_path,
         outdir=Path(rnafusion_dir, rnafusion_case_id),
         priority="development",
     )
 
 
 @pytest.fixture(scope="session")
 def total_sequenced_reads_pass() -> int:
@@ -2352,17 +2702,35 @@
 ) -> CGConfig:
     """context to use in cli"""
     cg_context.housekeeper_api_ = nf_analysis_housekeeper
     cg_context.trailblazer_api_ = trailblazer_api
     cg_context.meta_apis["analysis_api"] = RnafusionAnalysisAPI(config=cg_context)
     status_db: Store = cg_context.status_db
 
-    # Create ERROR case with NO SAMPLES
+    # Create case with no associated samples
     helpers.add_case(status_db, internal_id=no_sample_case_id, name=no_sample_case_id)
 
+    # Create case without enough reads
+    case_not_enough_reads: Case = helpers.add_case(
+        store=status_db,
+        internal_id=case_id_not_enough_reads,
+        name=case_id_not_enough_reads,
+        data_analysis=Workflow.RNAFUSION,
+    )
+
+    sample_not_enough_reads: Sample = helpers.add_sample(
+        status_db,
+        application_tag=apptag_rna,
+        internal_id=sample_id_not_enough_reads,
+        reads=total_sequenced_reads_not_pass,
+        last_sequenced_at=datetime.now(),
+    )
+
+    helpers.add_relationship(status_db, case=case_not_enough_reads, sample=sample_not_enough_reads)
+
     # Create textbook case with enough reads
     case_enough_reads: Case = helpers.add_case(
         store=status_db,
         internal_id=rnafusion_case_id,
         name=rnafusion_case_id,
         data_analysis=Workflow.RNAFUSION,
     )
@@ -2377,37 +2745,19 @@
 
     helpers.add_relationship(
         status_db,
         case=case_enough_reads,
         sample=sample_rnafusion_case_enough_reads,
     )
 
-    # Create case without enough reads
-    case_not_enough_reads: Case = helpers.add_case(
-        store=status_db,
-        internal_id=case_id_not_enough_reads,
-        name=case_id_not_enough_reads,
-        data_analysis=Workflow.RNAFUSION,
-    )
-
-    sample_not_enough_reads: Sample = helpers.add_sample(
-        status_db,
-        application_tag=apptag_rna,
-        internal_id=sample_id_not_enough_reads,
-        reads=total_sequenced_reads_not_pass,
-        last_sequenced_at=datetime.now(),
-    )
-
-    helpers.add_relationship(status_db, case=case_not_enough_reads, sample=sample_not_enough_reads)
-
     return cg_context
 
 
 @pytest.fixture(scope="function")
-def deliverable_data(rnafusion_dir: Path, rnafusion_case_id: str, sample_id: str) -> dict:
+def rnafusion_deliverable_data(rnafusion_dir: Path, rnafusion_case_id: str, sample_id: str) -> dict:
     return {
         "files": [
             {
                 "path": f"{rnafusion_dir}/{rnafusion_case_id}/multiqc/multiqc_report.html",
                 "path_index": "",
                 "step": "report",
                 "tag": ["multiqc-html", "rna"],
@@ -2416,42 +2766,46 @@
                 "mandatory": True,
             },
         ]
     }
 
 
 @pytest.fixture(scope="function")
-def mock_deliverable(rnafusion_dir: Path, deliverable_data: dict, rnafusion_case_id: str) -> None:
+def rnafusion_mock_deliverable_dir(
+    rnafusion_dir: Path, rnafusion_deliverable_data: dict, rnafusion_case_id: str
+) -> Path:
     """Create deliverable file with dummy data and files to deliver."""
     Path.mkdir(
         Path(rnafusion_dir, rnafusion_case_id),
         parents=True,
         exist_ok=True,
     )
     Path.mkdir(
         Path(rnafusion_dir, rnafusion_case_id, "multiqc"),
         parents=True,
         exist_ok=True,
     )
-    for report_entry in deliverable_data["files"]:
+    for report_entry in rnafusion_deliverable_data["files"]:
         Path(report_entry["path"]).touch(exist_ok=True)
     WriteFile.write_file_from_content(
-        content=deliverable_data,
+        content=rnafusion_deliverable_data,
         file_format=FileFormat.JSON,
-        file_path=Path(rnafusion_dir, rnafusion_case_id, rnafusion_case_id + "_deliverables.yaml"),
+        file_path=Path(rnafusion_dir, rnafusion_case_id, rnafusion_case_id + deliverables_yaml),
     )
 
+    return rnafusion_dir
+
 
 @pytest.fixture(scope="function")
 def rnafusion_mock_analysis_finish(
     rnafusion_dir: Path, rnafusion_case_id: str, rnafusion_multiqc_json_metrics: dict, tower_id: int
 ) -> None:
     """Create analysis_finish file for testing."""
     Path.mkdir(Path(rnafusion_dir, rnafusion_case_id, "pipeline_info"), parents=True, exist_ok=True)
-    Path(rnafusion_dir, rnafusion_case_id, "pipeline_info", "software_versions.yml").touch(
+    Path(rnafusion_dir, rnafusion_case_id, "pipeline_info", software_version_file).touch(
         exist_ok=True
     )
     Path(rnafusion_dir, rnafusion_case_id, f"{rnafusion_case_id}_samplesheet.csv").touch(
         exist_ok=True
     )
     Path.mkdir(
         Path(rnafusion_dir, rnafusion_case_id, "multiqc", "multiqc_data"),
@@ -2475,26 +2829,319 @@
             rnafusion_case_id,
             "tower_ids",
         ).with_suffix(FileExtensions.YAML),
     )
 
 
 @pytest.fixture(scope="function")
-def mock_config(rnafusion_dir: Path, rnafusion_case_id: str) -> None:
+def rnafusion_mock_config(rnafusion_dir: Path, rnafusion_case_id: str) -> None:
     """Create samplesheet.csv file for testing"""
     Path.mkdir(Path(rnafusion_dir, rnafusion_case_id), parents=True, exist_ok=True)
-    Path(rnafusion_dir, rnafusion_case_id, f"{rnafusion_case_id}_samplesheet.csv").touch(
-        exist_ok=True
+    Path(rnafusion_dir, rnafusion_case_id, f"{rnafusion_case_id}_samplesheet.csv").with_suffix(
+        FileExtensions.CSV
+    ).touch(exist_ok=True)
+
+
+# Tomte fixtures
+@pytest.fixture(scope="session")
+def tomte_case_id() -> str:
+    """Returns a tomte case id."""
+    return "tomte_case_enough_reads"
+
+
+@pytest.fixture(scope="function")
+def tomte_dir(tmpdir_factory, apps_dir: Path) -> str:
+    """Return the path to the tomte apps dir."""
+    tomte_dir = tmpdir_factory.mktemp("tomte")
+    return Path(tomte_dir).absolute().as_posix()
+
+
+@pytest.fixture(scope="function")
+def tomte_sample_sheet_path(tomte_dir, tomte_case_id) -> Path:
+    """Path to sample sheet."""
+    return Path(tomte_dir, tomte_case_id, f"{tomte_case_id}_samplesheet").with_suffix(
+        FileExtensions.CSV
+    )
+
+
+@pytest.fixture(scope="function")
+def tomte_params_file_path(tomte_dir, tomte_case_id) -> Path:
+    """Path to parameters file."""
+    return Path(tomte_dir, tomte_case_id, f"{tomte_case_id}_params_file").with_suffix(
+        FileExtensions.YAML
+    )
+
+
+@pytest.fixture(scope="function")
+def tomte_nexflow_config_file_path(tomte_dir, tomte_case_id) -> Path:
+    """Path to config file."""
+    return Path(tomte_dir, tomte_case_id, f"{tomte_case_id}_nextflow_config").with_suffix(
+        FileExtensions.JSON
+    )
+
+
+@pytest.fixture(scope="function")
+def tomte_mock_config(tomte_dir: Path, tomte_case_id: str) -> None:
+    """Create Tomte samplesheet.csv file for testing."""
+    Path.mkdir(Path(tomte_dir, tomte_case_id), parents=True, exist_ok=True)
+    Path(tomte_dir, tomte_case_id, f"{tomte_case_id}_samplesheet").with_suffix(
+        FileExtensions.CSV
+    ).touch(exist_ok=True)
+
+
+@pytest.fixture(scope="function")
+def tomte_metrics_deliverables_path(tomte_dir: Path, tomte_case_id: str) -> Path:
+    """Path to deliverables file."""
+    return Path(tomte_dir, tomte_case_id, f"{tomte_case_id}_metrics_deliverables").with_suffix(
+        FileExtensions.YAML
+    )
+
+
+@pytest.fixture(scope="function")
+def tomte_metrics_deliverables(tomte_analysis_dir: Path) -> list[dict]:
+    """Returns the content of a mock metrics deliverables file."""
+    return read_yaml(
+        file_path=Path(tomte_analysis_dir, "tomte_case_enough_reads_metrics_deliverables.yaml")
+    )
+
+
+@pytest.fixture(scope="function")
+def tomte_deliverable_data(tomte_dir: Path, tomte_case_id: str, sample_id: str) -> dict:
+    return {
+        "files": [
+            {
+                "path": f"{tomte_dir}/{tomte_case_id}/multiqc/multiqc_report.html",
+                "path_index": "",
+                "step": "report",
+                "tag": ["multiqc-html", "rna"],
+                "id": tomte_case_id,
+                "format": "html",
+                "mandatory": True,
+            },
+        ]
+    }
+
+
+@pytest.fixture(scope="function")
+def tomte_multiqc_json_metrics(tomte_analysis_dir) -> dict:
+    """Returns the content of a mock Multiqc JSON file."""
+    return read_json(file_path=Path(tomte_analysis_dir, multiqc_json_file))
+
+
+@pytest.fixture
+def tomte_analysis_dir(analysis_dir: Path) -> Path:
+    """Return the path to the directory with Tomte analysis files."""
+    return Path(analysis_dir, "tomte")
+
+
+@pytest.fixture(scope="function")
+def tomte_mock_deliverable_dir(
+    tomte_dir: Path, tomte_deliverable_data: dict, tomte_case_id: str
+) -> Path:
+    """Create deliverable file with dummy data and files to deliver."""
+    Path.mkdir(
+        Path(tomte_dir, tomte_case_id),
+        parents=True,
+        exist_ok=True,
+    )
+    Path.mkdir(
+        Path(tomte_dir, tomte_case_id, "multiqc"),
+        parents=True,
+        exist_ok=True,
+    )
+    for report_entry in tomte_deliverable_data["files"]:
+        Path(report_entry["path"]).touch(exist_ok=True)
+    WriteFile.write_file_from_content(
+        content=tomte_deliverable_data,
+        file_format=FileFormat.JSON,
+        file_path=Path(tomte_dir, tomte_case_id, tomte_case_id + deliverables_yaml),
+    )
+
+    return tomte_dir
+
+
+@pytest.fixture(scope="function")
+def tomte_sample_sheet_content(
+    tomte_case_id: str,
+    sample_id: str,
+    fastq_forward_read_path: Path,
+    fastq_reverse_read_path: Path,
+    strandedness: str,
+) -> str:
+    """Return the expected sample sheet content for tomte."""
+    headers: str = ",".join(TomteSampleSheetHeaders.list())
+    row: str = ",".join(
+        [
+            tomte_case_id,
+            sample_id,
+            fastq_forward_read_path.as_posix(),
+            fastq_reverse_read_path.as_posix(),
+            strandedness,
+        ]
+    )
+    return "\n".join([headers, row])
+
+
+@pytest.fixture(scope="function")
+def tomte_mock_analysis_finish(
+    tomte_dir: Path, tomte_case_id: str, tomte_multiqc_json_metrics: dict, tower_id: int
+) -> None:
+    """Create analysis_finish file for testing."""
+    Path.mkdir(Path(tomte_dir, tomte_case_id, "pipeline_info"), parents=True, exist_ok=True)
+    Path(tomte_dir, tomte_case_id, "pipeline_info", software_version_file).touch(exist_ok=True)
+    Path(tomte_dir, tomte_case_id, f"{tomte_case_id}_samplesheet.csv").touch(exist_ok=True)
+    Path.mkdir(
+        Path(tomte_dir, tomte_case_id, "multiqc", "multiqc_data"),
+        parents=True,
+        exist_ok=True,
+    )
+    write_json(
+        content=tomte_multiqc_json_metrics,
+        file_path=Path(
+            tomte_dir,
+            tomte_case_id,
+            "multiqc",
+            "multiqc_data",
+            "multiqc_data",
+        ).with_suffix(FileExtensions.JSON),
+    )
+    write_yaml(
+        content={tomte_case_id: [tower_id]},
+        file_path=Path(
+            tomte_dir,
+            tomte_case_id,
+            "tower_ids",
+        ).with_suffix(FileExtensions.YAML),
+    )
+
+
+@pytest.fixture(scope="function")
+def tomte_deliverables_file_path(tomte_dir, tomte_case_id) -> Path:
+    """Path to deliverables file."""
+    return Path(tomte_dir, tomte_case_id, f"{tomte_case_id}_deliverables").with_suffix(
+        FileExtensions.YAML
+    )
+
+
+@pytest.fixture(scope="function")
+def tomte_hermes_deliverables(tomte_deliverable_data: dict, tomte_case_id: str) -> dict:
+    hermes_output: dict = {"workflow": "tomte", "bundle_id": tomte_case_id, "files": []}
+    for file_info in tomte_deliverable_data["files"]:
+        tags: list[str] = []
+        if "html" in file_info["format"]:
+            tags.append("multiqc-html")
+        hermes_output["files"].append({"path": file_info["path"], "tags": tags, "mandatory": True})
+    return hermes_output
+
+
+@pytest.fixture(scope="function")
+def tomte_malformed_hermes_deliverables(tomte_hermes_deliverables: dict) -> dict:
+    malformed_deliverable: dict = tomte_hermes_deliverables.copy()
+    malformed_deliverable.pop("workflow")
+    return malformed_deliverable
+
+
+@pytest.fixture(scope="function")
+def tomte_deliverables_response_data(
+    create_multiqc_html_file,
+    create_multiqc_json_file,
+    tomte_case_id,
+    timestamp_yesterday,
+) -> InputBundle:
+    return InputBundle(
+        **{
+            "files": [
+                {
+                    "path": create_multiqc_json_file.as_posix(),
+                    "tags": ["multiqc-json", tomte_case_id],
+                },
+                {
+                    "path": create_multiqc_html_file.as_posix(),
+                    "tags": ["multiqc-html", tomte_case_id],
+                },
+            ],
+            "created": timestamp_yesterday,
+            "name": tomte_case_id,
+        }
     )
 
 
+@pytest.fixture(scope="function")
+def tomte_context(
+    cg_context: CGConfig,
+    helpers: StoreHelpers,
+    nf_analysis_housekeeper: HousekeeperAPI,
+    trailblazer_api: MockTB,
+    hermes_api: HermesApi,
+    cg_dir: Path,
+    tomte_case_id: str,
+    sample_id: str,
+    no_sample_case_id: str,
+    total_sequenced_reads_pass: int,
+    apptag_rna: str,
+    case_id_not_enough_reads: str,
+    sample_id_not_enough_reads: str,
+    total_sequenced_reads_not_pass: int,
+) -> CGConfig:
+    """Context to use in CLI."""
+    cg_context.housekeeper_api_ = nf_analysis_housekeeper
+    cg_context.trailblazer_api_ = trailblazer_api
+    cg_context.meta_apis["analysis_api"] = TomteAnalysisAPI(config=cg_context)
+    status_db: Store = cg_context.status_db
+
+    # Create ERROR case with NO SAMPLES
+    helpers.add_case(status_db, internal_id=no_sample_case_id, name=no_sample_case_id)
+
+    # Create a textbook case with enough reads
+    case_enough_reads: Case = helpers.add_case(
+        store=status_db,
+        internal_id=tomte_case_id,
+        name=tomte_case_id,
+        data_analysis=Workflow.TOMTE,
+    )
+
+    sample_enough_reads: Sample = helpers.add_sample(
+        status_db,
+        application_tag=apptag_rna,
+        internal_id=sample_id,
+        reads=total_sequenced_reads_pass,
+        last_sequenced_at=datetime.now(),
+    )
+
+    helpers.add_relationship(
+        status_db,
+        case=case_enough_reads,
+        sample=sample_enough_reads,
+    )
+
+    # Create a case without enough reads
+    case_not_enough_reads: Case = helpers.add_case(
+        store=status_db,
+        internal_id=case_id_not_enough_reads,
+        name=case_id_not_enough_reads,
+        data_analysis=Workflow.TOMTE,
+    )
+
+    sample_not_enough_reads: Sample = helpers.add_sample(
+        status_db,
+        application_tag=apptag_rna,
+        internal_id=sample_id_not_enough_reads,
+        reads=total_sequenced_reads_not_pass,
+        last_sequenced_at=datetime.now(),
+    )
+
+    helpers.add_relationship(status_db, case=case_not_enough_reads, sample=sample_not_enough_reads)
+
+    return cg_context
+
+
 # Taxprofiler fixtures
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture(scope="function")
 def taxprofiler_config(taxprofiler_dir: Path, taxprofiler_case_id: str) -> None:
     """Create CSV sample sheet file for testing."""
     Path.mkdir(Path(taxprofiler_dir, taxprofiler_case_id), parents=True, exist_ok=True)
     Path(taxprofiler_dir, taxprofiler_case_id, f"{taxprofiler_case_id}_samplesheet").with_suffix(
         FileExtensions.CSV
     ).touch(exist_ok=True)
 
@@ -2502,78 +3149,122 @@
 @pytest.fixture(scope="session")
 def taxprofiler_case_id() -> str:
     """Returns a taxprofiler case id."""
     return "taxprofiler_case"
 
 
 @pytest.fixture(scope="session")
+def taxprofiler_workflow() -> str:
+    """Returns taxprofiler workflow."""
+    return "taxprofiler"
+
+
+@pytest.fixture(scope="function")
 def taxprofiler_dir(tmpdir_factory, apps_dir: Path) -> Path:
     """Return the path to the Taxprofiler directory."""
     taxprofiler_dir = tmpdir_factory.mktemp("taxprofiler")
-    return Path(taxprofiler_dir).absolute()
+    return Path(taxprofiler_dir).absolute().as_posix()
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture(scope="function")
 def taxprofiler_sample_sheet_path(taxprofiler_dir, taxprofiler_case_id) -> Path:
     """Path to sample sheet."""
     return Path(
         taxprofiler_dir, taxprofiler_case_id, f"{taxprofiler_case_id}_samplesheet"
     ).with_suffix(FileExtensions.CSV)
 
 
-@pytest.fixture(scope="session")
-def taxprofiler_params_file_path(taxprofiler_dir, taxprofiler_case_id) -> Path:
-    """Path to parameters file."""
+@pytest.fixture(scope="function")
+def taxprofiler_nexflow_config_file_path(taxprofiler_dir, taxprofiler_case_id) -> Path:
+    """Path to config file."""
     return Path(
-        taxprofiler_dir, taxprofiler_case_id, f"{taxprofiler_case_id}_params_file"
-    ).with_suffix(FileExtensions.YAML)
+        taxprofiler_dir, taxprofiler_case_id, f"{taxprofiler_case_id}_nextflow_config"
+    ).with_suffix(FileExtensions.JSON)
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture(scope="function")
 def taxprofiler_sample_sheet_content(
     sample_name: str,
     sequencing_platform: str,
     fastq_forward_read_path: Path,
     fastq_reverse_read_path: Path,
 ) -> str:
     """Return the expected sample sheet content  for taxprofiler."""
-    return ",".join(
+    headers: str = ",".join(TaxprofilerSampleSheetEntry.headers())
+    row: str = ",".join(
         [
             sample_name,
             sample_name,
             sequencing_platform,
             fastq_forward_read_path.as_posix(),
             fastq_reverse_read_path.as_posix(),
             "",
         ]
     )
+    return "\n".join([headers, row])
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture(scope="function")
+def taxprofiler_params_file_path(taxprofiler_dir, taxprofiler_case_id) -> Path:
+    """Path to parameters file."""
+    return Path(
+        taxprofiler_dir, taxprofiler_case_id, f"{taxprofiler_case_id}_params_file"
+    ).with_suffix(FileExtensions.YAML)
+
+
+@pytest.fixture(scope="function")
+def taxprofiler_nexflow_config_file_path(taxprofiler_dir, taxprofiler_case_id) -> Path:
+    """Path to config file."""
+    return Path(
+        taxprofiler_dir, taxprofiler_case_id, f"{taxprofiler_case_id}_nextflow_config"
+    ).with_suffix(FileExtensions.JSON)
+
+
+@pytest.fixture(scope="function")
+def taxprofiler_hermes_deliverables(
+    taxprofiler_deliverable_data: dict, taxprofiler_case_id: str
+) -> dict:
+    hermes_output: dict = {"workflow": "taxprofiler", "bundle_id": taxprofiler_case_id, "files": []}
+    for file_info in taxprofiler_deliverable_data["files"]:
+        tags: list[str] = []
+        if "html" in file_info["format"]:
+            tags.append("multiqc-html")
+        hermes_output["files"].append({"path": file_info["path"], "tags": tags, "mandatory": True})
+    return hermes_output
+
+
+@pytest.fixture(scope="function")
+def taxprofiler_malformed_hermes_deliverables(taxprofiler_hermes_deliverables: dict) -> dict:
+    malformed_deliverable: dict = taxprofiler_hermes_deliverables.copy()
+    malformed_deliverable.pop("workflow")
+    return malformed_deliverable
+
+
+@pytest.fixture(scope="function")
 def taxprofiler_parameters_default(
     taxprofiler_dir: Path,
     taxprofiler_case_id: str,
     taxprofiler_sample_sheet_path: Path,
     existing_directory: Path,
 ) -> TaxprofilerParameters:
     """Return Taxprofiler parameters."""
     return TaxprofilerParameters(
         cluster_options="--qos=normal",
-        sample_sheet_path=taxprofiler_sample_sheet_path,
+        input=taxprofiler_sample_sheet_path,
         outdir=Path(taxprofiler_dir, taxprofiler_case_id),
         databases=existing_directory,
         hostremoval_reference=existing_directory,
         priority="development",
     )
 
 
 @pytest.fixture(scope="function")
 def taxprofiler_multiqc_json_metrics(taxprofiler_analysis_dir: Path) -> list[dict]:
     """Returns the content of a mock Multiqc JSON file."""
-    return read_json(file_path=Path(taxprofiler_analysis_dir, "multiqc_data.json"))
+    return read_json(file_path=Path(taxprofiler_analysis_dir, multiqc_json_file))
 
 
 @pytest.fixture(scope="function")
 def taxprofiler_metrics_deliverables(taxprofiler_analysis_dir: Path) -> dict:
     """Returns the content of a mock metrics deliverables file."""
     return read_yaml(
         file_path=Path(taxprofiler_analysis_dir, "taxprofiler_case_metrics_deliverables.yaml")
@@ -2593,81 +3284,80 @@
     """Path to deliverables file."""
     return Path(
         taxprofiler_dir, taxprofiler_case_id, f"{taxprofiler_case_id}_deliverables"
     ).with_suffix(FileExtensions.YAML)
 
 
 @pytest.fixture(scope="function")
-def nf_analysis_housekeeper(
-    housekeeper_api: HousekeeperAPI,
-    helpers: StoreHelpers,
-    mock_fastq_files: list[Path],
-    sample_id: str,
-    timestamp_now: datetime,
-):
-    """Create populated Housekeeper sample bundle mock."""
-
-    bundle_data: dict[str, Any] = {
-        "name": sample_id,
-        "created": timestamp_now,
-        "version": "1.0",
-        "files": [
-            {
-                "path": fastq_file_path.as_posix(),
-                "tags": [SequencingFileTag.FASTQ],
-                "archive": False,
-            }
-            for fastq_file_path in mock_fastq_files
-        ],
-    }
-    helpers.ensure_hk_bundle(store=housekeeper_api, bundle_data=bundle_data)
-    return housekeeper_api
-
-
-@pytest.fixture(scope="function")
 def taxprofiler_context(
     cg_context: CGConfig,
-    cg_dir: Path,
     helpers: StoreHelpers,
+    trailblazer_api: MockTB,
+    hermes_api: HermesApi,
+    nf_analysis_housekeeper: HousekeeperAPI,
+    cg_dir: Path,
     taxprofiler_case_id: str,
     sample_id: str,
     father_sample_id: str,
     sample_name: str,
     another_sample_name: str,
-    trailblazer_api: MockTB,
-    nf_analysis_housekeeper: HousekeeperAPI,
     no_sample_case_id: str,
     total_sequenced_reads_pass: int,
+    microbial_application_tag: str,
+    case_id_not_enough_reads: str,
+    sample_id_not_enough_reads: str,
+    total_sequenced_reads_not_pass: int,
 ) -> CGConfig:
     """Context to use in cli."""
     cg_context.housekeeper_api_ = nf_analysis_housekeeper
     cg_context.trailblazer_api_ = trailblazer_api
     cg_context.meta_apis["analysis_api"] = TaxprofilerAnalysisAPI(config=cg_context)
     status_db: Store = cg_context.status_db
 
-    # Create ERROR case with NO SAMPLES
+    # Create case with no associate samples
     helpers.add_case(status_db, internal_id=no_sample_case_id, name=no_sample_case_id)
 
+    # Create case without enough reads
+    case_not_enough_reads: Case = helpers.add_case(
+        store=status_db,
+        internal_id=case_id_not_enough_reads,
+        name=case_id_not_enough_reads,
+        data_analysis=Workflow.TAXPROFILER,
+    )
+
+    sample_not_enough_reads: Sample = helpers.add_sample(
+        status_db,
+        application_tag=microbial_application_tag,
+        internal_id=sample_id_not_enough_reads,
+        reads=total_sequenced_reads_not_pass,
+        last_sequenced_at=datetime.now(),
+    )
+
+    helpers.add_relationship(status_db, case=case_not_enough_reads, sample=sample_not_enough_reads)
+
+    # Create case with associated samples
     taxprofiler_case: Case = helpers.add_case(
         store=status_db,
         internal_id=taxprofiler_case_id,
         name=taxprofiler_case_id,
         data_analysis=Workflow.TAXPROFILER,
     )
 
     taxprofiler_sample: Sample = helpers.add_sample(
         status_db,
+        application_tag="multiqc",
         internal_id=sample_id,
         reads=total_sequenced_reads_pass,
         name=sample_name,
         last_sequenced_at=datetime.now(),
     )
 
     taxprofiler_another_sample: Sample = helpers.add_sample(
         status_db,
+        application_tag="multiqc",
         internal_id=father_sample_id,
         last_sequenced_at=datetime.now(),
         name=another_sample_name,
         reads=total_sequenced_reads_pass,
     )
 
     helpers.add_relationship(
@@ -2682,25 +3372,71 @@
         sample=taxprofiler_another_sample,
     )
 
     return cg_context
 
 
 @pytest.fixture(scope="function")
+def taxprofiler_deliverable_data(
+    taxprofiler_dir: Path, taxprofiler_case_id: str, sample_id: str
+) -> dict:
+    return {
+        "files": [
+            {
+                "path": f"{taxprofiler_dir}/{taxprofiler_case_id}/multiqc/multiqc_report.html",
+                "path_index": "",
+                "step": "report",
+                "tag": ["multiqc-html", "rna"],
+                "id": taxprofiler_case_id,
+                "format": "html",
+                "mandatory": True,
+            },
+        ]
+    }
+
+
+@pytest.fixture(scope="function")
+def taxprofiler_mock_deliverable_dir(
+    taxprofiler_dir: Path, taxprofiler_deliverable_data: dict, taxprofiler_case_id: str
+) -> Path:
+    """Create taxprofiler deliverable file with dummy data and files to deliver."""
+    Path.mkdir(
+        Path(taxprofiler_dir, taxprofiler_case_id),
+        parents=True,
+        exist_ok=True,
+    )
+    Path.mkdir(
+        Path(taxprofiler_dir, taxprofiler_case_id, "multiqc"),
+        parents=True,
+        exist_ok=True,
+    )
+    for report_entry in taxprofiler_deliverable_data["files"]:
+        Path(report_entry["path"]).touch(exist_ok=True)
+    WriteFile.write_file_from_content(
+        content=taxprofiler_deliverable_data,
+        file_format=FileFormat.JSON,
+        file_path=Path(
+            taxprofiler_dir, taxprofiler_case_id, taxprofiler_case_id + deliverables_yaml
+        ),
+    )
+    return taxprofiler_dir
+
+
+@pytest.fixture(scope="function")
 def taxprofiler_mock_analysis_finish(
     taxprofiler_dir: Path,
     taxprofiler_case_id: str,
     taxprofiler_multiqc_json_metrics: dict,
     tower_id: int,
 ) -> None:
-    """Create analysis finish file for testing."""
+    """Create analysis_finish file for testing."""
     Path.mkdir(
         Path(taxprofiler_dir, taxprofiler_case_id, "pipeline_info"), parents=True, exist_ok=True
     )
-    Path(taxprofiler_dir, taxprofiler_case_id, "pipeline_info", "software_versions.yml").touch(
+    Path(taxprofiler_dir, taxprofiler_case_id, "pipeline_info", software_version_file).touch(
         exist_ok=True
     )
     Path(taxprofiler_dir, taxprofiler_case_id, f"{taxprofiler_case_id}_samplesheet.csv").touch(
         exist_ok=True
     )
     Path.mkdir(
         Path(taxprofiler_dir, taxprofiler_case_id, "multiqc", "multiqc_data"),
@@ -2723,14 +3459,94 @@
             taxprofiler_dir,
             taxprofiler_case_id,
             "tower_ids",
         ).with_suffix(FileExtensions.YAML),
     )
 
 
+@pytest.fixture(scope="function")
+def taxprofiler_mock_config(taxprofiler_dir: Path, taxprofiler_case_id: str) -> None:
+    """Create CSV sample sheet file for testing."""
+    Path.mkdir(Path(taxprofiler_dir, taxprofiler_case_id), parents=True, exist_ok=True)
+    Path(taxprofiler_dir, taxprofiler_case_id, f"{taxprofiler_case_id}_samplesheet").with_suffix(
+        FileExtensions.CSV
+    ).touch(exist_ok=True)
+
+
+@pytest.fixture(scope="function")
+def taxprofiler_deliverable_data(
+    taxprofiler_dir: Path, taxprofiler_case_id: str, sample_id: str
+) -> dict:
+    return {
+        "files": [
+            {
+                "path": f"{taxprofiler_dir}/{taxprofiler_case_id}/multiqc/multiqc_report.html",
+                "path_index": "",
+                "step": "report",
+                "tag": ["multiqc-html"],
+                "id": taxprofiler_case_id,
+                "format": "html",
+                "mandatory": True,
+            },
+        ]
+    }
+
+
+@pytest.fixture(scope="function")
+def taxprofiler_deliverables_response_data(
+    create_multiqc_html_file,
+    create_multiqc_json_file,
+    taxprofiler_case_id,
+    timestamp_yesterday,
+) -> InputBundle:
+    return InputBundle(
+        **{
+            "files": [
+                {
+                    "path": create_multiqc_json_file.as_posix(),
+                    "tags": ["multiqc-json", taxprofiler_case_id],
+                },
+                {
+                    "path": create_multiqc_html_file.as_posix(),
+                    "tags": ["multiqc-html", taxprofiler_case_id],
+                },
+            ],
+            "created": timestamp_yesterday,
+            "name": taxprofiler_case_id,
+        }
+    )
+
+
+@pytest.fixture(scope="function")
+def nf_analysis_housekeeper(
+    housekeeper_api: HousekeeperAPI,
+    helpers: StoreHelpers,
+    mock_fastq_files: list[Path],
+    sample_id: str,
+    timestamp_now: datetime,
+) -> HousekeeperAPI:
+    """Create populated Housekeeper sample bundle mock."""
+
+    bundle_data: dict[str, Any] = {
+        "name": sample_id,
+        "created": timestamp_now,
+        "version": "1.0",
+        "files": [
+            {
+                "path": fastq_file_path.as_posix(),
+                "tags": [SequencingFileTag.FASTQ],
+                "archive": False,
+            }
+            for fastq_file_path in mock_fastq_files
+        ],
+    }
+    helpers.ensure_hk_bundle(store=housekeeper_api, bundle_data=bundle_data)
+    return housekeeper_api
+
+
 @pytest.fixture(scope="session")
 def expected_total_reads() -> int:
     return 1_000_000
 
 
 @pytest.fixture
 def flow_cell_name() -> str:
@@ -3039,36 +3855,32 @@
 ) -> DownsampleAPI:
     """Return a DownsampleAPI."""
     return DownsampleAPI(
         config=downsample_context,
     )
 
 
-@pytest.fixture(scope="session")
-def raredisease_case_id() -> str:
-    """Returns a raredisease case id."""
-    return "raredisease_case_enough_reads"
-
-
 @pytest.fixture(scope="function")
 def raredisease_context(
     cg_context: CGConfig,
     helpers: StoreHelpers,
     nf_analysis_housekeeper: HousekeeperAPI,
-    raredisease_case_id: str,
+    trailblazer_api: MockTB,
     sample_id: str,
     no_sample_case_id: str,
     total_sequenced_reads_pass: int,
     apptag_rna: str,
+    raredisease_case_id: str,
     case_id_not_enough_reads: str,
     sample_id_not_enough_reads: str,
     total_sequenced_reads_not_pass: int,
 ) -> CGConfig:
     """Raredisease context to use in CLI."""
     cg_context.housekeeper_api_ = nf_analysis_housekeeper
+    cg_context.trailblazer_api_ = trailblazer_api
     cg_context.meta_apis["analysis_api"] = RarediseaseAnalysisAPI(config=cg_context)
     status_db: Store = cg_context.status_db
 
     # Create ERROR case with NO SAMPLES
     helpers.add_case(status_db, internal_id=no_sample_case_id, name=no_sample_case_id)
 
     # Create a textbook case with enough reads
```

### Comparing `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py` & `cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,25 +114,14 @@
     """Create a flow cell object with flow cell that is demultiplexed."""
     return FlowCellDirectoryData(
         flow_cell_path=tmp_flow_cell_directory_bclconvert,
         bcl_converter=BclConverter.BCLCONVERT,
     )
 
 
-@pytest.fixture
-def unfinished_bcl2fastq_flow_cell(
-    demultiplexed_runs_unfinished_bcl2fastq_flow_cell_directory: Path,
-) -> FlowCellDirectoryData:
-    """Copy the content of a demultiplexed but not finished directory to a temporary location."""
-    return FlowCellDirectoryData(
-        flow_cell_path=demultiplexed_runs_unfinished_bcl2fastq_flow_cell_directory,
-        bcl_converter=BclConverter.BCL2FASTQ,
-    )
-
-
 # Flow cell attributes
 
 
 @pytest.fixture
 def bcl2fastq_flow_cell_id(
     novaseq_6000_pre_1_5_kits_flow_cell_bcl2fastq: FlowCellDirectoryData,
 ) -> str:
```

### Comparing `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py` & `cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py` & `cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,22 @@
     """Return the path to a working directory that will be deleted after test is run.
     This is a path to a flow cell directory with the run parameters present.
     """
     return Path(tmp_illumina_flow_cells_directory, bcl_convert_flow_cell_dir.name)
 
 
 @pytest.fixture
+def tmp_flow_cell_with_bcl2fastq_sample_sheet(
+    tmp_broken_flow_cells_directory: Path, hiseq_x_single_index_flow_cell_name: str
+) -> Path:
+    """This is a path to a flow cell directory with a bcl2fastq sample sheet."""
+    return Path(tmp_broken_flow_cells_directory, hiseq_x_single_index_flow_cell_name)
+
+
+@pytest.fixture
 def tmp_flow_cell_without_run_parameters_path(
     tmp_broken_flow_cells_directory: Path, hiseq_2500_custom_index_flow_cell_name: str
 ) -> Path:
     """This is a path to a flow cell directory with the run parameters missing."""
     return Path(tmp_broken_flow_cells_directory, hiseq_2500_custom_index_flow_cell_name)
```

### Comparing `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py` & `cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py` & `cg-60.0.0/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from datetime import datetime
 from pathlib import Path
+from typing import Any
 
 import pytest
 
 from cg.apps.demultiplex.sample_sheet.sample_sheet_models import SampleSheet
 from cg.apps.demultiplex.sample_sheet.sample_sheet_validator import SampleSheetValidator
 from cg.constants.constants import FileFormat
-from cg.constants.demultiplexing import BclConverter
 from cg.io.controller import ReadFile
 
 
 @pytest.fixture(scope="function")
 def sample_sheet_validator() -> SampleSheetValidator:
     """Return a sample sheet validator."""
     return SampleSheetValidator()
@@ -152,10 +153,35 @@
 @pytest.fixture
 def novaseq_6000_post_1_5_kits_sample_sheet_object(
     sample_sheet_validator: SampleSheetValidator,
     novaseq_6000_post_1_5_kits_correct_sample_sheet_path: Path,
 ) -> SampleSheet:
     """Return a NovaSeq 6000 sample sheet object."""
     return sample_sheet_validator.get_sample_sheet_object_from_file(
-        file_path=novaseq_6000_post_1_5_kits_correct_sample_sheet_path,
-        bcl_converter=BclConverter.BCLCONVERT,
+        file_path=novaseq_6000_post_1_5_kits_correct_sample_sheet_path
     )
+
+
+# HK bundle object
+
+
+@pytest.fixture
+def sample_sheet_bcl2fastq_bundle_data(
+    tmp_flow_cell_with_bcl2fastq_sample_sheet: Path,
+    timestamp_yesterday: datetime,
+) -> dict[str, Any]:
+    """Return a sample sheet bundle data dictionary."""
+    flow_cell_id: str = tmp_flow_cell_with_bcl2fastq_sample_sheet.name[-9:]
+    return {
+        "name": flow_cell_id,
+        "created": timestamp_yesterday,
+        "expires": timestamp_yesterday,
+        "files": [
+            {
+                "path": Path(
+                    tmp_flow_cell_with_bcl2fastq_sample_sheet, "SampleSheet.csv"
+                ).as_posix(),
+                "archive": False,
+                "tags": ["samplesheet", flow_cell_id],
+            },
+        ],
+    }
```

### Comparing `cg-59.9.1/tests/fixture_plugins/timestamp_fixtures.py` & `cg-60.0.0/tests/fixture_plugins/timestamp_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-60.0.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-60.0.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-60.0.0/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml` & `cg-60.0.0/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
   value: ''
 - condition: null
   header: null
   id: ADM1
   input: multiqc_data.json
   name: LIBRARY
   step: multiqc
-  value: Unknown Library
+  value: ''
 - condition: null
   header: null
   id: ADM1
   input: multiqc_data.json
   name: READ_GROUP
   step: multiqc
   value: ''
@@ -606,7 +606,49 @@
 - condition: null
   header: null
   id: ADM1
   input: multiqc_data.json
   name: pct_adapter
   step: multiqc
   value: 12.005654574904709
+- condition: null
+  header: null
+  id: ADM1
+  input: multiqc_data.json
+  name: percent_gc
+  step: multiqc
+  value: 51.0
+- condition: null
+  header: null
+  id: ADM1
+  input: multiqc_data.json
+  name: avg_sequence_length
+  step: multiqc
+  value: 98.42709962090532
+- condition: null
+  header: null
+  id: ADM1
+  input: multiqc_data.json
+  name: median_sequence_length
+  step: multiqc
+  value: 100
+- condition: null
+  header: null
+  id: ADM1
+  input: multiqc_data.json
+  name: total_sequences
+  step: multiqc
+  value: 74557102.0
+- condition: null
+  header: null
+  id: ADM1
+  input: multiqc_data.json
+  name: percent_duplicates
+  step: multiqc
+  value: 64.54554620264767
+- condition: null
+  header: null
+  id: ADM1
+  input: multiqc_data.json
+  name: percent_fails
+  step: multiqc
+  value: 18.181818181818183
```

### Comparing `cg-59.9.1/tests/fixtures/analysis/sample_coverage.bed` & `cg-60.0.0/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json` & `cg-60.0.0/tests/fixtures/analysis/taxprofiler/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml` & `cg-60.0.0/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/balsamic/case/config.json` & `cg-60.0.0/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-60.0.0/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-60.0.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-60.0.0/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv` & `cg-60.0.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-60.0.0/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/madeline/madeline.xml` & `cg-60.0.0/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-60.0.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-60.0.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/scout/643594.config.yaml` & `cg-60.0.0/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/scout/case_export.json` & `cg-60.0.0/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/scout/export_causatives.json` & `cg-60.0.0/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/scout/none_case_export.json` & `cg-60.0.0/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/scout/other_sex_case.json` & `cg-60.0.0/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/scout/panel_export.bed` & `cg-60.0.0/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/scout/panel_export.csv` & `cg-60.0.0/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv` & `cg-60.0.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-60.0.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.0.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/cgweb_orders/balsamic.json` & `cg-60.0.0/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/cgweb_orders/fastq.json` & `cg-60.0.0/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/cgweb_orders/metagenome.json` & `cg-60.0.0/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/cgweb_orders/microsalt.json` & `cg-60.0.0/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/cgweb_orders/mip.json` & `cg-60.0.0/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-60.0.0/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/cgweb_orders/rml.json` & `cg-60.0.0/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-60.0.0/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-60.0.0/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/data/SampleSheet.csv` & `cg-60.0.0/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/data/cgfixture.db` & `cg-60.0.0/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/data/hkstore.db` & `cg-60.0.0/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/io/example_json.json` & `cg-60.0.0/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1508.30.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1508.30.fastq.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1508.30.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1508.30.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1508.30.mip.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1508.30.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1508.30.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1508.30.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-60.0.0/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/NIPT-json.json` & `cg-60.0.0/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-60.0.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-60.0.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/report/case_data.json` & `cg-60.0.0/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/report/lims_exported_samples.json` & `cg-60.0.0/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/fixtures/report/lims_family.json` & `cg-60.0.0/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/io/conftest.py` & `cg-60.0.0/tests/io/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,20 +63,32 @@
 @pytest.fixture
 def txt_file_path(fixtures_dir: Path) -> Path:
     """Return a file path to example TXT file."""
     return Path(fixtures_dir, "io", "example.txt")
 
 
 @pytest.fixture
+def txt_file_path_2(fixtures_dir: Path) -> Path:
+    """Return a file path to example TXT file, 2 files needed to test concatenation."""
+    return Path(fixtures_dir, "io", "example2.txt")
+
+
+@pytest.fixture
 def tsv_stream() -> str:
     """Return string with TSV format."""
     return """Lorem	ipsum	sit	amet"""
 
 
 @pytest.fixture
+def config_dict() -> dict:
+    """Return dictionary format."""
+    return {"input": "input_path", "output": "output_path"}
+
+
+@pytest.fixture
 def txt_temp_path(cg_dir: Path) -> Path:
     """Return a temp file path to use when writing text files."""
     return Path(cg_dir, "write.txt")
 
 
 @pytest.fixture
 def csv_stream() -> str:
```

### Comparing `cg-59.9.1/tests/io/test_io_controller.py` & `cg-60.0.0/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/io/test_io_csv.py` & `cg-60.0.0/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/io/test_io_json.py` & `cg-60.0.0/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/io/test_io_txt.py` & `cg-60.0.0/tests/io/test_io_txt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 import pytest
 
-from cg.io.txt import read_txt, write_txt
+from cg.io.txt import concat_txt, read_txt, write_txt
 
 
 def test_read_txt_to_list(txt_file_path: Path):
     """
     Test reading content from a TXT file into a list.
     """
     # GIVEN a txt file
@@ -61,7 +61,34 @@
     write_txt(content=content, file_path=txt_temp_path)
 
     # THEN assert file exists
     assert txt_temp_path.exists()
 
     # THEN the content should match the original content
     assert content == read_txt(file_path=txt_temp_path)
+
+
+def test_concat_txt(txt_file_path: Path, txt_file_path_2: Path):
+    """Test concatenating two files, no optional string content"""
+    # GIVEN a list of file paths to concatenate
+
+    # WHEN concatenating two files
+    content: str = concat_txt(file_paths=[txt_file_path, txt_file_path_2], str_content=None)
+
+    # THEN the content of the files should have been concatenated
+    expected_content: str = "Line 1\nLine 2\nLine 3\nLine 4\nLine 5\nLine 6\n"
+    assert content == expected_content
+
+
+def test_concat_txt_with_string(txt_file_path: Path, txt_file_path_2: Path, csv_stream: str):
+    """Test concatenating two files, no optional string content"""
+    # GIVEN a list of file paths to concatenate
+
+    # WHEN concatenating two files
+    content: str = concat_txt(
+        file_paths=[txt_file_path, txt_file_path_2],
+        str_content=[csv_stream],
+    )
+
+    # THEN the content of the files should have been concatenated
+    expected_content: str = "Lorem,ipsum,sit,amet\nLine 1\nLine 2\nLine 3\nLine 4\nLine 5\nLine 6\n"
+    assert content == expected_content
```

### Comparing `cg-59.9.1/tests/io/test_io_xml.py` & `cg-60.0.0/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/io/test_io_yaml.py` & `cg-60.0.0/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/io/test_validate_path.py` & `cg-60.0.0/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/archive/conftest.py` & `cg-60.0.0/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/archive/test_archive_api.py` & `cg-60.0.0/tests/meta/archive/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/archive/test_archive_cli.py` & `cg-60.0.0/tests/meta/archive/test_archive_cli.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/archive/test_archiving.py` & `cg-60.0.0/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/backup/conftest.py` & `cg-60.0.0/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/backup/test_meta_backup.py` & `cg-60.0.0/tests/meta/backup/test_meta_backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -672,44 +672,42 @@
     novaseq_x_flow_cell: FlowCellDirectoryData,
 ):
     """Tests creating a copy complete file in the flow cell directory. There are two cases: when
     the file exists and when it does not exist."""
 
     # GIVEN a flow cell that has been decrypted in flow_cell directory
     flow_cell_dir: Path = novaseq_x_flow_cell.path
-    flow_cells: Path = flow_cell_dir.parent
 
     # GIVEN the copy complete to be created
     copy_complete_txt: str = DemultiplexingDirsAndFiles.COPY_COMPLETE
 
     # GIVEN a copy complete file exists
     flow_cell_dir.joinpath(copy_complete_txt).touch()
 
     # WHEN creating a copy complete file
-    backup_api.create_copy_complete(decrypted_flow_cell=flow_cell_dir, run_dir=flow_cells)
+    backup_api.create_copy_complete(flow_cell_dir)
 
     # THEN the copy complete file should exist in the flow cell directory
     assert flow_cell_dir.joinpath(copy_complete_txt).exists() is True
 
 
 def test_create_copy_complete_file_does_not_exist(
     backup_api: BackupAPI,
     novaseq_x_flow_cell: FlowCellDirectoryData,
 ):
     """Tests creating a copy complete file in the flow cell directory. There are two cases: when
     the file exists and when it does not exist."""
 
     # GIVEN a flow cell that has been decrypted in flow_cell directory
     flow_cell_dir: Path = novaseq_x_flow_cell.path
-    flow_cells: Path = flow_cell_dir.parent
 
     # GIVEN the copy complete to be created
     copy_complete_txt: str = DemultiplexingDirsAndFiles.COPY_COMPLETE
 
     # GIVEN that the copy complete file does not exists
     flow_cell_dir.joinpath(copy_complete_txt).unlink(missing_ok=True)
 
     # WHEN creating a copy complete file
-    backup_api.create_copy_complete(decrypted_flow_cell=flow_cell_dir, run_dir=flow_cells)
+    backup_api.create_copy_complete(flow_cell_dir)
 
     # THEN the copy complete file should exist in the flow cell directory
     assert flow_cell_dir.joinpath(copy_complete_txt).exists() is True
```

### Comparing `cg-59.9.1/tests/meta/backup/test_meta_pdc.py` & `cg-60.0.0/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/clean/conftest.py` & `cg-60.0.0/tests/meta/clean/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import SequencingFileTag
 from cg.constants.subject import Sex
 from cg.meta.clean.clean_flow_cells import CleanFlowCellAPI
 from cg.meta.clean.clean_retrieved_spring_files import CleanRetrievedSpringFilesAPI
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
-from cg.store.models import Flowcell, Sample
+from cg.store.models import Flowcell
 from cg.store.store import Store
 from tests.store_helpers import StoreHelpers
 
 
 @pytest.fixture(scope="function")
 def flow_cell_clean_api_can_be_removed(
     tmp_flow_cell_to_clean_path: Path,
@@ -92,21 +92,20 @@
         (sample_id, tmp_flow_cell_to_clean.id, 2, 50_000_0000, 90.4, 31),
     ]
     flow_cell: Flowcell = helpers.add_flow_cell(
         flow_cell_name=tmp_flow_cell_to_clean.id,
         store=store,
         has_backup=True,
     )
-    sample: Sample = helpers.add_sample(
+    helpers.add_sample(
         store=store, customer_id="cust500", internal_id=sample_id, name=sample_id, sex=Sex.MALE
     )
     helpers.add_multiple_sample_lane_sequencing_metrics_entries(
         metrics_data=sample_sequencing_metrics_details, store=store
     )
-    flow_cell.samples = [sample]
     store.session.add(flow_cell)
     store.session.commit()
     return store
 
 
 @pytest.fixture
 def store_with_flow_cell_not_to_clean(
@@ -121,21 +120,20 @@
         (sample_id, tmp_flow_cell_not_to_clean.id, 2, 50_000_0000, 90.4, 31),
     ]
     flow_cell: Flowcell = helpers.add_flow_cell(
         flow_cell_name=tmp_flow_cell_not_to_clean.id,
         store=store,
         has_backup=True,
     )
-    sample: Sample = helpers.add_sample(
+    helpers.add_sample(
         store=store, customer_id="cust500", internal_id=sample_id, name=sample_id, sex=Sex.MALE
     )
     helpers.add_multiple_sample_lane_sequencing_metrics_entries(
         metrics_data=sample_sequencing_metrics_details, store=store
     )
-    flow_cell.samples = [sample]
     store.session.add(flow_cell)
     store.session.commit()
     return store
 
 
 @pytest.fixture(scope="function")
 def housekeeper_api_with_flow_cell_to_clean(
```

### Comparing `cg-59.9.1/tests/meta/clean/test_clean_flow_cells_api.py` & `cg-60.0.0/tests/meta/clean/test_clean_flow_cells_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,17 +176,16 @@
 
     # GIVEN a store with a flow cell to be cleaned
     store: Store = flow_cell_clean_api_can_be_removed.status_db
     flow_cell: Flowcell = flow_cell_clean_api_can_be_removed.get_flow_cell_from_status_db()
 
     # GIVEN that the flow cell has two samples
     sample: Sample = helpers.add_sample(
-        store=store, customer_id="cust500", internal_id="123", name="123"
+        store=store, customer_id="cust500", internal_id="123", name="123", flowcell=flow_cell
     )
-    flow_cell.samples.append(sample)
     assert len(flow_cell.samples) == 2
     store.session.add(flow_cell)
     store.session.commit()
 
     # GIVEN that one of the samples is not in Housekeeper
     hk_api: HousekeeperAPI = flow_cell_clean_api_can_be_removed.hk_api
     assert not hk_api.bundle(sample.internal_id)
```

### Comparing `cg-59.9.1/tests/meta/clean/test_clean_retrieved_spring_files.py` & `cg-60.0.0/tests/meta/clean/test_clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/compress/conftest.py` & `cg-60.0.0/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/compress/test_clean_fastq.py` & `cg-60.0.0/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/compress/test_compress_files.py` & `cg-60.0.0/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/compress/test_compress_meta_fastq.py` & `cg-60.0.0/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/compress/test_decompress_spring_meta.py` & `cg-60.0.0/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-60.0.0/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/conftest.py` & `cg-60.0.0/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/deliver/conftest.py` & `cg-60.0.0/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/deliver/test_deliver_ticket.py` & `cg-60.0.0/tests/meta/rsync/test_rsync.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,244 +1,278 @@
-"""Tests for the deliver ticket command"""
+"""Tests for rsync API"""
 
 import logging
+import shutil
 from pathlib import Path
 
-from cg.constants.constants import Workflow
-from cg.constants.delivery import INBOX_NAME
-from cg.meta.deliver_ticket import DeliverTicketAPI
-from cg.models.cg_config import CGConfig
+import pytest
+
+from cg.constants.priority import SlurmAccount, SlurmQos
+from cg.exc import CgError
+from cg.meta.rsync import RsyncAPI
+from cg.store.models import Case
 from cg.store.store import Store
-from tests.store_helpers import StoreHelpers
+from tests.meta.deliver.conftest import all_samples_in_inbox, dummy_file_name
+from tests.store.conftest import case_obj
 
 
-def test_get_inbox_path(
-    cg_context: CGConfig, customer_id: str, helpers: StoreHelpers, mocker, ticket_id: str
+def test_get_source_and_destination_paths(
+    mutant_case: Case, rsync_api: RsyncAPI, ticket_id: str, mocker
 ):
-    """Test to get the path to customer inbox on the HPC."""
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
-
-    # GIVEN a case for analysis
-    case = helpers.add_case(
-        store=cg_context.status_db,
-        internal_id="angrybird",
-        name=ticket_id,
-        data_analysis=Workflow.MUTANT,
-    )
-
-    mocker.patch.object(DeliverTicketAPI, "get_all_cases_from_ticket")
-    DeliverTicketAPI.get_all_cases_from_ticket.return_value = [case]
-
-    # WHEN running get_inbox_path
-    inbox = deliver_ticket_api.get_inbox_path(ticket=ticket_id)
-
-    # THEN a path is returned for cust000 with the folder ticket in the inbox
-    assert inbox.parts[-3:] == (customer_id, INBOX_NAME, ticket_id)
+    """Test generating the source path before rsync."""
 
+    # GIVEN a valid Sars-cov-2 case
+    case = mutant_case
 
-def test_check_if_upload_is_needed(cg_context: CGConfig, mocker, ticket_id: str):
-    """Test if upload is needed when it is needed"""
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
-
-    # GIVEN the customer inbox
-    mocker.patch.object(DeliverTicketAPI, "get_inbox_path")
-    DeliverTicketAPI.get_inbox_path.return_value = Path(
-        "th155h0uLdC3R7aNlyNo7eX157f0RsuReaNdIfiTd03St3n0Mg"
+    # GIVEN file exists
+    mocker.patch.object(RsyncAPI, "get_all_cases_from_ticket")
+    RsyncAPI.get_all_cases_from_ticket.return_value = [case]
+
+    # WHEN the source path is created
+    source_and_destination_paths = rsync_api.get_source_and_destination_paths(
+        ticket=ticket_id, customer_internal_id=case.customer.internal_id
     )
 
-    # WHEN running check_if_upload_is_needed
-    is_upload_needed = deliver_ticket_api.check_if_upload_is_needed(ticket=ticket_id)
-
-    # THEN it turns out that upload is needed
-    assert is_upload_needed is True
-
-
-def test_check_if_upload_is_needed_part_deux(cg_context: CGConfig, mocker, ticket_id: str):
-    """Test if upload is needed when it is not needed"""
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
-
-    # GIVEN the customer inbox
-    mocker.patch.object(DeliverTicketAPI, "get_inbox_path")
-    DeliverTicketAPI.get_inbox_path.return_value = Path("/")
-
-    # WHEN running check_if_upload_is_needed
-    is_upload_needed = deliver_ticket_api.check_if_upload_is_needed(ticket=ticket_id)
-
-    # THEN it turns out that upload is not needed
-    assert is_upload_needed is False
-
+    # THEN the source path ends with a customer id, followed by "inbox" and a ticket_id id
+    assert (
+        source_and_destination_paths["delivery_source_path"]
+        .as_posix()
+        .endswith(f"/cust000/inbox/{ticket_id}")
+    )
+    # THEN the destination path is in the format server.name.se:/path/cust_id/path/ticket_id/
+    assert (
+        source_and_destination_paths["rsync_destination_path"].as_posix()
+        == "server.name.se:/some/cust000/inbox"
+    )
 
-def test_generate_date_tag(cg_context: CGConfig, mocker, helpers, ticket_id: str, timestamp_now):
-    """Test to generate the date tag."""
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
 
-    # GIVEN a case for analysis
-    case = helpers.add_case(
-        store=cg_context.status_db,
-        internal_id="angrybird",
-        name=ticket_id,
-        data_analysis=Workflow.MUTANT,
-    )
+def test_set_log_dir(rsync_api: RsyncAPI, ticket_id: str, caplog):
+    """Test function to set log dir for path."""
 
-    case.ordered_at = timestamp_now
+    caplog.set_level(logging.INFO)
 
-    mocker.patch.object(DeliverTicketAPI, "get_all_cases_from_ticket")
-    DeliverTicketAPI.get_all_cases_from_ticket.return_value = [case]
+    # GIVEN an RsyncAPI, with its base path as its log dir
+    base_path: Path = rsync_api.log_dir
 
-    # WHEN running generate_date_tag
-    date = deliver_ticket_api.generate_date_tag(ticket=ticket_id)
+    # WHEN setting the log directory
+    rsync_api.set_log_dir(folder_prefix=ticket_id)
 
-    # THEN check that a date was returned
-    assert str(timestamp_now) == str(date)
+    # THEN the log dir should set to a new path, different from the base path
+    assert base_path.as_posix() != rsync_api.log_dir.as_posix()
+    assert "Setting log dir to:" in caplog.text
 
 
-def test_sort_files(cg_context: CGConfig):
-    """Test to sort files"""
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
+def test_make_log_dir(rsync_api: RsyncAPI, ticket_id: str, caplog):
+    """Test generating the directory for logging."""
+    caplog.set_level(logging.INFO)
 
-    # GIVEN a list of paths
-    unsorted_list_of_paths = []
-    unsorted_list_of_paths.append(Path("2.fastq"))
-    unsorted_list_of_paths.append(Path("1.fastq"))
-    unsorted_list_of_paths.append(Path("3.fastq"))
+    # WHEN the log directory is created
+    rsync_api.set_log_dir(folder_prefix=ticket_id)
+    rsync_api.create_log_dir(dry_run=True)
 
-    # WHEN when sorting the paths
-    sorted_list_of_paths = deliver_ticket_api.sort_files(unsorted_list_of_paths)
+    # THEN the path is not created since it is a dry run
+    assert "Would have created path" in caplog.text
 
-    # THEN 1.fastq is first in the list
-    assert str(sorted_list_of_paths[0]) == "1.fastq"
+    # THEN the created path is
+    assert str(rsync_api.log_dir).startswith(f"/another/path/{ticket_id}")
 
 
-def test_check_if_concatenation_is_needed(
-    cg_context: CGConfig, mocker, helpers, analysis_store: Store, case_id, ticket_id: str
+def test_run_rsync_on_slurm(
+    microsalt_case: Case, rsync_api: RsyncAPI, ticket_id: str, caplog, mocker, helpers
 ):
-    """Test to check if concatenation is needed when it is not needed"""
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
-
-    # GIVEN a case object
-    case_obj = analysis_store.get_case_by_internal_id(internal_id=case_id)
+    """Test for running rsync using SLURM."""
+    caplog.set_level(logging.INFO)
 
-    mocker.patch.object(DeliverTicketAPI, "get_all_cases_from_ticket")
-    DeliverTicketAPI.get_all_cases_from_ticket.return_value = [case_obj]
+    # GIVEN a valid microsalt case
+    case: Case = microsalt_case
 
-    # GIVEN an application tag that is not a micro application
-    mocker.patch.object(DeliverTicketAPI, "get_app_tag")
-    DeliverTicketAPI.get_app_tag.return_value = "RMLP15S175"
+    # GIVEN paths needed to run rsync
+    mocker.patch.object(RsyncAPI, "get_source_and_destination_paths")
+    RsyncAPI.get_source_and_destination_paths.return_value = {
+        "delivery_source_path": Path("/path/to/source"),
+        "rsync_destination_path": Path("/path/to/destination"),
+    }
 
-    # WHEN running check_if_concatenation_is_needed
-    is_concatenation_needed = deliver_ticket_api.check_if_concatenation_is_needed(ticket=ticket_id)
+    mocker.patch.object(RsyncAPI, "get_all_cases_from_ticket")
+    RsyncAPI.get_all_cases_from_ticket.return_value = [case]
 
-    # THEN concatenation is not needed
-    assert is_concatenation_needed is False
+    # WHEN the destination path is created
+    sbatch_number: int = rsync_api.run_rsync_on_slurm(ticket=ticket_id, dry_run=True)
 
+    # THEN check that SARS-COV-2 analysis is not delivered
+    assert "Delivering report for SARS-COV-2 analysis" not in caplog.text
 
-def test_check_if_concatenation_is_needed_part_deux(
-    cg_context: CGConfig, mocker, helpers, analysis_store: Store, case_id, ticket_id: str
-):
-    """Test to check if concatenation is needed when it is needed"""
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
+    # THEN check that an integer was returned as sbatch number
+    assert isinstance(sbatch_number, int)
 
-    # GIVEN a case object
-    case_obj = analysis_store.get_case_by_internal_id(internal_id=case_id)
 
-    mocker.patch.object(DeliverTicketAPI, "get_all_cases_from_ticket")
-    DeliverTicketAPI.get_all_cases_from_ticket.return_value = [case_obj]
+def test_run_rsync_on_slurm_no_cases(rsync_api: RsyncAPI, ticket_id: str, caplog, mocker, helpers):
+    """Test for running rsync using SLURM when there are no cases on the ticket."""
+    caplog.set_level(logging.INFO)
 
-    # GIVEN an application tag that is a micro application
-    mocker.patch.object(DeliverTicketAPI, "get_app_tag")
-    DeliverTicketAPI.get_app_tag.return_value = "MWRNXTR003"
+    # GIVEN ticket without any cases
+    mocker.patch.object(RsyncAPI, "get_all_cases_from_ticket")
+    RsyncAPI.get_all_cases_from_ticket.return_value = None
 
-    # WHEN running check_if_concatenation_is_needed
-    is_concatenation_needed = deliver_ticket_api.check_if_concatenation_is_needed(ticket=ticket_id)
+    # WHEN the job is submitted
+    with pytest.raises(CgError):
+        rsync_api.run_rsync_on_slurm(ticket=ticket_id, dry_run=True)
 
-    # THEN concatenation is needed
-    assert is_concatenation_needed is True
+        # THEN check that error is raised based on no cases being present
+        assert "Could not find any cases for ticket" in caplog.text
 
 
-def test_get_samples_from_ticket(
-    cg_context: CGConfig, mocker, helpers, analysis_store: Store, case_id, ticket_id: str
+def test_get_folders_to_deliver(
+    analysis_family: dict, analysis_store_trio, rsync_api: RsyncAPI, case_id: str
 ):
-    """Test to get all samples from a ticket"""
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
+    """Tests the ability for the rsync api to get case and sample names."""
+    # GIVEN a case
 
-    # GIVEN a case object
-    case_obj = analysis_store.get_case_by_internal_id(internal_id=case_id)
+    # WHEN the function gets the folders
+    folder_list: list[str] = rsync_api.get_folders_to_deliver(
+        case_id=case_id, sample_files_present=True, case_files_present=True
+    )
 
-    mocker.patch.object(DeliverTicketAPI, "get_all_cases_from_ticket")
-    DeliverTicketAPI.get_all_cases_from_ticket.return_value = [case_obj]
+    # THEN it the list should contain the case name and all the samples
+    assert folder_list == [
+        analysis_family["samples"][0]["name"],
+        analysis_family["samples"][1]["name"],
+        analysis_family["samples"][2]["name"],
+        analysis_family["name"],
+    ]
 
-    # WHEN checking which samples there are in the ticket
-    all_samples: list = deliver_ticket_api.get_samples_from_ticket(ticket=ticket_id)
 
-    # THEN concatenation is needed
-    assert "child" in all_samples
-    assert "father" in all_samples
-    assert "mother" in all_samples
+def test_concatenate_rsync_commands(
+    analysis_family: dict, analysis_store_trio, project_dir, customer_id, ticket_id: str
+):
+    """Tests the function to concatenate rsync commands for transferring multiple files."""
+    # GIVEN a list with a case and a sample name
+    folder_list: list[str] = [analysis_family["name"], analysis_family["samples"][0]["name"]]
+    source_and_destination_paths = {
+        "delivery_source_path": project_dir / customer_id / ticket_id,
+        "rsync_destination_path": project_dir / customer_id,
+    }
+    # WHEN then commands are generated
+    commands: str = RsyncAPI.concatenate_rsync_commands(
+        folder_list=folder_list,
+        source_and_destination_paths=source_and_destination_paths,
+        ticket=ticket_id,
+    )
+    # THEN the correct folder should be added to the source path
+    assert (
+        " ".join(
+            [
+                str(source_and_destination_paths["delivery_source_path"] / analysis_family["name"]),
+                str(source_and_destination_paths["delivery_source_path"]),
+            ]
+        )
+        in commands
+    )
+    assert (
+        " ".join(
+            [
+                str(
+                    source_and_destination_paths["delivery_source_path"]
+                    / analysis_family["samples"][0]["name"]
+                ),
+                str(source_and_destination_paths["delivery_source_path"]),
+            ]
+        )
+        in commands
+    )
 
 
-def test_all_samples_in_cust_inbox(
-    cg_context: CGConfig, mocker, caplog, ticket_id: str, all_samples_in_inbox
+def test_slurm_rsync_single_case(
+    all_samples_in_inbox: Path,
+    case: Case,
+    destination_path: Path,
+    rsync_api: RsyncAPI,
+    caplog,
+    mocker,
+    ticket_id: str,
 ):
-    """Test that no samples will be reported as missing when all samples in inbox"""
+    """Test for running rsync on a single case using SLURM."""
     caplog.set_level(logging.INFO)
 
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
-
-    # GIVEN a path to the customer inbox
-    mocker.patch.object(DeliverTicketAPI, "get_inbox_path")
-    DeliverTicketAPI.get_inbox_path.return_value = all_samples_in_inbox
-
-    # GIVEN a ticket with certain samples
-    mocker.patch.object(DeliverTicketAPI, "get_samples_from_ticket")
-    DeliverTicketAPI.get_samples_from_ticket.return_value = ["ACC1", "ACC2"]
-
-    # WHEN checking if a sample is missing
-    deliver_ticket_api.report_missing_samples(ticket=ticket_id, dry_run=False)
+    # GIVEN paths needed to run rsync
+    mocker.patch.object(RsyncAPI, "get_source_and_destination_paths")
+    RsyncAPI.get_source_and_destination_paths.return_value = {
+        "delivery_source_path": all_samples_in_inbox,
+        "rsync_destination_path": destination_path,
+    }
+
+    mocker.patch.object(Store, "get_latest_ticket_from_case")
+    Store.get_latest_ticket_from_case.return_value = ticket_id
+
+    # WHEN the destination path is created
+    sbatch_number: int
+    is_complete_delivery: bool
+    is_complete_delivery, sbatch_number = rsync_api.slurm_rsync_single_case(
+        case=case,
+        case_files_present=True,
+        dry_run=True,
+        sample_files_present=True,
+    )
 
-    # THEN assert that all files were delivered
-    assert "Data has been delivered for all samples" in caplog.text
+    # THEN check that an integer was returned as sbatch number and the delivery should be complete
+    assert isinstance(sbatch_number, int)
+    assert is_complete_delivery
 
 
-def test_samples_missing_in_inbox(
-    analysis_family: dict,
-    cg_context: CGConfig,
-    mocker,
+def test_slurm_rsync_single_case_missing_file(
+    all_samples_in_inbox: Path,
+    case: Case,
+    destination_path: Path,
+    rsync_api: RsyncAPI,
     caplog,
+    mocker,
     ticket_id: str,
-    samples_missing_in_inbox,
 ):
-    """Test when samples is missing in customer inbox."""
+    """Test for running rsync on a single case with a missing file using SLURM."""
     caplog.set_level(logging.INFO)
 
-    # GIVEN a deliver_ticket API
-    deliver_ticket_api = DeliverTicketAPI(config=cg_context)
+    # GIVEN a valid mip case and sample folder missing
+    shutil.rmtree(Path(all_samples_in_inbox, case.links[0].sample.name))
 
-    # GIVEN a path to the customer inbox
-    mocker.patch.object(DeliverTicketAPI, "get_inbox_path")
-    DeliverTicketAPI.get_inbox_path.return_value = samples_missing_in_inbox
+    # GIVEN paths needed to run rsync
+    mocker.patch.object(RsyncAPI, "get_source_and_destination_paths")
+    RsyncAPI.get_source_and_destination_paths.return_value = {
+        "delivery_source_path": all_samples_in_inbox,
+        "rsync_destination_path": destination_path,
+    }
+
+    mocker.patch.object(Store, "get_latest_ticket_from_case")
+    Store.get_latest_ticket_from_case.return_value = ticket_id
+
+    # WHEN the destination path is created
+    sbatch_number: int
+    is_complete_delivery: bool
+    is_complete_delivery, sbatch_number = rsync_api.slurm_rsync_single_case(
+        case=case,
+        case_files_present=True,
+        dry_run=True,
+        sample_files_present=True,
+    )
 
-    # GIVEN a ticket with certain samples
-    mocker.patch.object(DeliverTicketAPI, "get_samples_from_ticket")
-    DeliverTicketAPI.get_samples_from_ticket.return_value = [
-        sample["name"] for sample in analysis_family["samples"]
-    ]
+    # THEN check that an integer was returned as sbatch number
+    assert isinstance(sbatch_number, int)
+    assert not is_complete_delivery
+
+
+def test_slurm_quality_of_service_production(rsync_api: RsyncAPI):
+    # GIVEN an RsyncAPI instance
+
+    # WHEN the account of the api is set to production
+    rsync_api.account = SlurmAccount.PRODUCTION
+
+    # THEN the quality of service should be set to HIGH
+    assert rsync_api.slurm_quality_of_service == SlurmQos.HIGH
 
-    # WHEN checking if a sample is missing
-    deliver_ticket_api.report_missing_samples(ticket=ticket_id, dry_run=False)
 
-    # THEN assert that a sample that is not missing is not missing
-    assert analysis_family["samples"][1]["name"] not in caplog.text
+def test_slurm_quality_of_service_other(rsync_api: RsyncAPI):
+    # GIVEN an RsyncAPI instance
 
-    # THEN assert that the empty case folder is not considered as a sample that is missing data
-    assert analysis_family["name"] not in caplog.text
+    # WHEN the account of the api is set to development
+    rsync_api.account = SlurmAccount.DEVELOPMENT
 
-    # THEN assert that a missing sample is logged as missing
-    assert analysis_family["samples"][0]["name"] in caplog.text
+    # THEN the quality of service should be set to LOW
+    assert rsync_api.slurm_quality_of_service == SlurmQos.LOW
```

### Comparing `cg-59.9.1/tests/meta/deliver/test_delivery_api.py` & `cg-60.0.0/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/demultiplex/conftest.py` & `cg-60.0.0/tests/meta/demultiplex/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants.demultiplexing import BclConverter, DemultiplexingDirsAndFiles
 from cg.meta.demultiplex.demux_post_processing import DemuxPostProcessingAPI
 from cg.meta.demultiplex.housekeeper_storage_functions import (
     add_and_include_sample_sheet_path_to_housekeeper,
 )
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 from cg.store.models import Case, Sample
 from cg.store.store import Store
 from tests.store_helpers import StoreHelpers
 
 FlowCellInfo = namedtuple("FlowCellInfo", "directory name sample_internal_ids")
 
 
@@ -234,40 +233,14 @@
 @pytest.fixture(scope="session")
 def flow_cell_name_demultiplexed_with_bcl_convert_on_sequencer() -> str:
     """Return the name of a flow cell directory that has been demultiplexed with Bcl Convert on the NovaseqX sequencer."""
     return "22522YLT3"
 
 
 @pytest.fixture(scope="session")
-def bcl2fastq_folder_structure(tmp_path_factory, cg_dir: Path) -> Path:
-    """Return a folder structure that resembles a bcl2fastq run folder."""
-    base_dir: Path = tmp_path_factory.mktemp("".join((str(cg_dir), BclConverter.BCL2FASTQ)))
-    folders: list[str] = ["l1t21", "l1t11", "l2t11", "l2t21"]
-
-    for folder in folders:
-        new_dir: Path = Path(base_dir, folder)
-        new_dir.mkdir()
-
-    return base_dir
-
-
-@pytest.fixture(scope="function")
-def not_bcl2fastq_folder_structure(tmp_path_factory, cg_dir: Path) -> Path:
-    """Return a folder structure that does not resemble a bcl2fastq run folder."""
-    base_dir: Path = tmp_path_factory.mktemp("".join((str(cg_dir), "not_bcl2fastq")))
-    folders: list[str] = ["just", "some", "folders"]
-
-    for folder in folders:
-        new_dir: Path = Path(base_dir, folder)
-        new_dir.mkdir()
-
-    return base_dir
-
-
-@pytest.fixture(scope="session")
 def base_call_file() -> Path:
     return Path("Data", "Intensities", "BaseCalls", "L001", "C1.1", "L001_1.cbcl")
 
 
 @pytest.fixture(scope="session")
 def inter_op_file() -> Path:
     return Path(DemultiplexingDirsAndFiles.INTER_OP, "AlignmentMetricsOut.bin")
@@ -325,16 +298,16 @@
         flow_cell_name="HHKVCALXX",
         hk_api=demux_post_processing_api.hk_api,
     )
     return flow_cell_dir_name
 
 
 @pytest.fixture
-def bcl2fastq_sample_id_with_non_pooled_undetermined_reads() -> str:
-    return "SVE2528A1"
+def bcl_convert_sample_id_with_non_pooled_undetermined_reads() -> str:
+    return "ACC11927A2"
 
 
 @pytest.fixture
 def bcl2fastq_non_pooled_sample_read_count() -> int:
     """Based on the data in 170407_ST-E00198_0209_BHHKVCALXX, the sum of all reads - mapped and undetermined."""
     return 8000000
```

### Comparing `cg-59.9.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py` & `cg-60.0.0/tests/meta/demultiplex/test_combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-60.0.0/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,31 +44,25 @@
     [
         DemultiplexingScenario(
             flow_cell_directory="flow_cell_directory_name_demultiplexed_with_bcl_convert",
             flow_cell_name="flow_cell_name_demultiplexed_with_bcl_convert",
             samples_ids="bcl_convert_demultiplexed_flow_cell_sample_internal_ids",
         ),
         DemultiplexingScenario(
-            flow_cell_directory="flow_cell_directory_name_demultiplexed_with_bcl2fastq",
-            flow_cell_name="flow_cell_name_demultiplexed_with_bcl2fastq",
-            samples_ids="bcl2fastq_demultiplexed_flow_cell_sample_internal_ids",
-            bcl_converter=BclConverter.BCL2FASTQ,
-        ),
-        DemultiplexingScenario(
             flow_cell_directory="flow_cell_directory_name_demultiplexed_with_bcl_convert_on_sequencer",
             flow_cell_name="flow_cell_name_demultiplexed_with_bcl_convert_on_sequencer",
             samples_ids="bcl_convert_demultiplexed_flow_cell_sample_internal_ids",
         ),
         DemultiplexingScenario(
             flow_cell_directory="flow_cell_directory_name_demultiplexed_with_bcl_convert_flat",
             flow_cell_name="flow_cell_name_demultiplexed_with_bcl_convert",
             samples_ids="bcl_convert_demultiplexed_flow_cell_sample_internal_ids",
         ),
     ],
-    ids=["BCLConvert tree", "BCL2FASTQ", "BCLConvert on sequencer", "BCLConvert flat"],
+    ids=["BCLConvert tree", "BCLConvert on sequencer", "BCLConvert flat"],
 )
 def test_post_processing_of_flow_cell(
     scenario: DemultiplexingScenario,
     demultiplex_context: CGConfig,
     request,
     tmp_illumina_demultiplexed_flow_cells_directory: Path,
 ):
@@ -102,14 +96,15 @@
         hk_api=demux_post_processing_api.hk_api,
     )
 
     # THEN the sample sheet is in housekeeper
     assert demux_post_processing_api.hk_api.get_files(
         bundle=flow_cell_name, tags=[SequencingFileTag.SAMPLE_SHEET]
     ).all()
+
     # WHEN post-processing the demultiplexed flow cell
     demux_post_processing_api.finish_flow_cell(
         flow_cell_directory_name=flow_cell_demultiplexing_directory,
         bcl_converter=scenario.bcl_converter,
     )
 
     # THEN a flow cell was created in statusdb
@@ -171,43 +166,14 @@
     # WHEN calling get_all_demultiplexed_flow_cell_dirs
     demultiplexed_flow_cell_dirs: list[Path] = demux_api.get_all_demultiplexed_flow_cell_dirs()
 
     # THEN the demultiplexed flow cells run directories should be returned
     assert tmp_demultiplexed_runs_bcl2fastq_directory in demultiplexed_flow_cell_dirs
 
 
-def test_post_processing_tracks_undetermined_fastqs_for_bcl2fastq(
-    demux_post_processing_api: DemuxPostProcessingAPI,
-    bcl2fastq_flow_cell_dir_name: str,
-    bcl2fastq_sample_id_with_non_pooled_undetermined_reads: str,
-    bcl2fastq_non_pooled_sample_read_count: int,
-):
-    # GIVEN a flow cell with undetermined fastqs in a non-pooled lane
-
-    # WHEN post processing the flow cell
-    demux_post_processing_api.finish_flow_cell(
-        flow_cell_directory_name=bcl2fastq_flow_cell_dir_name, bcl_converter=BclConverter.BCL2FASTQ
-    )
-
-    # THEN the undetermined fastqs were stored in housekeeper
-    fastq_files: list[File] = demux_post_processing_api.hk_api.get_files(
-        tags=[SequencingFileTag.FASTQ],
-        bundle=bcl2fastq_sample_id_with_non_pooled_undetermined_reads,
-    ).all()
-
-    undetermined_fastq_files = [file for file in fastq_files if "Undetermined" in file.path]
-    assert undetermined_fastq_files
-
-    # THEN the sample read count was updated with the undetermined reads
-    sample: Sample = demux_post_processing_api.status_db.get_sample_by_internal_id(
-        bcl2fastq_sample_id_with_non_pooled_undetermined_reads
-    )
-    assert sample.reads == bcl2fastq_non_pooled_sample_read_count
-
-
 def test_post_processing_tracks_undetermined_fastqs_for_bclconvert(
     demux_post_processing_api: DemuxPostProcessingAPI,
     bclconvert_flow_cell_dir_name: str,
     bcl_convert_sample_id_with_non_pooled_undetermined_reads: str,
     bcl_convert_non_pooled_sample_read_count: int,
 ):
     # GIVEN a flow cell with undetermined fastqs in a non-pooled lane
@@ -232,32 +198,35 @@
         bcl_convert_sample_id_with_non_pooled_undetermined_reads
     )
     assert sample.reads == bcl_convert_non_pooled_sample_read_count
 
 
 def test_sample_read_count_update_is_idempotent(
     demux_post_processing_api: DemuxPostProcessingAPI,
-    bcl2fastq_flow_cell_dir_name: str,
-    bcl2fastq_sample_id_with_non_pooled_undetermined_reads: str,
+    bclconvert_flow_cell_dir_name: str,
+    bcl_convert_sample_id_with_non_pooled_undetermined_reads: str,
 ):
     """Test that sample read counts are the same if the flow cell is processed twice."""
 
     # GIVEN a demultiplexed flow cell
 
     # WHEN post processing the flow cell twice
     demux_post_processing_api.finish_flow_cell(
-        flow_cell_directory_name=bcl2fastq_flow_cell_dir_name, bcl_converter=BclConverter.BCL2FASTQ
+        flow_cell_directory_name=bclconvert_flow_cell_dir_name,
+        bcl_converter=BclConverter.BCLCONVERT,
     )
     first_sample_read_count: int = demux_post_processing_api.status_db.get_sample_by_internal_id(
-        bcl2fastq_sample_id_with_non_pooled_undetermined_reads
+        bcl_convert_sample_id_with_non_pooled_undetermined_reads
     ).reads
 
-    demux_post_processing_api.finish_flow_cell(bcl2fastq_flow_cell_dir_name)
+    demux_post_processing_api.finish_flow_cell(
+        bclconvert_flow_cell_dir_name, bcl_converter=BclConverter.BCLCONVERT
+    )
     second_sample_read_count: int = demux_post_processing_api.status_db.get_sample_by_internal_id(
-        bcl2fastq_sample_id_with_non_pooled_undetermined_reads
+        bcl_convert_sample_id_with_non_pooled_undetermined_reads
     ).reads
 
     # THEN the sample read counts are not zero
     assert first_sample_read_count
 
     # THEN the sample read count is the same after the second post processing
     assert first_sample_read_count == second_sample_read_count
```

### Comparing `cg-59.9.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py` & `cg-60.0.0/tests/meta/demultiplex/test_housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/demultiplex/test_status_db_storage_functions.py` & `cg-60.0.0/tests/meta/demultiplex/test_status_db_storage_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Tests for the status_db_storage_functions module of the demultiplexing post post-processing module."""
 
 from mock import MagicMock
 
 from cg.meta.demultiplex.demux_post_processing import DemuxPostProcessingAPI
 from cg.meta.demultiplex.status_db_storage_functions import (
-    add_samples_to_flow_cell_in_status_db,
     add_sequencing_metrics_to_statusdb,
     delete_sequencing_metrics_from_statusdb,
     metric_has_sample_in_statusdb,
     update_sample_read_count,
 )
 from cg.models.cg_config import CGConfig
 from cg.store.models import Flowcell, Sample, SampleLaneSequencingMetrics
@@ -74,34 +73,14 @@
 
     # WHEN checking if the sample exists in statusdb
     assert not metric_has_sample_in_statusdb(
         sample_internal_id=sample_internal_id, store=demux_post_processing_api.status_db
     )
 
 
-def test_add_samples_to_flow_cell_in_status_db(
-    store_with_sequencing_metrics: Store, flow_cell_name: str, sample_id: str
-):
-    # GIVEN a store with sequencing metrics
-    store = store_with_sequencing_metrics
-
-    # GIVEN a flow cell
-    flow_cell = store_with_sequencing_metrics.get_flow_cell_by_name(flow_cell_name=flow_cell_name)
-
-    # WHEN adding samples to flow cell
-    add_samples_to_flow_cell_in_status_db(
-        flow_cell=flow_cell, sample_internal_ids=[sample_id], store=store
-    )
-
-    # THEN the samples are added to the flow cell in statusdb and FlowcellSamples are updated
-    flow_cell = store_with_sequencing_metrics.get_flow_cell_by_name(flow_cell_name=flow_cell_name)
-    assert flow_cell.samples
-    assert flow_cell.samples[0].internal_id == sample_id
-
-
 def test_delete_sequencing_metrics_from_statusdb_existing_metrics(
     store_with_sequencing_metrics: Store, flow_cell_name: str
 ):
     # GIVEN a store with sequencing metrics
     store = store_with_sequencing_metrics
 
     # GIVEN that the flow cell has sequencing metrics
```

### Comparing `cg-59.9.1/tests/meta/demultiplex/test_utils.py` & `cg-60.0.0/tests/meta/demultiplex/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/demultiplex/test_validation.py` & `cg-60.0.0/tests/meta/demultiplex/test_validation.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/encryption/conftest.py` & `cg-60.0.0/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/encryption/test_encryption.py` & `cg-60.0.0/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/observations/conftest.py` & `cg-60.0.0/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/observations/test_meta_upload_observations.py` & `cg-60.0.0/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/orders/conftest.py` & `cg-60.0.0/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-60.0.0/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-60.0.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-60.0.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-60.0.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/orders/test_meta_orders_api.py` & `cg-60.0.0/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/orders/test_meta_orders_lims.py` & `cg-60.0.0/tests/meta/orders/test_meta_orders_lims.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     # THEN it should have found the same number of samples
     assert len(samples) == 5
     # ... and pick out relevant UDFs
     first_sample = samples[0].dict()
     assert first_sample["udfs"]["collection_date"] == "2021-05-05"
     assert first_sample["udfs"]["extraction_method"] == "MagNaPure 96"
-    assert first_sample["udfs"]["lab_code"] == "SE110 Växjö"
+    assert first_sample["udfs"]["lab_code"] == "SE100 Karolinska"
     assert first_sample["udfs"]["organism"] == "SARS CoV-2"
     assert first_sample["udfs"]["original_lab"] == "Karolinska University Hospital Solna"
     assert first_sample["udfs"]["original_lab_address"] == "171 76 Stockholm"
     assert first_sample["udfs"]["pre_processing_method"] == "COVIDSeq"
     assert first_sample["udfs"]["priority"] == "research"
     assert first_sample["udfs"]["reference_genome"] == "NC_111"
     assert first_sample["udfs"]["region"] == "Stockholm"
```

### Comparing `cg-59.9.1/tests/meta/orders/test_meta_orders_status.py` & `cg-60.0.0/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/orders/test_rnafusion_submitter.py` & `cg-60.0.0/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/orders/test_ticket_handler.py` & `cg-60.0.0/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/qc_metrics/conftest.py` & `cg-60.0.0/tests/meta/qc_metrics/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 import pytest
 from housekeeper.store.models import File
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.clients.arnold.api import ArnoldAPIClient
+from cg.clients.arnold.dto.create_case_request import CreateCaseRequest
 from cg.clients.janus.api import JanusAPIClient
 from cg.clients.janus.dto.create_qc_metrics_request import (
     CreateQCMetricsRequest,
     FilePathAndTag,
     WorkflowInfo,
 )
 from cg.constants.housekeeper_tags import JanusTags
@@ -80,15 +81,15 @@
 @pytest.fixture
 def mock_janus_api() -> JanusAPIClient:
     return JanusAPIClient(config={"janus": {"host": ""}})
 
 
 @pytest.fixture
 def mock_arnold_api() -> ArnoldAPIClient:
-    return ArnoldAPIClient(config={"api_url": ""})
+    return ArnoldAPIClient(config={"arnold": {"api_url": ""}})
 
 
 @pytest.fixture(scope="function")
 def collect_qc_metrics_api(
     janus_store: Store,
     janus_hk_store: HousekeeperAPI,
     mock_janus_api: JanusAPIClient,
@@ -119,7 +120,22 @@
         case_id=case_id_with_single_sample,
         sample_ids=[sample.internal_id],
         workflow_info=WorkflowInfo(
             workflow=case.data_analysis, version=case.analyses[0].workflow_version
         ),
         files=[file_path_and_tag],
     )
+
+
+@pytest.fixture
+def mock_case_id() -> str:
+    return "mock_id"
+
+
+@pytest.fixture
+def mock_case_qc_metrics(mock_case_id: str) -> dict:
+    return {"case_id": mock_case_id, "case_info": {}}
+
+
+@pytest.fixture
+def expected_create_case_request(mock_case_qc_metrics: dict) -> CreateCaseRequest:
+    return CreateCaseRequest(**mock_case_qc_metrics)
```

### Comparing `cg-59.9.1/tests/meta/qc_metrics/test_collect_qc_metrics.py` & `cg-60.0.0/tests/meta/qc_metrics/test_collect_qc_metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for the collect qc metrics module."""
 
 from housekeeper.store.models import File
 
+from cg.clients.arnold.dto.create_case_request import CreateCaseRequest
 from cg.clients.janus.dto.create_qc_metrics_request import CreateQCMetricsRequest
 from cg.meta.qc_metrics.collect_qc_metrics import CollectQCMetricsAPI
 
 
 def test_get_qc_metrics_file_paths_for_case(
     case_id_with_single_sample: str,
     collect_qc_metrics_api: CollectQCMetricsAPI,
@@ -34,7 +35,28 @@
     # WHEN creating a qc metrics request for a case id
     qc_metrics_request: CreateQCMetricsRequest = collect_qc_metrics_api.create_qc_metrics_request(
         case_id_with_single_sample
     )
 
     # THEN a qc metrics request is created
     assert qc_metrics_request == expected_request
+
+
+def test_create_case_request(
+    collect_qc_metrics_api: CollectQCMetricsAPI,
+    mock_case_qc_metrics: dict,
+    mock_case_id: str,
+    expected_create_case_request: CreateCaseRequest,
+    mocker,
+):
+
+    # GIVEN a mock case qc metrics
+    mocker.patch.object(CollectQCMetricsAPI, "get_case_qc_metrics")
+    CollectQCMetricsAPI.get_case_qc_metrics.return_value = mock_case_qc_metrics
+
+    # WHEN creating a case request
+    create_case_request: CreateCaseRequest = collect_qc_metrics_api.get_create_case_request(
+        mock_case_id
+    )
+
+    # THEN a create case request is returned
+    assert create_case_request == expected_create_case_request
```

### Comparing `cg-59.9.1/tests/meta/report/conftest.py` & `cg-60.0.0/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/report/test_balsamic_api.py` & `cg-60.0.0/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/report/test_field_validators.py` & `cg-60.0.0/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/report/test_mip_dna_api.py` & `cg-60.0.0/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/report/test_report_api.py` & `cg-60.0.0/tests/meta/report/test_report_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,17 +417,17 @@
     mip_analysis_api: MipDNAAnalysisAPI,
     case_mip_dna: Case,
     caplog: LogCaptureFixture,
 ):
     """Test validation error if the analysis workflow is not supported by the delivery report workflow."""
 
     # GIVEN a pre-built case with Fluffy as data analysis
-    case_mip_dna.data_analysis = Workflow.FLUFFY
+    case_mip_dna.data_analysis = Workflow.MICROSALT
     mip_analysis: Analysis = case_mip_dna.analyses[0]
-    mip_analysis.workflow = Workflow.FLUFFY
+    mip_analysis.workflow = Workflow.MICROSALT
 
     # GIVEN a mip analysis mock metadata
     mip_metadata: MipAnalysis = mip_analysis_api.get_latest_metadata(case_mip_dna.internal_id)
 
     # WHEN retrieving data analysis information
 
     # THEN a validation error should be raised
```

### Comparing `cg-59.9.1/tests/meta/report/test_rnafusion_api.py` & `cg-60.0.0/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/rsync/conftest.py` & `cg-60.0.0/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/test_invoice.py` & `cg-60.0.0/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/transfer/test_external_data.py` & `cg-60.0.0/tests/meta/transfer/test_external_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,17 +167,14 @@
 
     mocker.patch.object(Path, "iterdir")
     Path.iterdir.return_value = []
 
     mocker.patch.object(ExternalDataAPI, "get_available_samples")
     ExternalDataAPI.get_available_samples.return_value = samples[:-1]
 
-    mocker.patch.object(Store, "cases")
-    Store.cases.return_value = [{"internal_id": "yellowhog"}]
-
     mocker.patch.object(Store, "set_case_action")
     Store.set_case_action.return_value = None
 
     # THEN none of the samples should exist in housekeeper
     assert all(
         external_data_api.housekeeper_api.bundle(sample.internal_id) is None for sample in samples
     )
```

### Comparing `cg-59.9.1/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-60.0.0/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/balsamic/test_balsamic.py` & `cg-60.0.0/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/conftest.py` & `cg-60.0.0/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-60.0.0/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/mutacc/conftest.py` & `cg-60.0.0/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-60.0.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/nipt/conftest.py` & `cg-60.0.0/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/nipt/test_models.py` & `cg-60.0.0/tests/meta/upload/nipt/test_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-60.0.0/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/scout/conftest.py` & `cg-60.0.0/tests/meta/upload/scout/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,20 +92,14 @@
 @pytest.fixture
 def dna_sample_father_id() -> str:
     """Return a father DNA sample id."""
     return "dna_father"
 
 
 @pytest.fixture
-def another_sample_id() -> str:
-    """Return another sample id."""
-    return "another_sample_id"
-
-
-@pytest.fixture
 def another_rna_sample_id() -> str:
     """Return another RNA sample id."""
     return "another_rna_sample_id"
 
 
 @pytest.fixture
 def rna_store(
```

### Comparing `cg-59.9.1/tests/meta/upload/scout/test_generate_load_config.py` & `cg-60.0.0/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-60.0.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-60.0.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-60.0.0/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/test_meta_upload_coverage.py` & `cg-60.0.0/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/test_upload_api.py` & `cg-60.0.0/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/upload/test_upload_genotypes_api.py` & `cg-60.0.0/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/workflow/conftest.py` & `cg-60.0.0/tests/meta/workflow/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from tests.cli.workflow.balsamic.conftest import (
     balsamic_housekeeper_dir,
     fastq_file_l_1_r_1,
     fastq_file_l_2_r_1,
     fastq_file_l_2_r_2,
 )
 from tests.meta.compress.conftest import compress_api, real_crunchy_api
-from tests.meta.upload.scout.conftest import another_sample_id
 from tests.mocks.tb_mock import MockTB
 from tests.store_helpers import StoreHelpers
 
 
 @pytest.fixture(scope="function")
 def populated_compress_spring_api(
     compress_api: CompressAPI, only_spring_bundle: dict, helpers
```

### Comparing `cg-59.9.1/tests/meta/workflow/microsalt/conftest.py` & `cg-60.0.0/tests/meta/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/workflow/microsalt/test_quality_controller.py` & `cg-60.0.0/tests/meta/workflow/microsalt/test_quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py` & `cg-60.0.0/tests/meta/workflow/microsalt/test_quality_controller_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/workflow/microsalt/test_report_generation.py` & `cg-60.0.0/tests/meta/workflow/microsalt/test_report_generation.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/workflow/test_analysis.py` & `cg-60.0.0/tests/meta/workflow/test_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 
     # GIVEN a case
     case: Case = analysis_store.get_cases()[0]
 
     # GIVEN that no samples are down-sampled nor external
     for sample in case.samples:
         assert not sample.from_sample
-        assert not sample.is_external
 
     # WHEN checking if a flow cell check is applicable
     # THEN the method should return True
     assert mip_analysis_api._is_flow_cell_check_applicable(case_id=case.internal_id)
 
 
 def test_is_flow_cell_check_not_applicable_when_external(
```

### Comparing `cg-59.9.1/tests/meta/workflow/test_balsamic.py` & `cg-60.0.0/tests/meta/workflow/test_balsamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tests for BALSAMIC analysis."""
 
 from pathlib import Path
 
 import pytest
 
+from cg.constants.constants import AnalysisType
 from cg.constants.observations import ObservationsFileWildcards
 from cg.constants.sequencing import Variants
 from cg.constants.subject import Sex
 from cg.exc import BalsamicStartError
 from cg.meta.workflow.balsamic import BalsamicAnalysisAPI
 from cg.models.cg_config import CGConfig
```

### Comparing `cg-59.9.1/tests/meta/workflow/test_fastq.py` & `cg-60.0.0/tests/meta/workflow/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/workflow/test_microsalt.py` & `cg-60.0.0/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/workflow/test_nf_analysis.py` & `cg-60.0.0/tests/meta/workflow/test_nf_analysis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,72 @@
 """Module for nf-core analysis API tests."""
 
 import logging
 from typing import Any
 
 import pytest
+from _pytest.fixtures import FixtureRequest
 from _pytest.logging import LogCaptureFixture
-from pathlib import Path
 
+from cg.constants import Workflow
 from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.cg_config import CGConfig
 from tests.cli.workflow.conftest import deliverables_template_content
 
 
 @pytest.mark.parametrize(
-    ("context", "metrics_deliverables", "case_id", "analysis_finish"),
-    [
-        (
-            "rnafusion_context",
-            "rnafusion_metrics_deliverables",
-            "rnafusion_case_id",
-            "rnafusion_mock_analysis_finish",
-        ),
-        (
-            "taxprofiler_context",
-            "taxprofiler_metrics_deliverables",
-            "taxprofiler_case_id",
-            "taxprofiler_mock_analysis_finish",
-        ),
-    ],
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
 )
 def test_create_metrics_deliverables_content(
-    context: str,
-    case_id: str,
-    metrics_deliverables: str,
+    workflow: Workflow,
     caplog: LogCaptureFixture,
-    analysis_finish,
-    request,
+    request: FixtureRequest,
 ):
     """Test metrics deliverables file content function for Taxprofiler and Rnafusion."""
-
     caplog.set_level(logging.INFO)
 
     # GIVEN each fixture is being initialised
-    context: CGConfig = request.getfixturevalue(context)
-    metrics_deliverables: dict = request.getfixturevalue(metrics_deliverables)
-    case_id: str = request.getfixturevalue(case_id)
-    request.getfixturevalue(analysis_finish)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
+
+    metrics_deliverables: dict = request.getfixturevalue(f"{workflow}_metrics_deliverables")
+    case_id: str = request.getfixturevalue(f"{workflow}_case_id")
+    request.getfixturevalue(f"{workflow}_mock_analysis_finish")
 
     # GIVEN a Nextflow workflow analysis API and a list of QC metrics
     analysis_api: NfAnalysisAPI = context.meta_apis["analysis_api"]
 
     # WHEN writing the metrics deliverables file
     metrics_deliverables_content: dict[str, list[dict[str, Any]]] = (
         analysis_api.create_metrics_deliverables_content(case_id)
     )
 
     # THEN assert that the content created is correct
     assert metrics_deliverables_content == metrics_deliverables
 
 
 @pytest.mark.parametrize(
-    ("context", "case_id"),
-    [
-        (
-            "rnafusion_context",
-            "rnafusion_case_id",
-        ),
-        (
-            "taxprofiler_context",
-            "taxprofiler_case_id",
-        ),
-    ],
+    "workflow",
+    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
 )
 def test_get_formatted_file_deliverable(
-    context: str,
-    case_id: str,
+    workflow: Workflow,
     sample_id: str,
     sample_name: str,
     caplog: LogCaptureFixture,
     deliverables_template_content,
-    request,
+    request: FixtureRequest,
 ):
     """Test the formatted file deliverable with the case and sample attributes for Taxprofiler and Rnafusion."""
 
     caplog.set_level(logging.INFO)
 
     # GIVEN each fixture is being initialised
-    context: CGConfig = request.getfixturevalue(context)
-    case_id: str = request.getfixturevalue(case_id)
+    context: CGConfig = request.getfixturevalue(f"{workflow}_context")
+    case_id: str = request.getfixturevalue(f"{workflow}_case_id")
 
     caplog.set_level(logging.INFO)
     analysis_api: NfAnalysisAPI = context.meta_apis["analysis_api"]
 
     # WHEN formatting the template
     for field in deliverables_template_content:
         formatted_file_deliverable = analysis_api.get_formatted_file_deliverable(
```

### Comparing `cg-59.9.1/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-60.0.0/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/meta/workflow/test_rnafusion.py` & `cg-60.0.0/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/balsamic_analysis_mock.py` & `cg-60.0.0/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/crunchy.py` & `cg-60.0.0/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/hk_mock.py` & `cg-60.0.0/tests/mocks/hk_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,20 @@
         """Find a file in the latest version of a bundle."""
         version: Version = self.last_version(bundle=bundle_name)
         if not version:
             LOG.info(f"Bundle: {bundle_name} not found in Housekeeper")
             raise HousekeeperBundleVersionMissingError
         return self.files(version=version.id, tags=tags).first()
 
-    def get_files_from_latest_version(self, bundle_name: str, tags: list[str]) -> list[File] | None:
+    def get_files_from_latest_version_containing_tags(self, **_kwargs) -> list[File]:
+        return self._files.all()
+
+    def get_files_from_latest_version(
+        self, bundle_name: str, tags: list[str] | None = None
+    ) -> list[File] | None:
         """Return files in the latest version of a bundle."""
         version: Version = self.last_version(bundle=bundle_name)
         if not version:
             LOG.info(f"Bundle: {bundle_name} not found in Housekeeper")
             raise HousekeeperBundleVersionMissingError
         return self.files(version=version.id, tags=tags)
 
@@ -583,13 +588,16 @@
         """Drop all tables in the store"""
 
     @contextmanager
     def session_no_autoflush(self):
         """Wrap property in Housekeeper Store"""
         yield True
 
+    def rollback(self) -> None:
+        return None
+
     def __repr__(self):
         return f"HousekeeperMockAPI:version_obj={self._version_obj}"
 
 
 if __name__ == "__main__":
     hk_api = MockHousekeeperAPI(config={})
```

### Comparing `cg-59.9.1/tests/mocks/limsmock.py` & `cg-60.0.0/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/madeline.py` & `cg-60.0.0/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/mip_analysis_mock.py` & `cg-60.0.0/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/osticket.py` & `cg-60.0.0/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/process_mock.py` & `cg-60.0.0/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/report.py` & `cg-60.0.0/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/scout.py` & `cg-60.0.0/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/store_model.py` & `cg-60.0.0/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/mocks/tb_mock.py` & `cg-60.0.0/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/balsamic/conftest.py` & `cg-60.0.0/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/balsamic/test_balsamic_analysis.py` & `cg-60.0.0/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/conftest.py` & `cg-60.0.0/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/demultiplexing/test_run_parameters.py` & `cg-60.0.0/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/downsample/test_down_sample_meta_data.py` & `cg-60.0.0/tests/models/downsample/test_down_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/flow_cell/test_flowcell_model.py` & `cg-60.0.0/tests/models/flow_cell/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/mip/conftest.py` & `cg-60.0.0/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/mip/test_mip_analysis.py` & `cg-60.0.0/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/mip/test_mip_config.py` & `cg-60.0.0/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-60.0.0/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/mip/test_mip_sample_info.py` & `cg-60.0.0/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/nextflow/test_nextflow_deliver.py` & `cg-60.0.0/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/observations/conftest.py` & `cg-60.0.0/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/observations/test_observations_input_files.py` & `cg-60.0.0/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/report/test_validators.py` & `cg-60.0.0/tests/models/report/test_validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 import pytest
 from _pytest.logging import LogCaptureFixture
 from pydantic import ValidationInfo
 
 from cg.constants import NA_FIELD, NO_FIELD, REPORT_GENDER, YES_FIELD, Workflow
 from cg.constants.constants import AnalysisType
 from cg.constants.subject import Sex
+from cg.models.delivery.delivery import DeliveryFile
 from cg.models.orders.constants import OrderType
 from cg.models.report.validators import (
     get_analysis_type_as_string,
     get_boolean_as_string,
     get_date_as_string,
+    get_delivered_files_as_file_names,
     get_float_as_percentage,
     get_float_as_string,
     get_gender_as_string,
     get_list_as_string,
     get_path_as_string,
     get_prep_category_as_string,
     get_report_string,
@@ -134,14 +136,29 @@
     # WHEN performing the validation
     validated_list: str = get_list_as_string(mock_list)
 
     # THEN check if the input values were formatted correctly
     assert validated_list == "I am, a, list"
 
 
+def test_get_list_paths_as_strings(filled_file: Path):
+    """Test file path name extraction from a list."""
+
+    # GIVEN a list of delivery files
+    path_list: list[DeliveryFile] = [
+        DeliveryFile(source_path=filled_file, destination_path=filled_file)
+    ]
+
+    # WHEN validating the provided list of delivery paths
+    path_name_list: list[str] = get_delivered_files_as_file_names(path_list)
+
+    # THEN the returned list should contain the file names
+    assert path_name_list.pop() == "a_file.txt"
+
+
 def test_get_path_as_string(filled_file: Path):
     """Test file path name extraction."""
 
     # GIVEN a mock path
 
     # WHEN performing the validation
     path_name: str = get_path_as_string(filled_file)
```

### Comparing `cg-59.9.1/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-60.0.0/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/test_cg_models.py` & `cg-60.0.0/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/test_compression_data.py` & `cg-60.0.0/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/test_fastq.py` & `cg-60.0.0/tests/models/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/models/test_file_data.py` & `cg-60.0.0/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/server/endpoints/test_orders_endpoint.py` & `cg-60.0.0/tests/server/endpoints/test_orders_endpoint.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 
 import mock.mock
 import pytest
 from flask.testing import FlaskClient
 
 from cg.apps.tb import TrailblazerAPI
 from cg.apps.tb.dto.summary_response import AnalysisSummary
-from cg.constants import Workflow
-from cg.services.orders.order_service.utils import create_order_response
-from cg.services.orders.order_status_service.dto.order_status_summary import (
-    OrderSummary,
-)
-from cg.services.orders.order_status_service.utils import create_summaries
+from cg.constants.constants import Workflow
 from cg.store.models import Order
 
 
 @pytest.mark.parametrize(
     "limit, workflow, expected_orders",
     [
         (None, Workflow.MIP_DNA, 2),
@@ -30,52 +25,71 @@
     client: FlaskClient,
     order: Order,
     order_another: Order,
     order_balsamic: Order,
     limit: int | None,
     workflow: str,
     expected_orders: int,
-    analysis_summary,
 ):
     """Tests that orders are returned from the orders endpoint"""
     # GIVEN a store with three orders, two of which are MIP-DNA and the last is BALSAMIC
 
     # WHEN a request is made to get all orders
     endpoint: str = "/api/v1/orders"
-    with mock.patch.object(TrailblazerAPI, "get_summaries", return_value=[]):
+    with mock.patch.object(
+        TrailblazerAPI,
+        "get_summaries",
+        return_value=[
+            AnalysisSummary(
+                order_id=order.id, cancelled=0, completed=1, delivered=0, failed=0, running=0
+            ),
+            AnalysisSummary(
+                order_id=order_another.id,
+                cancelled=0,
+                completed=1,
+                delivered=0,
+                failed=0,
+                running=0,
+            ),
+            AnalysisSummary(
+                order_id=order_balsamic.id,
+                cancelled=0,
+                completed=1,
+                delivered=0,
+                failed=0,
+                running=0,
+            ),
+        ],
+    ):
         response = client.get(endpoint, query_string={"pageSize": limit, "workflow": workflow})
 
     # THEN the response should be successful
     assert response.status_code == HTTPStatus.OK
 
     # THEN the response contains the correct number of orders
     assert len(response.json["orders"]) == expected_orders
 
 
 def test_order_endpoint(
     client: FlaskClient, order: Order, order_another: Order, analysis_summary: AnalysisSummary
 ):
     """Tests that the order endpoint returns the order with matching id"""
     # GIVEN a store with two orders
-
     order_id_to_fetch: int = order.id
 
     # WHEN a request is made to get a specific order
     endpoint: str = f"/api/v1/orders/{order_id_to_fetch}"
     with mock.patch.object(TrailblazerAPI, "get_summaries", return_value=[analysis_summary]):
         response = client.get(endpoint)
 
     # THEN the response should be successful
     assert response.status_code == HTTPStatus.OK
 
-    order_summary: OrderSummary = create_summaries(
-        orders=[order], analysis_summaries=[analysis_summary]
-    )[0]
-    # THEN the response should only contain the specified order
-    assert response.json == create_order_response(order=order, summary=order_summary).model_dump()
+    # THEN the response contains the specified order
+    assert response.json["id"] == order_id_to_fetch
 
 
 def test_order_endpoint_not_found(
     client: FlaskClient, order: Order, order_another: Order, non_existent_order_id: int
 ):
     """Tests that the order endpoint returns the order with matching id"""
     # GIVEN a store with two orders
```

### Comparing `cg-59.9.1/tests/services/fastq_file_service/conftest.py` & `cg-60.0.0/tests/services/fastq_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/services/fastq_file_service/test_fastq_file_service.py` & `cg-60.0.0/tests/services/fastq_file_service/test_fastq_file_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,102 @@
 from pathlib import Path
-
 from cg.services.fastq_file_service.fastq_file_service import FastqFileService
 
 
 def test_empty_directory(fastq_file_service: FastqFileService, tmp_path):
     # GIVEN an empty directory
 
     # GIVEN output files
-    forward_output = Path(tmp_path, "forward.fastq.gz")
-    reverse_output = Path(tmp_path, "reverse.fastq.gz")
+    forward_output_path = Path(tmp_path, "forward.fastq.gz")
+    reverse_output_path = Path(tmp_path, "reverse.fastq.gz")
 
     # WHEN concatenating the reads
     fastq_file_service.concatenate(
         fastq_directory=tmp_path,
-        forward_output=forward_output,
-        reverse_output=reverse_output,
+        forward_output_path=forward_output_path,
+        reverse_output_path=reverse_output_path,
     )
 
     # THEN the output files should not exist
-    assert not forward_output.exists()
-    assert not reverse_output.exists()
+    assert not forward_output_path.exists()
+    assert not reverse_output_path.exists()
 
 
 def test_concatenate(fastq_file_service: FastqFileService, fastqs_dir: Path):
     # GIVEN a directory with forward and reverse reads
 
     # GIVEN output files for the concatenated reads
-    forward_output = Path(fastqs_dir, "forward.fastq.gz")
-    reverse_output = Path(fastqs_dir, "reverse.fastq.gz")
+    forward_output_path = Path(fastqs_dir, "forward.fastq.gz")
+    reverse_output_path = Path(fastqs_dir, "reverse.fastq.gz")
 
     # WHEN concatenating the reads
     fastq_file_service.concatenate(
         fastq_directory=fastqs_dir,
-        forward_output=forward_output,
-        reverse_output=reverse_output,
+        forward_output_path=forward_output_path,
+        reverse_output_path=reverse_output_path,
         remove_raw=True,
     )
 
     # THEN the output files should exist
-    assert forward_output.exists()
-    assert reverse_output.exists()
+    assert forward_output_path.exists()
+    assert reverse_output_path.exists()
 
     # THEN the concatenated forward reads only contain forward reads
-    assert "forward" in forward_output.read_text()
-    assert "reverse" not in forward_output.read_text()
+    assert "forward" in forward_output_path.read_text()
+    assert "reverse" not in forward_output_path.read_text()
 
     # THEN the concatenated reverse reads only contain reverse reads
-    assert "reverse" in reverse_output.read_text()
-    assert "forward" not in reverse_output.read_text()
+    assert "reverse" in reverse_output_path.read_text()
+    assert "forward" not in reverse_output_path.read_text()
 
 
 def test_concatenate_when_output_exists(fastq_file_service: FastqFileService, fastqs_dir: Path):
     # GIVEN a directory with forward and reverse reads
     existing_fastq_files = list(fastqs_dir.iterdir())
     existing_forward: Path = existing_fastq_files[0]
 
     # GIVEN that the forward output file already exists
-    forward_output = existing_forward
-    reverse_output = Path(fastqs_dir, "reverse.fastq.gz")
+    forward_output_path = existing_forward
+    reverse_output_path = Path(fastqs_dir, "reverse.fastq.gz")
 
     # WHEN concatenating the reads
     fastq_file_service.concatenate(
         fastq_directory=fastqs_dir,
-        forward_output=forward_output,
-        reverse_output=reverse_output,
+        forward_output_path=forward_output_path,
+        reverse_output_path=reverse_output_path,
         remove_raw=True,
     )
 
     # THEN the output files should exist
-    assert forward_output.exists()
-    assert reverse_output.exists()
+    assert forward_output_path.exists()
+    assert reverse_output_path.exists()
 
     # THEN the concatenated forward reads only contain forward reads
-    assert "forward" in forward_output.read_text()
-    assert "reverse" not in forward_output.read_text()
+    assert "forward" in forward_output_path.read_text()
+    assert "reverse" not in forward_output_path.read_text()
 
     # THEN the concatenated reverse reads only contain reverse reads
-    assert "reverse" in reverse_output.read_text()
-    assert "forward" not in reverse_output.read_text()
+    assert "reverse" in reverse_output_path.read_text()
+    assert "forward" not in reverse_output_path.read_text()
 
 
 def test_concatenate_missing_reverse(
     fastq_file_service: FastqFileService, fastqs_forward: Path, tmp_path
 ):
     # GIVEN a directory with forward reads only
 
     # GIVEN output files for the concatenated reads
-    forward_output = Path(tmp_path, "forward.fastq.gz")
-    reverse_output = Path(tmp_path, "reverse.fastq.gz")
+    forward_output_path = Path(tmp_path, "forward.fastq.gz")
+    reverse_output_path = Path(tmp_path, "reverse.fastq.gz")
 
     # WHEN concatenating the reads
     fastq_file_service.concatenate(
         fastq_directory=fastqs_forward,
-        forward_output=forward_output,
-        reverse_output=reverse_output,
+        forward_output_path=forward_output_path,
+        reverse_output_path=reverse_output_path,
     )
 
     # THEN forward reads should be concatenated
-    assert forward_output.exists()
+    assert forward_output_path.exists()
 
     # THEN reverse reads should not exist
-    assert not reverse_output.exists()
+    assert not reverse_output_path.exists()
```

### Comparing `cg-59.9.1/tests/store/api/conftest.py` & `cg-60.0.0/tests/store/api/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         store=store,
         flow_cell_name=bcl2fastq_flow_cell_id,
         samples=[store_sample],
         date=timestamp_now,
     )
 
     helpers.add_relationship(store=store, case=store_case, sample=store_sample)
-    helpers.add_sample_lane_sequencing_metrics(
+    helpers.ensure_sample_lane_sequencing_metrics(
         store=store,
         sample_internal_id=store_sample.internal_id,
         flow_cell_name=bcl2fastq_flow_cell_id,
         flow_cell_lane_number=1,
         sample_total_reads_in_lane=5,
         sample_base_percentage_passing_q30=30,
     )
```

### Comparing `cg-59.9.1/tests/store/api/test_base.py` & `cg-60.0.0/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/conftest.py` & `cg-60.0.0/tests/store/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,20 +215,18 @@
         is_tumour=True,
         internal_id=StoreConstants.INTERNAL_ID_SAMPLE_WITH_ATTRIBUTES.value,
         reads=StoreConstants.READS_SAMPLE_WITH_ATTRIBUTES.value,
         name=StoreConstants.NAME_SAMPLE_WITH_ATTRIBUTES.value,
         original_ticket=StoreConstants.ORIGINAL_TICKET_SAMPLE_WITH_ATTRIBUTES.value,
         ordered_at=timestamp_now,
         created_at=timestamp_now,
-        sequence_start=timestamp_now,
         delivered_at=timestamp_now,
         received_at=timestamp_now,
         last_sequenced_at=timestamp_now,
         prepared_at=timestamp_now,
-        invoiced_at=timestamp_now,
         application_version_id=StoreConstants.APPLICATION_VERSION_ID_SAMPLE_WITH_ATTRIBUTES.value,
         subject_id=StoreConstants.SUBJECT_ID_SAMPLE_WITH_ATTRIBUTES.value,
         invoice_id=StoreConstants.INVOICE_ID_SAMPLE_WITH_ATTRIBUTES.value,
         organism_id=StoreConstants.ORGANISM_ID_SAMPLE_WITH_ATTRIBUTES.value,
         loqusdb_id=StoreConstants.LOCUSDB_ID_SAMPLE_WITH_ATTRIBUTES.value,
         downsampled_to=StoreConstants.DOWN_SAMPLED_TO_SAMPLE_WITH_ATTRIBUTES.value,
         no_invoice=False,
@@ -286,19 +284,18 @@
         no_invoice=True,
         name=StoreConstants.NAME_POOL_WITHOUT_ATTRIBUTES.value,
     )
 
     return store
 
 
-@pytest.fixture(name="store_with_an_application_with_and_without_attributes")
+@pytest.fixture
 def store_with_an_application_with_and_without_attributes(
     store: Store,
     helpers: StoreHelpers,
-    timestamp_now=dt.datetime.now(),
 ) -> Store:
     """Return a store with an application with and without attributes."""
     helpers.ensure_application(
         store=store,
         tag=StoreConstants.TAG_APPLICATION_WITH_ATTRIBUTES.value,
         prep_category=StoreConstants.PREP_CATEGORY_APPLICATION_WITH_ATTRIBUTES.value,
         is_external=True,
@@ -312,15 +309,15 @@
         is_external=False,
         is_archived=False,
     )
 
     return store
 
 
-@pytest.fixture(name="store_with_application_limitations")
+@pytest.fixture
 def store_with_application_limitations(
     store_with_an_application_with_and_without_attributes: Store, helpers: StoreHelpers
 ) -> Store:
     """Return a store with different application limitations."""
     helpers.ensure_application_limitation(
         store=store_with_an_application_with_and_without_attributes,
         application=store_with_an_application_with_and_without_attributes.get_application_by_tag(
```

### Comparing `cg-59.9.1/tests/store/crud/add/test_store_add_application_version.py` & `cg-60.0.0/tests/store/crud/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/add/test_store_add_base.py` & `cg-60.0.0/tests/store/crud/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/add/test_store_add_customer.py` & `cg-60.0.0/tests/store/crud/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/add/test_store_add_flow_celll.py` & `cg-60.0.0/tests/store/crud/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/conftest.py` & `cg-60.0.0/tests/store/crud/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         store=re_sequenced_sample_store,
         flow_cell_name=bcl2fastq_flow_cell_id,
         samples=[store_sample],
         date=one_day_ahead_of_now,
     )
 
     helpers.add_relationship(store=re_sequenced_sample_store, case=store_case, sample=store_sample)
-    helpers.add_sample_lane_sequencing_metrics(
+    helpers.ensure_sample_lane_sequencing_metrics(
         store=re_sequenced_sample_store,
         sample_internal_id=store_sample.internal_id,
         flow_cell_name=bcl2fastq_flow_cell_id,
         flow_cell_lane_number=1,
         sample_total_reads_in_lane=120000000,
         sample_base_percentage_passing_q30=90,
     )
```

### Comparing `cg-59.9.1/tests/store/crud/delete/test_delete.py` & `cg-60.0.0/tests/store/crud/delete/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/read/test_read.py` & `cg-60.0.0/tests/store/crud/read/test_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -934,15 +934,15 @@
         )
     )
 
     # THEN assert that the application limitation was found
     assert (
         application_limitation
         and application_limitation.application.tag == tag
-        and application_limitation.pipeline == workflow
+        and application_limitation.workflow == workflow
     )
 
 
 def test_get_case_samples_by_case_id(
     store_with_analyses_for_cases: Store,
     case_id: str,
 ):
```

### Comparing `cg-59.9.1/tests/store/crud/read/test_read_analyses_to_clean.py` & `cg-60.0.0/tests/store/crud/read/test_read_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py` & `cg-60.0.0/tests/store/crud/read/test_read_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/read/test_read_analysis.py` & `cg-60.0.0/tests/store/crud/read/test_read_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/read/test_read_application_version.py` & `cg-60.0.0/tests/store/crud/read/test_read_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/read/test_read_customer.py` & `cg-60.0.0/tests/store/crud/read/test_read_customer.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/read/test_read_pool.py` & `cg-60.0.0/tests/store/crud/read/test_read_pool.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/read/test_read_sample.py` & `cg-60.0.0/tests/store/crud/read/test_read_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/crud/update/test_update.py` & `cg-60.0.0/tests/store/crud/update/test_update.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_analyses_filters.py` & `cg-60.0.0/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_application_filters.py` & `cg-60.0.0/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_application_limitations_filters.py` & `cg-60.0.0/tests/store/filters/test_status_application_limitations_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,9 +51,9 @@
     # ASSERT that application limitations is a query
     assert isinstance(application_limitations, Query)
 
     # THEN assert the application limitations was found
     assert (
         application_limitations.all()
         and len(application_limitations.all()) == 1
-        and application_limitations.all()[0].pipeline == workflow
+        and application_limitations.all()[0].workflow == workflow
     )
```

### Comparing `cg-59.9.1/tests/store/filters/test_status_application_version_filters.py` & `cg-60.0.0/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_bed_filters.py` & `cg-60.0.0/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_bed_version_filters.py` & `cg-60.0.0/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_case_sample_filters.py` & `cg-60.0.0/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_cases_filters.py` & `cg-60.0.0/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_collaboration_filters.py` & `cg-60.0.0/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_customer_filters.py` & `cg-60.0.0/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_flow_cell_filters.py` & `cg-60.0.0/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_invoice_filters.py` & `cg-60.0.0/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_metrics_filters.py` & `cg-60.0.0/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_organism_filters.py` & `cg-60.0.0/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_panel_filters.py` & `cg-60.0.0/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_pool_filters.py` & `cg-60.0.0/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/filters/test_status_samples_filters.py` & `cg-60.0.0/tests/store/filters/test_status_samples_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -627,29 +627,27 @@
         "customer_id": sample.customer_id,
         "delivered_at": sample.delivered_at,
         "downsampled_to": sample.downsampled_to,
         "from_sample": sample.from_sample,
         "id": sample.id,
         "internal_id": sample.internal_id,
         "invoice_id": sample.invoice_id,
-        "invoiced_at": sample.invoiced_at,
         "is_tumour": sample.is_tumour,
         "loqusdb_id": sample.loqusdb_id,
         "name": sample.name,
         "no_invoice": sample.no_invoice,
         "order": sample.order,
         "ordered_at": sample.ordered_at,
         "organism_id": sample.organism_id,
         "original_ticket": sample.original_ticket,
         "prepared_at": sample.prepared_at,
         "priority": sample.priority,
         "reads": sample.reads,
         "received_at": sample.received_at,
         "reference_genome": sample.reference_genome,
-        "sequence_start": sample.sequence_start,
         "sex": sample.sex,
         "last_sequenced_at": sample.last_sequenced_at,
         "subject_id": sample.subject_id,
     }
     for key, value in identifiers.items():
         filtered_sample_query: Query = filter_samples_by_identifier_name_and_value(
             samples=sample_query,
```

### Comparing `cg-59.9.1/tests/store/filters/test_status_user_filters.py` & `cg-60.0.0/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/test_delivery.py` & `cg-60.0.0/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store/test_store_models.py` & `cg-60.0.0/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/store_helpers.py` & `cg-60.0.0/tests/store_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,15 +241,15 @@
     def ensure_application_limitation(
         store: Store,
         application: Application,
         workflow: str = Workflow.MIP_DNA,
         limitations: str = "Dummy limitations",
         **kwargs,
     ) -> ApplicationLimitations:
-        """Ensure that application limitations exists in store."""
+        """Ensure that application limitations exist in store."""
         application_limitation: ApplicationLimitations = (
             store.get_application_limitation_by_tag_and_workflow(
                 tag=application.tag, workflow=workflow
             )
         )
         if application_limitation:
             return application_limitation
@@ -397,15 +397,22 @@
 
         sample.application_version_id = application_version_id
         sample.customer = customer
         sample.ordered_at = datetime.now()
 
         for key, value in kwargs.items():
             if key == "flowcell":
-                sample.flowcells.append(kwargs["flowcell"])
+                flow_cell: Flowcell = kwargs["flowcell"]
+                metric: SampleLaneSequencingMetrics = store.add_sample_lane_sequencing_metrics(
+                    sample_internal_id=sample.internal_id,
+                    flow_cell_name=flow_cell.name,
+                    **kwargs,
+                )
+                store.session.add(metric)
+
             elif hasattr(sample, key):
                 setattr(sample, key, value)
             else:
                 raise AttributeError(f"Unknown sample attribute/feature: {key}, {value}")
 
         store.session.add(sample)
         store.session.commit()
@@ -517,15 +524,15 @@
                 data_delivery=data_delivery,
                 name=case_name,
                 internal_id=case_id,
                 action=action,
             )
             case.customer = customer
         if order:
-            order.cases = [case]
+            store.link_case_to_order(order_id=order.id, case_id=case.id)
         return case
 
     @staticmethod
     def ensure_case_from_dict(
         store: Store,
         case_info: dict,
         app_tag: str = None,
@@ -681,21 +688,28 @@
             flow_cell_name=flow_cell_name,
             sequencer_name="dummy_sequencer",
             sequencer_type=sequencer_type,
             date=date,
             has_backup=has_backup,
         )
         flow_cell.archived_at = archived_at
-        if samples:
-            flow_cell.samples = samples
         if status:
             flow_cell.status = status
 
         store.session.add(flow_cell)
         store.session.commit()
+
+        if samples:
+            for sample in samples:
+                StoreHelpers.ensure_sample_lane_sequencing_metrics(
+                    sample_internal_id=sample.internal_id,
+                    flow_cell_name=flow_cell.name,
+                    store=store,
+                )
+        store.session.commit()
         return flow_cell
 
     @staticmethod
     def add_relationship(
         store: Store,
         sample: Sample,
         case: Case,
@@ -911,20 +925,24 @@
 
         case = cls.add_case(store=base_store, internal_id=case_id, name=case_id)
         sample = cls.add_sample(store=base_store, internal_id=sample_id)
         cls.add_relationship(store=base_store, sample=sample, case=case)
         return case
 
     @classmethod
-    def add_sample_lane_sequencing_metrics(
+    def ensure_sample_lane_sequencing_metrics(
         cls,
         store: Store,
         sample_internal_id: str,
         flow_cell_name: str,
         customer_id: str = "some_customer_007",
+        sample_total_reads_in_lane: int = 500_000_000,
+        sample_base_percentage_passing_q30: int = 90,
+        sample_base_mean_quality_score: int = 35,
+        created_at: datetime = datetime.now(),
         **kwargs,
     ):
         """Helper function to add a sample lane sequencing metrics associated with a sample with the given ids."""
         sample: Sample = store.get_sample_by_internal_id(internal_id=sample_internal_id)
         flow_cell: Flowcell = store.get_flow_cell_by_name(flow_cell_name=flow_cell_name)
 
         if not sample:
@@ -933,14 +951,18 @@
             )
         if not flow_cell:
             flow_cell = cls.add_flow_cell(store=store, flow_cell_name=flow_cell_name)
 
         metrics: SampleLaneSequencingMetrics = store.add_sample_lane_sequencing_metrics(
             sample_internal_id=sample.internal_id,
             flow_cell_name=flow_cell.name,
+            sample_total_reads_in_lane=sample_total_reads_in_lane,
+            sample_base_percentage_passing_q30=sample_base_percentage_passing_q30,
+            sample_base_mean_quality_score=sample_base_mean_quality_score,
+            created_at=created_at,
             **kwargs,
         )
         metrics.sample = sample
         metrics.flowcell = flow_cell
         store.session.add(metrics)
         store.session.commit()
         return metrics
@@ -953,15 +975,15 @@
             sample_internal_id,
             flow_cell_name_,
             flow_cell_lane_number,
             sample_total_reads_in_lane,
             sample_base_percentage_passing_q30,
             sample_base_mean_quality_score,
         ) in metrics_data:
-            cls.add_sample_lane_sequencing_metrics(
+            cls.ensure_sample_lane_sequencing_metrics(
                 store=store,
                 sample_internal_id=sample_internal_id,
                 flow_cell_name=flow_cell_name_,
                 flow_cell_lane_number=flow_cell_lane_number,
                 sample_total_reads_in_lane=sample_total_reads_in_lane,
                 sample_base_percentage_passing_q30=sample_base_percentage_passing_q30,
                 sample_base_mean_quality_score=sample_base_mean_quality_score,
```

### Comparing `cg-59.9.1/tests/test_copy_novaseqx_flow_cell.py` & `cg-60.0.0/tests/test_copy_novaseqx_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/test_store_helpers.py` & `cg-60.0.0/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/utils/conftest.py` & `cg-60.0.0/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/utils/test_commands.py` & `cg-60.0.0/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/utils/test_date.py` & `cg-60.0.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/utils/test_dict.py` & `cg-60.0.0/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/utils/test_dispatcher.py` & `cg-60.0.0/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/utils/test_files.py` & `cg-60.0.0/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/utils/test_time.py` & `cg-60.0.0/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/tests/utils/test_utils.py` & `cg-60.0.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.1/PKG-INFO` & `cg-60.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 59.9.1
+Version: 60.0.0
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -26,14 +26,15 @@
 Requires-Dist: SQLAlchemy
 Requires-Dist: WTForms
 Requires-Dist: alembic
 Requires-Dist: blinker
 Requires-Dist: cachetools
 Requires-Dist: click
 Requires-Dist: coloredlogs
+Requires-Dist: cryptography
 Requires-Dist: genologics
 Requires-Dist: google-auth
 Requires-Dist: gunicorn
 Requires-Dist: housekeeper (>=4.11.3)
 Requires-Dist: lxml
 Requires-Dist: marshmallow
 Requires-Dist: openpyxl
```

