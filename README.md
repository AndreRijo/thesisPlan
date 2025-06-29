<img src="http://joaomlourenco.github.io/novathesis/novathesis-latex-logo-v5.jpg" width="600"/>
<meta property="og:image" content="http://joaomlourenco.github.io/novathesis/novathesis-latex-logo-v5.svg" />

*Do you have a suggestion
[![GitHub forks](https://img.shields.io/github/forks/joaomlourenco/novathesis.svg?style=social&label=Fork)](https://github.com/joaomlourenco/novathesis)
[![GitHub stars](https://img.shields.io/github/stars/joaomlourenco/novathesis.svg?style=social&label=Star)](https://github.com/joaomlourenco/novathesis)
[![GitHub watchers](https://img.shields.io/github/watchers/joaomlourenco/novathesis.svg?style=social&label=Watch)](https://github.com/joaomlourenco/novathesis)
[![GitHub followers](https://img.shields.io/github/followers/joaomlourenco.svg?style=social&label=Follow)](https://github.com/joaomlourenco/novathesis)

[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/joaomlourenco/novathesis/graphs/commit-activity)
[![made-with-latex](https://img.shields.io/badge/Made%20with-LaTeX-1f425f.svg?color=green)](https://www.latex-project.org/)
[![GitHub license](https://img.shields.io/badge/License-LaTeX%20v1.3c-green.svg)](https://www.latex-project.org/lppl/lppl-1-3c)

[![GitHub release](https://img.shields.io/github/release/joaomlourenco/novathesis.svg)](https://github.com/joaomlourenco/novathesis/releases/)
[![GitHub commits](https://img.shields.io/github/commits-since/joaomlourenco/novathesis/2.0.0.svg)](https://github.com/joaomlourenco/novathesis/commit/)
![![Last commit](https://github.com/joaomlourenco/novathesis)](https://img.shields.io/github/last-commit/joaomlourenco/novathesis?color=blue)

[![GitHub license](https://img.shields.io/badge/SAY%20THANKS-€5-orange.svg)](https://www.paypal.com/donate/?hosted_button_id=8WA8FRVMB78W8)



--------
## Table of Contents

* [About](#about)
* [Getting Started](#getting-started)
	* [With a Local LaTeX Installation](#with-a-local-latex-installation)
	* [With a Remote Cloud-based Service](#with-a-remote-cloud-based-service)
* [Getting Help](#getting-help)
	* [Problems and Difficulties](#problems-and-difficulties)
	* [Suggestions, Bugs and Feature Requests](#suggestions-bugs-and-feature-requests)
* [Recognition](#recognition)
* [List of Supported Schools](#list-of-supported-schools)
    * [Showcase](#showcase)
* [Disclaimer](#disclaimer)
* [Microsoft Word Templates](#word-templates)


--------

**If you opt for using this project, please give it a star by clicking the (⭐️) at the top right of the [project's page at GitHub](https://github.com/joaomlourenco/novathesis).**

--------
## About

The [“*novathesis*” LaTeX template](https://joaomlourenco.github.io/novathesis/) is an Open Source project for writing thesis, dissertations, and other monograph-like documents, which…

* **Is very easy to use for the LaTeX beginners:**
    * Just fill the cover data and your chapters with text!
* **Is flexible and adaptable for the LaTeX experts:**
    * It's LaTeX!  What would you expect?! 😉
* **Includes dozens of options that answer the requests from the large user's community (1000's users):**
    * e.g., multiple chapter styles, multiple font styles, automatic book spine generation, …
* **Supports multiples schools:**
    * Currently supports +20 Schools, drawing the covers and typesetting the text according to the rules  of each School.

*This work is licensed under the LaTeX Project Public License v1.3c. To view a copy of this license, visit the [LaTeX project public license](https://www.latex-project.org/lppl/lppl-1-3c/).*

--------
## Getting Started

### With a Local LaTeX Installation

*[See below](#with-a-remote-cloud-based-service) for alternatives to a local LaTeX installation*

*See “[minimal installation](minimal_installation)” for instructions on how to build/use a minimal installation of LaTeX (<100 MB vs. 5GB for tex-live), which is just enough to compile the template successfully*

1. Download LaTeX:
	* **Windows:** install either [MikTeX](https://miktex.org) or [TeX-Live](https://www.tug.org/texlive/).
	* **Linux:** install [TeX-Live](https://www.tug.org/texlive/).
	* **macOS:** install [MacTeX](https://www.tug.org/mactex/) (a macOS version of [TeX-Live](https://www.tug.org/texlive/)).
2. Download “novathesis” by either:
	* Cloning the [GitHub repository](https://github.com/joaomlourenco/novathesis) with <kbd>git clone https://github.com/joaomlourenco/novathesis.git</kbd>; or
	* Downloading the [latest version from the GitHub repository as a Zip file](https://github.com/joaomlourenco/novathesis/archive/master.zip)
3. Compile the document with you favorite LaTeX processor (pdfLaTeX, XeLaTeX or LuaLaTeX):
	* The main file is named “*template.tex*”.  
	* Either load it in your favorite [LaTeX text editor](https://en.wikipedia.org/wiki/Comparison_of_TeX_editors) or compile it in the terminal with
<kbd>latexmk -pdf template</kbd>.  If you use a LaTeX text editor, please notice that the NOVAthesis template uses `biber`and not `bibtex` to process the bibliography, which means that most probably you have to open the _Editor Preferences_ and somehwere (depends on the Editor) chage `bibtex`to `biber`.
	* If Murphy is elsewhere, LaTeX will create the file “`template.pdf`”, which you may open with your favorite PDF viewer.
4. Edit the files in the “*Config*” folder:

| File                      | Contents                                                           |
|---------------------------|--------------------------------------------------------------------|
| `0_memoir.tex`            | Options specific for the `memoir` package.  _Don't touch this file unless you know what you are doing!_                                                                              |
| `1_novathesis.tex`        | Configure the template, i.e., the document type, the school, etc.  |
| **`2_biblatex.tex`**      | **Configure the bibliography.**                                        |
| **`3_cover.tex`**         | **Configure cover contents (e.g., author's name, thesis/dissertation title, advisers, committee, etc)**                                                                        |
| **`4_files.tex`**         | **Configure the the files for chapters, appendices, annexes, etc…**     |
| **`5_packages.tex`**      | **Configure additional packages and commands**                     |
| `6_list_of.tex`           | Configure the lists to be printed (table of contents, list of figures, list of tables, list of listings, etc).  _Don't touch this file unless you know what you are doing!_       |
|                           |                                                                    |
| `9_nova_fct.tex`          | Configuration specific to **nova/fct**                             |
| `9_nova_ims.tex`          | Configuration specific to **nova/ims**                             |
| `9_nova_itqb.tex`         | Configuration specific to **nova/itqb**                            |
| `9_ulisboa_fmv.tex`       | Configuration specific to **ulisboa/fmv**                          |
| `9_uminho.tex`            | Configuration specific to **uminho** (all schools)                 |

5. Recompile de document:
	* See 3. above.
6. You're done with a beautifully formatted thesis/dissertation! 😃

### With a Remote Cloud-based Service

*[See above](#with-a-local-latex-installation) for using a local installation of LaTeX*

*NOVAthesis v6.5.3 is available as an [Overleaf template](https://www.overleaf.com/latex/templates/novathesis-v6-dot-5-3/jhqwhtcwbmqc).  Just select <kbd>open as template</kbd> and follow from [step 3 above](#with-a-local-latex-installation)!*

1. Download the [latest version from the GitHub repository as a Zip file](https://github.com/joaomlourenco/novathesis/archive/master.zip).
2. Login to your favorite LaTeX cloud service.  I recommend [Overleaf](https://www.overleaf.com?r=f5160636&rm=d&rs=b) but there are alternatives (these instructions apply to Overleaf  and you'll have to adapt for other providers).
3. In the menu select <kbd>New project</kbd>-><kbd>Upload project</kbd>
4. Upload the zip with all the "novathesis" files.
5. Select “*template.tex*” as the main file.
6. Follow from [step 3 above](#with-a-local-latex-installation)

--------
## Getting Help

### Problems and Difficulties

Check the [wiki](https://github.com/joaomlourenco/novathesis/wiki) and have some hope! :smile:

If you couldn't find what you were looking for, ask for help in:

* The [GitHub Discussions page](https://github.com/joaomlourenco/novathesis/discussions) (only EN please) at https://github.com/joaomlourenco/novathesis/discussions.
* The [Facebook page](https://www.facebook.com/groups/novathesis/) (PT or EN) at https://www.facebook.com/groups/novathesis.
* You may also give a look at the [novathesis blog](https://novathesis.blogspot.pt) at [https://novathesis.blogspot.pt](https://novathesis.blogspot.pt).

The [GitHub Discussions page](https://github.com/joaomlourenco/novathesis/discussions) and the [Facebook page](https://www.facebook.com/groups/novathesis/) are the right places to ask for help and support!  *Please don't try to contact me directly for questions or support, by email or any other channel! I will not answer such requests…*

### Suggestions, Bugs and Feature Requests

* **Do you have a suggestion?** Please add it to the [wiki](https://github.com/joaomlourenco/novathesis/wiki) and help other users!
* **Did you find a bug?**  Please [open an issue](https://github.com/joaomlourenco/novathesis/issues). Thanks!
* **Would you like to request a new feature (or support of a new School)?**  Please [open an issue](https://github.com/joaomlourenco/novathesis/issues). Thanks!

--------
## Recognition

This template is the result of hundreds (yes! *hundreds*) of hours of work from the main developer.  If you use this template, please be kind and give something back by choosing at least one of the following:

1. Cite the NOVAthesis manual in your thesis/dissertation.  Just use `\cite{novathesis-manual}` (the correct bibliographic reference, as shown below, will be added automatically).

         @Manual{novathesis-manual,
              title        = "{The NOVAthesis Template User's Manual}",
              author       = "João M. Lourenço",
              organization = "NOVA University Lisbon",
              year         = "2021",
              url          = "https://github.com/joaomlourenco/novathesis/raw/master/template.pdf",
         }

1.  [**Make a small donation**](https://paypal.me/novathesis). We will [keep a list thanking to all the identified donors](https://github.com/joaomlourenco/novathesis/wiki#-donations) that identify themselves in the “*Add special instructions to the seller:*” box.

1. Give the NOVAthesis project a star in GitHub by clicking in the star at the top-right of the [project's home page](https://github.com/joaomlourenco/novathesis).

--------
## List of Supported Schools

* NOVA University Lisbon
    * [NOVA School for Science and Technology](https://www.fct.unl.pt) (FCT-NOVA)
    * [NOVA Information Management School](https://www.novaims.unl.pt) (NOVA-IMS)
        * [PhD in Information Management](https://www.novaims.unl.pt/doutoramento)
        * [Master in Geographical Information Systems and Science](https://www.novaims.unl.pt/unigis)
        * [Master in Statistics and Information Management](https://www.novaims.unl.pt/megi)
        * [Master in Information Management](https://www.novaims.unl.pt/mgi)
        * [Master in Geospatial Technologies](https://www.novaims.unl.pt/geotech)
        * [Master in Data Science and Advanced Analytics](https://www.novaims.unl.pt/mdsaa)
        * [Masters in Geospatial Technologies](https://mastergeotech.info)
    * [National School of Public Heath](https://www.ensp.unl.pt) (ENSP-NOVA)
    * [Faculdade de Ciências Humanas e Sociais](https://www.fcsh.unl.pt) (FCSH-NOVA)
    * [Instituto de Tecnologia Química e Biologica Antonio Xavier](https://www.itqb.unl.pt) (ITQB-NOVA)
* University of Lisbon
    * [Instituto Superior Técnico](https://tecnico.ulisboa.pt) (IST-ULISBOA)
    * [Faculdade de Ciências](https://ciencias.ulisboa.pt) (FC-ULISBOA)
    * [Faculdade de Medicina Veterinária](https://www.fmv.ulisboa.pt) (FMV-ULISBOA)
* University of Minho
    * [Escola de Arquitetura](https://www.arquitetura.uminho.pt) (EA-UMIMHO)
    * [Escola de Ciências](https://www.ecum.uminho.pt) (EC-UMIMHO)
    * [Escola de Direito](https://www.direito.uminho.pt) (ED-UMIMHO)
    * [Escola de Economia e Gestão](https://www.eeg.uminho.pt) (EEG-UMIMHO)
    * [Escolha de Engenharia](https://www.eng.uminho.pt) (EE-UMIMHO)
    * [Escola de Medicina](https://www.med.uminho.pt) (EM-UMIMHO)
    * [Escola de Psicologia](https://www.psi.uminho.pt) (EP-UMIMHO)
    * [Escola Superior de Enfermagem](https://www.ese.uminho.pt) (ESE-UMIMHO)
    * [Instituto de Ciências Sociais](https://www.ese.uminho.pt) (ICS-UMIMHO)
    * [Instituto de Educação](https://www.ie.uminho.pt) (IE-UMIMHO)
    * [Instituto de Letras e Ciências Humanas](https://www.ilch.uminho.pt) (ILCH-UMIMHO)
    * [Instituto de Investigação em Biomateriais, Biodegradáveis e Biomiméticos](https://i3bs.uminho.pt) (I3Bs-UMIMHO)
* Universidade Lusófona de Humanidades e Tecnologias
    * [Departamento de Engenharia Informática e Sistemas de Informação](http://informatica.ulusofona.ptpt) (ULHT-DEISI)
<!-- * ISCTE – Instituto Universitário de Lisboa
    * [Escola de Tecnologia e Arquitectura](https://ciencia.iscte-iul.pt/schools/escola-tecnologias-arquitectura) (ETA-ISCTE-IUL) _NOTE: this template is outdated (there are new covers/specifications)_ -->
* Instituto Politécnico de Lisboa
    * [Instituto Superior de Engenharia de Lisboa](https://www.isel.pt) (ISEL-IPL)
* Instituto Politécnico de Setúbal
    <!-- * [Escola Superior de Saúde](https://www.ess.ips.pt) (ESS-IPS) -->
    * [Escola Superior de Tecnologia do Barreiro](https://www.estbarreiro.ips.pt) (ESTB-IPS)
* Other Schools/Degrees
    * [Escola Superior de Enfermagem do Porto](https://www.esenf.pt/pt/) (ESEP)

<!-- -------- -->
### Showcase

Although the template goes far beyond the cover… some covers from the supported schools are is display below.

<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ipl-isel-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ips-ests-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-ensp-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-ensp-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-fcsh-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-fcsh-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-fct-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-fct-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-ims-msc-mcsig-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-ims-msc-megi-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-ims-msc-mgi-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-ims-msc-mgt-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-ims-msc-mmaa-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-ims-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-itqb-msc-gray-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-itqb-msc-green-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-itqb-phd-gray-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/nova-itqb-phd-green-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/other-esep-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ulht-deisi-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ulht-deisi-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ulisboa-fc-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ulisboa-fc-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ulisboa-fmv-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ulisboa-fmv-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ulisboa-ist-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/ulisboa-ist-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ea-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ea-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ec-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ec-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ed-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ed-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ee-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ee-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-eeg-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-eeg-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-em-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-em-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ep-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ep-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ese-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ese-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-i3b-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-i3b-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ics-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ics-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ie-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ie-phd-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ilch-msc-en.svg" border="1" width="100"/></kbd>&nbsp;&nbsp;<kbd><img src="https://raw.githubusercontent.com/joaomlourenco/novathesis/gh-pages/Showcase/Covers/SVG/uminho-ilch-phd-en.svg" border="1" width="100"/></kbd>



--------
## Disclaimer

These are not official templates for FCT-NOVA nor any other School, although we have done our best to make it fully compliant to each School regulations for thesis/dissertation presentation.

All [contributors](https://github.com/joaomlourenco/novathesis/wiki#help-with-the-project-patches-and-new-features), both sporadic and regular, are welcome. :) Please [contact me](http://docentes.fct.unl.pt/joao-lourenco) to join the team.

--------
## Word Templates

*If you are here looking for the (deprecated) Word templates (not maintained anymore), please go to [this other repository](https://github.com/joaomlourenco/novathesis_word).*
