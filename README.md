# BioBB community workflows

Welcome to the community repository for the **BioExcel Building Blocks Workflows**. In this repo there are all the workflows developed by the community members. If you want to take a look to the BioBB **demonstration workflows**, please visit the [**BioExcel Building Blocks Workflows**](https://github.com/bioexcel/biobb_workflows/) repository.

## How to contribute

If you have developed a workflow using **BioExcel Building Blocks**, you can contribute to this repository doing a **Pull Request**. Please follow the steps defined in this section.

### Fork the repository

Click the **"Fork" button** at the top-right corner of this repository page. This will create a copy of the repository under **your GitHub account**.

### Clone the Forked Repository

Go to **your GitHub profile** and find the forked **biobb_community_wfs** repository under your profile. Then, click the **"Code" button** on the repository page and copy the repository URL (HTTPS/SSH). Open your terminal and run:

    git clone <repository-url>

### Create a New Branch

Run the following command to **create** and **switch** to a **new branch**:

    git checkout -b <branch-name>

It's recommended to name the new branch after the **new workflow** name (ie _biobb_wf_md_setup_).

### Add new workflow

Now, copy **your workflow** into the repository. Please use the following **file structure**:

📂 workflow_name_main_folder
- 📖 README.md
- 📁 workflow_name_subfolder

Where:

#### workflow_name_main_folder

It's the name of your workflow starting by the prefix _biobb_wf_\_ (ie _biobb_wf_md_setup_)

#### README.md

It's a copy of the [README-template.md](README-template.md) file that can be found in this same repository. Add here all the information needed in order to **install** and **run** the workflow.

#### workflow_name_subfolder

It's the name of your workflow starting by the prefix _biobb_wf_\_ (ie _biobb_wf_md_setup_). 

This folder must be a [GitHub submodule](https://gist.github.com/gitaarik/8735255) for the sake of improving the maintenance of this repository. For creating a new submodule from your own repo, please type the following instruction:

      git submodule add git@github.com:path_to/submodule.git <workflow_name_subfolder>

### Commit and Push

Stage the Changes:

    git add .

Commit the Changes:

    git commit -m "Added new XXXX wf"

Push Changes to GitHub (don't forget to push the current branch):

    git push origin <branch-name>

### Create a Pull Request

Go to the original repository [https://github.com/bioexcel/biobb_community_wfs](https://github.com/bioexcel/biobb_community_wfs).

In this repo, GitHub should detect the new branch and show a **"Compare & pull request" button**. Click it.

Alternatively, go to the **"Pull Requests" tab** and click the **"New pull request" button**.

**Select Branches:** ensure the base fork (original repository) and its default branch (usually main or master) are selected, and compare it with the head fork (your repository) and your branch.

**Fill Out the PR Form:** provide a title and description for your PR.
Describe what changes you made and why they are necessary. Click the **"Create pull request" button**.


## Copyright & Licensing

This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU Horizon Europe [101093290](https://cordis.europa.eu/project/id/101093290), EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).

* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)

Licensed under the
[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.

![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")