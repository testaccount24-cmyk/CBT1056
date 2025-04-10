# CBT1056
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. GitHub repos will be deleted and created during this period...

```
//***FILE1056 is by Frank Clarke, Oldsmar FL, USA and features a    *   FILE1056
//*           REXX exec called RUNDATA.  RUNDATA provides a means   *   FILE1056
//*           of customizing all your REXX execs for a particular   *   FILE1056
//*           z/OS installation or instance, WITHOUT ANY INTERNAL   *   FILE1056
//*           CHANGES TO THE REXX EXEC AT ALL (other than the       *   FILE1056
//*           one-time mod to make your EXEC RUNDATA-aware, of      *   FILE1056
//*           course).                                              *   FILE1056
//*                                                                 *   FILE1056
//*           Please see member $AUTOCUS for more detail and        *   FILE1056
//*           specific information.                                 *   FILE1056
//*                                                                 *   FILE1056
//*           When RUNDATA is incorporated in your REXX execs,      *   FILE1056
//*           then ALL CUSTOMIZATION IS IN AN EXTERNAL TABLE, SO    *   FILE1056
//*           NO CHANGES NEED TO BE MADE IN THE EXEC ITSELF.  You   *   FILE1056
//*           just change the table, for each z/OS instance or      *   FILE1056
//*           LPAR.  If you install a new version of the REXX exec  *   FILE1056
//*           and RUNDATA is supported, then you do not need to     *   FILE1056
//*           customize the new version.  RUNDATA does it           *   FILE1056
//*           automatically.                                        *   FILE1056
//*                                                                 *   FILE1056
//*           This file is meant to show you how RUNDATA works.     *   FILE1056
//*           However, RUNDATA support is included in some of the   *   FILE1056
//*           REXX execs from CBT Files 433 and 435 already.  Over  *   FILE1056
//*           here in this file, we will show in detail how         *   FILE1056
//*           RUNDATA is set up and installed.                      *   FILE1056
//*                                                                 *   FILE1056
//*           Several other subroutines are also included because   *   FILE1056
//*           they are required either by RUNDATA or by another     *   FILE1056
//*           subroutine.  DFLTTLIB, LA, SYSUMON, and TRAPOUT may   *   FILE1056
//*           already be on your system by virtue of downloading    *   FILE1056
//*           another package in this family, files 433, 435, or    *   FILE1056
//*           1044.  You may safely dummy-out SYSUMON if you don't  *   FILE1056
//*           want it.                                              *   FILE1056
//*                                                                 *   FILE1056
//*        email:  rexxhead@yahoo.com, Frank Clarke                 *   FILE1056
//*                                                                 *   FILE1056
//*               'FCLARKE.RUNDATA.EXEC' - Directory                *   FILE1056
//*                                                                 *   FILE1056
//*                 Usage or                                        *   FILE1056
//*       Member    Caller      Description                         *   FILE1056
//*       ========  =========   =================================   *   FILE1056
//*                                                                 *   FILE1056
//*       $AUTOCUS  text        Describes auto-customization        *   FILE1056
//*                             technique                           *   FILE1056
//*                                                                 *   FILE1056
//*       $HOWTO    text        How to operate RUNDATA              *   FILE1056
//*                                                                 *   FILE1056
//*       $INITS    text        Initialization instructions         *   FILE1056
//*                                                                 *   FILE1056
//*       @FIL1056  text        Inventory                           *   FILE1056
//*                                                                 *   FILE1056
//*       @RUNDATA  text        Code examples                       *   FILE1056
//*                                                                 *   FILE1056
//*       DFLTTLIB  exec        Set default ISPTLIB                 *   FILE1056
//*                                                                 *   FILE1056
//*       DUMPDATA  exec        Generate a reload exec for          *   FILE1056
//*                             RUNDATA                             *   FILE1056
//*                                                                 *   FILE1056
//*       LA        exec        LISTA ST to a scrollable display    *   FILE1056
//*                                                                 *   FILE1056
//*       RDSPLAIN  text        More information about RUNDATA      *   FILE1056
//*                             operations                          *   FILE1056
//*                                                                 *   FILE1056
//*       RUNDATA   exec        Maintain application-specific       *   FILE1056
//*                             information                         *   FILE1056
//*                                                                 *   FILE1056
//*       SHOWDATA  exec        Full-screen access to RUNDATA       *   FILE1056
//*                                                                 *   FILE1056
//*       STRSORT   exec        Sort a string of words              *   FILE1056
//*                                                                 *   FILE1056
//*       SYSUMON   exec        Count tool usage                    *   FILE1056
//*                                                                 *   FILE1056
//*       TRAPOUT   exec        Trap trace output to DASD           *   FILE1056
//*                                                                 *   FILE1056
```
