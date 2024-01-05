# Getting started

To connect to Open OnDemand, visit [https://ondemand.cluster.france-bioinformatique.fr](https://ondemand.cluster.france-bioinformatique.fr)

The first page of IFB Open OnDemand will bring you to a login prompt. Use your IFB cluster account to login.

![Login](https://raw.githubusercontent.com/lkhamvongsa/OpenOnDemandDoc/main/docs/assets/img/Login.png)

## Features

Once you have logged into IFB Open OnDemand, the landing page will display several tabs across the top, including **Files**, **Jobs**, **Clusters** (shell access), **Interactive Apps**, and **My Interactive Sessions**. In the center of the page, direct links to popular interactive apps are prominently featured for easy access.

![Homepage](https://raw.githubusercontent.com/lkhamvongsa/OpenOnDemandDoc/main/docs/assets/img/OpenOnDemand_home_IFB.png)

## Files

The File menu lets you view and use files in different file spaces: your home directory and the projects directory (/shared/projects).
Selecting one of the file spaces takes you to a page that lets you navigate through the space in a graphical frame similar to a file browser on a personal computer. From here you can download, upload, create, delete and open files.

![Files](https://raw.githubusercontent.com/lkhamvongsa/OpenOnDemandDoc/main/docs/assets/img/Files.png)

!!! Tip

    The projects space contains all the "projects" directories hosted on the infrastructure. Use the text box filter to find your project **quickly**.

![Project_filter](https://raw.githubusercontent.com/lkhamvongsa/OpenOnDemandDoc/main/docs/assets/img/Projects_filter.jpg)


!!! Warning

    When you do not have access to a project, you will see an Error message like the one in the image below. 

![Project_acces_denied](https://raw.githubusercontent.com/lkhamvongsa/OpenOnDemandDoc/main/docs/assets/img/Projects_acces_denied.png)

## Jobs

Jobs can be monitored, created, edited and scheduled with the job management tools under the Jobs menu.

=== "Active Jobs"

    Under the "Active Jobs" tab you can view active jobs. You can choose to view your jobs or all jobs. From this menu you can also cancel your own jobs.

    ![Active_jobs_all](https://raw.githubusercontent.com/lkhamvongsa/OpenOnDemandDoc/main/docs/assets/img/Active_jobs_all.png)

=== "Job Composer" 

    Create and edit job scripts and schedule jobs under this menu.

    ![Jobs_composer](https://raw.githubusercontent.com/lkhamvongsa/OpenOnDemandDoc/main/docs/assets/img/Job_composer.png)

## Clusters (Shell Access)

The Clusters menu offers shell access to the login node within the IFB cluster. This shell terminal operates similarly to various other tools providing terminal access.

Upon initiating the Terminal, you will be prompted to enter your IFB cluster account password. Once entered successfully (no characters will appear on the screen as you type), your shell session on the login node will begin.

![Shell_access](https://raw.githubusercontent.com/lkhamvongsa/OpenOnDemandDoc/main/docs/assets/img/Shell_access.png)

From here, you can work on the cluster using command line to run SLURM commands. If you are new to SLURM, please go through our documentations :

 - [SLURM at IFB Core](https://ifb-elixirfr.gitlab.io/cluster/doc/slurm/slurm_at/)
 - [SLURM user guide](https://ifb-elixirfr.gitlab.io/cluster/doc/slurm/slurm_user_guide/)
 - [SLURM examples](https://ifb-elixirfr.gitlab.io/cluster/doc/slurm/slurm_examples/)
 - [SLURM GPU](https://ifb-elixirfr.gitlab.io/cluster/doc/slurm/slurm_GPU/)
 - [SLURM advanced guide](https://ifb-elixirfr.gitlab.io/cluster/doc/slurm/slurm_advanced_guide/)
 - [SLURM Cookbook](https://ifb-elixirfr.gitlab.io/cluster/doc/slurm/slurm_cookbook/)
 - [SLURM Running interactive jobs](https://ifb-elixirfr.gitlab.io/cluster/doc/slurm/sinteractive/)

!!! Warning
    
    Please don't run any bioinformatics tools directly on the login node. The login node is not a compute node ; it has no resources to run heavy calculation.

## Interactive Apps

The Interactive Apps menu contains options to launch certain applications that have graphical user interfaces (GUIs) for interactive use on IFB cluster. Each application is running in a dedicated SLURM jobs with the resources (RAM, CPU, GPU) you request.

Current supported applications include :

 - JupyterLab : JupyterLab is a web-based interactive development environment for notebooks, code and data
 - RStudio Server : RStudio Server is web based version of the RStudio integrated development envrionment (IDE) for R

To find out more about using apps, please consult the following documents :

 - [Starting a JupyterLab session](Starting_JupyterLab_session.md)
 - [Starting a Rstudio server](Starting_Rstudio_server.md)

 