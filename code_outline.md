<p align="center">
<img src="./images/Ce11.gif" width="50">
</p>

# Ce11: Cellerator Code
*TL;DR* The code and documentation used to run Cellerator.

Cellerator code is a combination of [python](https://www.python.org), [XOJO](https://www.xojo.com), and [gCode](https://en.wikipedia.org/wiki/G-code).  Python was used for its flexibility, open source nature, and ease of use.  Xojo was used for its cross platform GUI programming interface and ease of use, its ability to compiles ARM for the raspberry pi. And gCode was used because its the industry standard.


### Tabs
1. [User Login](#user-login)
2. [Lab](#lab)
3. [Hand Tools](#hand-tools)
4. [Bench Tools](#bench-tools)
5. [Experiment Calendar](#experiment-calendar)
6. [Design Experiment](#design-experiment)
7. [Peer Review](#peer-review)
8. [Sell Downtime](#sell-downtime)
9. [Data Analysis](#data-analysis)
10. [Electronic Laboritory Notebook](#electronic-laboritory-notebook)
11. [Publish](#publish)
12. [gCode Sender](#gcode-sender)
13. [Photo](#photo)



## User Login
*TL;DR* Logging into Cellerator adds the user signature to each process.

>`"Anonymity is the death of responsibility, accountability, and credibility"`

**About:**
 When you first log into Cellerator application the first page loaded is the **Login** page.  This page loads oricid.org and the user is prompted to log in.  Once logged in Cellerator aquires the users sixteen digit ^0000-0000-0000-0000^ [ORCID](http://orcid.org) to sign each step of your experiment.

**From the site**
>ORCID provides a persistent digital identifier (an ORCID iD) that you own and control, and that distinguishes you from every other researcher. You can connect your iD with your professional information — affiliations, grants, publications, peer review, and more. You can use your iD to share your information with other systems, ensuring you get recognition for all your contributions, saving you time and hassle, and reducing the risk of errors.


|Code|Version  |Date |
|--|--|--|
| [XOJO Orcid ID Code](./code/OrcidID/OrcidID.md)| *α*lpha |2020/12/22|


## Lab
*TL;DR* The Lab page is a snapshot of all Cellerators under your control, with quick feature access.

>`"There are two spiritual dangers in not owning a farm. One is the danger of supposing that breakfast comes from the grocery, and the other that heat comes from the furnace."` ~Aldo Leopold

**About:** The **Lab** page is a snap shot of your Cellerator Setup.  This snapshot is a bird's eye view of your local and recruited Cellerators. Whether you have a single Cellerator, Cellerator extender, Dual Cellerators, recruited Cellerators, or a Cellerator farm.  

The snapshot shows a quick overview of each cellerator, with quicklinks to other features.


|Code|Version  |Date |
|--|--|--|
| [MD file](LINK)| *α*lpha *β*eta *γ*amma 1.0 |YYYY/MM/DD|

## Hand Tools
*TL;DR*

>`""` ~Name

**About:**  The **Hand Tool** page allows the user to modify features of hand tools. In the Hand tool page you start by selecting the Cellerator, once selected a list of active hand tools are displayed. From here you can view, add, delete, or update drivers for hand tools.

When viewing properties of a hand tool, first you click on the hand tool of interest. This loads and displays data about this tool; Name, Firmware Version, Documentation Link, Physical Location, Tool Volume, Tip Location, Data Pins, and Data Protocol. Each field can be update from this page.  
1. *Name*: can be changed if multiple of the same tools are present.
2. *Firmware Version*: is displayed as a number, if a new version is available a download arrow is present.
3. *Documentation*: Contains a URL to the online documentation on the selected hand tool.
4. *Physical Location*: This is a global variable for Cellerator knows where to acquire the tool.
5. *Tool Volume*: This helps Cellerator move the Hand Tool in 3D space and avoid obstacles.
6. *Tip Location*: This tells Cellerator where the tip is located in 3D space in relation to an experiment and bench tool access ports location.
7. *Data Pins*: this explains which pins are utilized and the mode of the pin.
8. *Data Protocol*: This contains the language reference of the hand tool.
</br></br>**NOTE:** These properties are attached to the experiment.


view hand tools, add hand tools, and edit hand tools.



|Code|Version  |Date |
|--|--|--|
| [MD file](LINK)| *α*lpha *β*eta *γ*amma 1.0 |YYYY/MM/DD|

## Bench Tools
*TL;DR*

>`""` ~Name

**About:**  



|Code|Version  |Date |
|--|--|--|
| [MD file](LINK)| *α*lpha *β*eta *γ*amma 1.0 |YYYY/MM/DD|

## Experiment Calendar
## Design Experiment
## Peer Review
## Sell Downtime
## Data Analysis
## Electronic Laboritory Notebook
## Publish
## gCode Sender
## Photo


## Authors

* **[S James Parsons Jr](https://www.linkedin.com/in/sjamesparsonsjr/)**

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
