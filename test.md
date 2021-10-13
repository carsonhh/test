1.  [CHPC Guide](./index.md)
2.  [Getting Started with UCGD Resources at
    CHPC](./Getting_Started_with_UCGD_Resources_at_CHPC.md)
3.  [Transfering Data](./Transfering_Data.md)
:::

# [ CHPC Guide : Globus ]
:::

::: {#content .view}
::: page-metadata
Created by [ Carson Holt]{.author}, last modified on Feb 05, 2020
:::

::: {#main-content .wiki-content .group}
Globus is a parallelized multi-stream data transfer solution. It is used
by the NFS funded XSEDE clusters, ENSEMBL, and US national laboratories.
Data transfer rates greater than 7 Gb/s can be achieved using Globus at
CHPC compared to \~1 Gb/s using tools like sftp, scp, and rsync. Most
importantly data streams are encrypted and the University of Utah has a
sign Business Association Agreement with Globus making all data
transfers HIPAA compliant.

In addition to fast data transfer, Globus also allows for easy and
secure sharing of files and directories to other individuals with
University of Utah IDs. Please use Globus as the prefered method of data
transfer into and out of the CHPC protected environment.

# CLI Interface and API {#Globus-CLIInterfaceandAPI}

You can transfer using Globus via the command line, programmatically
using available API\'s, or using a web browser enabled interface.
Install [Globus CLI](https://docs.globus.org/cli/){.external-link} on
any server where you wish to access Globus via the command line. See
the [Globus Quick Start
Guide](https://docs.globus.org/cli/quickstart/){.external-link} for more
info on using Globus CLI. Also to transfer files from your local
machines, you will also need to install [Globus Connect
Personal](https://www.globus.org/globus-connect-personal){.external-link}.

Example transfer command lines:

#\....

# Web interface {#Globus-Webinterface}

Go to <https://www.globus.org> to access the web interface. You can log
in with your Use the \"File Manager\" to search for CHPC endpoints using
the keyword \"University of Utah\" or endpoints at other institutions
using keywords like \"EBI\" or \"XSEDE\". If you installed Globus
Connect Personal, you can also find your local machine.

[![](/attachments/5963967/5964240.png){.confluence-embedded-image
width="1000" image-src="attachments/5963967/5964240.png"
unresolved-comment-count="0" linked-resource-id="5964240"
linked-resource-version="1" linked-resource-type="attachment"
linked-resource-default-alias="globus-web.png"
base-url="https://confluence.genetics.utah.edu"
linked-resource-content-type="image/png"
linked-resource-container-id="5963967"
linked-resource-container-version="8"}]{.confluence-embedded-file-wrapper
.confluence-embedded-manual-size}

# [[Creating/Sharing New Globus Collection](http://confluence.genetics.utah.edu/pages/viewpage.action?pageId=13828836){.external-link}]{style="color: rgb(0,0,0);"} {#Globus-Creating/SharingNewGlobusCollection}

Data can be shared both internally and externally by creating a new
\'Collection\' in Globus.  This is a similar process to creating shared
endpoints that we used previously, but with a couple of less intuitive
steps.

\

Quick guide:

1.  Login to Globus.
2.  Open \'Endpoint\' page.
3.  Search for and load the \'pe-dtn01\' endpoint.
4.  Open the \'Collections\' dialog page.
5.  Open the \'Add a Collection\' dialog page.
6.  Open the \'CHPC PE-DTN01 StorageGateway (POSIX)\'  dialog page.
7.  Fill in the \'Base Directory\', \'[Collection Display Name\',
    \'Descriptions\', \'Key Words\'
    (Fig. 1)]{style="color: rgb(33,37,41);"}
8.  Click the \'Share data on this new collection with others\'
9.  Use the \'User Search\' to find the user you\'re sharing with (make
    sure you have the correct user account!), click the \'Send E-mail\',
    set \'Permissions\' as read and/or write, optionally set a message
    and click \'Add Permission\'. (Fig. 2)

\

*Fig. 1 Create a Guest Collection*

[![Fig. 1 Create a Guest Collection](/attachments/5963967/13828889.png "Fig. 1 Create a Guest Collection"){.confluence-embedded-image
.confluence-content-image-border width="800"
image-src="attachments/5963967/13828889.png"
unresolved-comment-count="0" linked-resource-id="13828889"
linked-resource-version="1" linked-resource-type="attachment"
linked-resource-default-alias="Globus_Collection_Creation.png"
base-url="https://confluence.genetics.utah.edu"
linked-resource-content-type="image/png"
linked-resource-container-id="5963967"
linked-resource-container-version="8"}]{.confluence-embedded-file-wrapper
.confluence-embedded-manual-size}

\

*Fig. 2 Add Permissions*

[![Fig. 2 Add
Permissions](/attachments/5963967/13828890.png "Fig. 2 Add Permissions"){.confluence-embedded-image
.confluence-content-image-border width="800"
image-src="attachments/5963967/13828890.png"
unresolved-comment-count="0" linked-resource-id="13828890"
linked-resource-version="1" linked-resource-type="attachment"
linked-resource-default-alias="Add_Permissions_to_Collection.png"
base-url="https://confluence.genetics.utah.edu"
linked-resource-content-type="image/png"
linked-resource-container-id="5963967"
linked-resource-container-version="8"}]{.confluence-embedded-file-wrapper
.confluence-embedded-manual-size}

\
:::

::: {.pageSection .group}
::: pageSectionHeader
## Attachments: {#attachments .pageSectionTitle}
:::

::: {.greybox align="left"}
![](/images/icons/bullet_blue.gif){height="8" width="8"}
[globus-web.png](/attachments/5963967/5964240.png) (image/png)\
![](/images/icons/bullet_blue.gif){height="8" width="8"}
[Globus_Collection_Creation.png](/attachments/5963967/13828889.png)
(image/png)\
![](/images/icons/bullet_blue.gif){height="8" width="8"}
[Add_Permissions_to_Collection.png](/attachments/5963967/13828890.png)
(image/png)\
:::
:::
:::
:::

::: {#footer role="contentinfo"}
::: {.section .footer-body}
Document generated by Confluence on Oct 07, 2021 22:58

::: {#footer-logo}
[Atlassian](http://www.atlassian.com/)
:::
:::
:::
:::
