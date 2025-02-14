Changelog
==========

<!--
Newest changes should be on top.

This document is user facing. Please word the changes in such a way
that users understand how the changes affect the new version.
-->

version 1.1.0
---------------------------
+ Update multiqc to version 1.10.
+ Update CutAdapt to version 3.4.
+ Update biowdl-input-converter to version 0.3.
+ Add the dockerImages to the output section.
+ Replace travis with github CI.
+ Update CutAdapt to version 3.0.0.
+ Remove metrics file from classification (which causes the
  summary report to be empty).
  https://github.com/DaehwanKimLab/centrifuge/issues/83
+ Adapt the pipeline so it can also handle fasta files.

version 1.0.0
---------------------------
+ Update tasks and the input/output names.
+ Rename workflow outputs to shorter names.
+ Add `meta {allowNestedInputs: true}` to the workflows, to allow for the use
  of nested inputs.
+ Remove `execute` from the naming structure for calls of tasks and workflows.
+ Add centrifuge kreport to the pipeline.
+ Make the multiqc task suitable for use with a `final_workflow_outputs_dir`
  so it can be used on all of cromwell's supported backends.
+ Tasks were updated to contain the `time_minutes` runtime attribute and
  associated `timeMinutes` input, describing the maximum time the task will
  take to run.
+ Renamed workflow from `pipeline` to `Classification`.
+ Removed jenkinsfile from repo.
+ Update documentation with more specific example of sample sheet csv file.
+ Update cutadapt to 2.8.
+ Update multiqc to 1.8.
+ Update fastqc to 0.11.9.
+ Remove unused docker image.
+ Add cromwell test config.
+ Add krona plot.
+ Setup the centrifuge pipeline.
