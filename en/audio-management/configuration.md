# Configuration 

---

- [Overview](#overview)
- [General settings](#general-settings)
- [Switching modules on and off](#switching-modules-on-and-off)
- [E-mail settings](#email-settings)
- [Sales settings](#sales-settings)
- [Distributor settings](#distributor-settings)
- [Define ISRC root](#isrc-root)

<a name="overview"></a>
## Overview      

### Where can I find the settings?
You will find the settings of your Affekt system in two places.
* Click the settings icon on the left quick panel bar
* Click on your user avatar picture in the upper right corner and then on SETTINGS

<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/Ud4ObNc277.png" width="500">
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/k4mWHhXsXG.png" width="500">

### Selecting your audio management / record label
Select the record label you want to set on the colored tab bar.
Here you will find a list of all audio management systems that belong to your customers at Affekt.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/GvFZYZ4QFh.png" width="500">

<a name="general-settings"></a>
## General settings  
### Exclusivity-types 
We have defined 4 exclusivity types for each Record Label Start by default.
1. exclusive - for all tracks that belong exclusively to your repertoire in the label, but need a separate contract for compilations
2. non-exclusive-full - for all tracks that are exclusive to your repertoire and a license for compilation is available
3. non-exclusive - for all tracks that are non-exclusive to your repertoire
4. not-available - for tracks that are no longer licensed for release on your label, for example older expired licenses (but these tracks must remain in the database for billing purposes)

<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/PDU2CrSxJw.png" width="500">

### Document-Types    

> {warning} We are currently implementing these functions.

<a name="switching-modules-on-and-off"></a>
## Switching modules on and off
We are always developing cool new functions for record labels, but we also offer you the possibility to switch off single modules. If you do not need a module, turn it off. However, we do not delete any data in the background if you have already used a module once. We just hide it.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/jyBnoCaIHY.png" width="500">  

### Overview of module development
| # | Name   | Status |
| : |   :-   |  :  |
| 1 | Remixes | experimental - in development |
| 2 | Demos / Preview Tracks | experimental - in development |
| 3 | DJ-Sets | experimental - in development |

<a name="email-settings"></a>
## E-mail settings           
For outgoing e-mails you can specify specific CC addresses here. Please enter your desired addresses here..
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/4nT1bAprgq.png" width="500">

### Overview of current Outgoing-Emails
| # | Name   | Description |
| : |   :-   |  -:-  |
| 1 | Release Info Email | A release information that goes to your artist. Under RELEASES we have included a tool that allows you to notify your artist about the status of his release on your label. |
| 2 | Royalty Email | This email contains the royalty statement that you send to your artists. You can find these tools under ACCOUNTS and the respective artist to be billed. |

<a name="sales-settings"></a>
## Sales settings
### Cross-System Currency
Please define your basic currency with which you work in your record label. We currently support only one currency per **Audio Management**. This currency is displayed for your artists in their own overviews and also on the royalty statements.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/HAMATsZ0Bs.png" width="500">

### Billing-bases
There are 3 standard settlement types.
1. About Digital Retail Sales - Digital Single NET
2. About Digital Bundle Sales - Digital Bundle NET
3. About Streams - Digital Stream NET

You can add other special types of billing if you need them.

> {info} Switching on and off only shows and hides the settlement type in the respective editors. You don't lose data when you shut down a type here. The shares set on your licenses remain in the background.

<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/o3r9JiD7e7.png" width="800">

### Abrechnungsarten 
| # | Name   | Description |
| : |   :-   |  -:-  |
| 1 | Retail NET | CD / Retail sale |
| 2 | Retail Dealer Selling Price | Deduction/Share at wholesale price |
| 3 | Retail Distribution Selling Price | Deduction/Share according to distributor price |
| 4 | Digital Single Distribution Selling Price | Digital single sale with Deduction/Share according to distributor price |
| 5 | Digital Bundle Distribution Selling Price | Digitaler Bundle-Verkauf mit Abzug/Share nach Distributorenpreis |
| 6 | Digital Stream Distribution Selling Price | Stream mit Abzug/Share nach Distributorenpreis |
| 7 | Digital Single NET on Compilations | Digitaler Einzel-Verkauf auf einer Compilation |
| 8 | Digital Bundle NET on Compilations | Digitaler Bundle-Verkauf auf einer Compilation |
| 9 | Digital Stream NET on Compilations | Stream auf einer Compilation |

<a name="distributor-settings"></a>
## Distributor settings
Here you will find our previously supported distributors with their FTP settings. Please enter here the FPT access data that your distributor provides on the respective backend. Our system is able to automatically upload all WAV files of a release to the FTP server of the distributor during the PUBLISHING process.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/YS3Ty4N6H7.png" width="800">

<a name="isrc-root"></a>
## Define ISRC root
Please enter here your ISRC roots, which you use for a record label. We have built an integrated ISRC manager to help you not to skip consecutive numbers or even worse to create duplicates.

> {primary} Without ISRC root, you will have to manually enter all ISRC codes for each track yourself. Otherwise, the billing system will not be able to assign and function.

<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/WswJqcmrmZ.png" width="800">

> {info} The ISRC code is a 12-digit code and stands for International Standard Recording Code.  The first two letters stand for the country in which the title was published. The next three digits stand for the label that published the title. The next two figures represent the year of publication. The last five numbers are used to count through the individual titles. Each title and each version of a title has its own ISRC code. The ISRC code is encoded in the TOC (Table of Contents) of a master CD. It identifies each title at GEMA and is read out by the radio and television stations to facilitate GEMA accounting. The ISRC codes are determined by the label that releases the album. The allocation of the code can be requested from the IFPI.

### TRACK EDIT - ISRC-Manager
Here is an outlook on the ISRC manager at a TRACK EDIT. As you can see, if you enter a root, you can select it and the system will give you the next ISRC code. This means that there are no gaps in the consecutive numbering and no duplicates.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/I9xLWerFWX.png" width="800">
