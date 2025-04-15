# CBT967
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 967 is the CBT Usermod Collection for ISPF (CUCI)         *   FILE 967
//*                                                                 *   FILE 967
//* Tom Conley, formerly SHARE's ISPF Advocate (now defunct), is    *   FILE 967
//* establishing this collection to provide function that will in   *   FILE 967
//* all likelihoood not be provided by IBM.  IBM's investment in    *   FILE 967
//* ISPF has steadily dwindled since z/OS V2R1, while investment in *   FILE 967
//* z/OSMF has vastly increased.  There is still a user community   *   FILE 967
//* for ISPF that requires increased function.  Even with recent    *   FILE 967
//* events, where IBM reversed course and increased ISPF            *   FILE 967
//* development resources for z/OS V2R5, CUCI will continue to      *   FILE 967
//* provide extended function for ISPF wherever possible.           *   FILE 967
//*                                                                 *   FILE 967
//*       email:  Pinnacle <pinncons@rochester.rr.com>              *   FILE 967
//*                                                                 *   FILE 967
//* Submissions to this collection should be in SMP/E usermod       *   FILE 967
//* format.  Manual hacks are accepted, but not encouraged.  It is  *   FILE 967
//* expected that the ISPF community will provide functions to this *   FILE 967
//* collection with the foregoing in mind.                          *   FILE 967
//*                                                                 *   FILE 967
//* This collection includes the following documentation members:   *   FILE 967
//*                                                                 *   FILE 967
//*  $$README - Installation instructions for z/OS sysprogs         *   FILE 967
//*  $CHANGES - Change log of all changes to CUCI                   *   FILE 967
//*  $HIGHLIT - Edit highlighting command HIGHLITE documentation    *   FILE 967
//*  $ISPCMDS - Command abbreviation documentation                  *   FILE 967
//*  $MANHACJ - JCL to manually create ISPF CUCI libraries          *   FILE 967
//*  $MANHACK - Instructions for the SMP/E-averse among us          *   FILE 967
//*  $MULTTSO - Instructions to unload ISPF Multi profile article   *   FILE 967
//*  $SHARZIP - Instructions for unloading CUCI SHARE presentations *   FILE 967
//*  $USRCONF - USRCCONF documentation for settings not in ISPCCONF *   FILE 967
//*  $34DELET - ISPF 3.4 delete documentation                       *   FILE 967
//*  @FILE967 - This member                                         *   FILE 967
//*                                                                 *   FILE 967
//* The following list of members is followed by a short            *   FILE 967
//* description to show you the ISPF usermods supported by the      *   FILE 967
//* CBT Usermod Collection for ISPF.                                *   FILE 967
//*                                                                 *   FILE 967
//*  BPXWISH  - ISHELL exec to reset UID(0) to user's default UID   *   FILE 967
//*  BPXWP99  - ISHELL panel to reset UID(0) to user's default UID  *   FILE 967
//*  ISH      - alias for BPXWISH                                   *   FILE 967
//*  ISHELL   - alias for BPXWISH                                   *   FILE 967
//*  ISPCMDS  - Command Table w/abbreviations (e.g. UDL for UDLIST) *   FILE 967
//*  ISR@PRIM - Primary option menu for default USRCCONF settings   *   FILE 967
//*  ISR@PR24 - z/OS V2R4 version of ISR@PRIM                       *   FILE 967
//*  ISREDDE2 - Edit panel for highlighting and Unix path prepend   *   FILE 967
//*  ISREDDE4 - Edit panel highlight/Unix path prepend (no act bar) *   FILE 967
//*  ISRED224 - z/OS V2R4 version of ISREDDE2                       *   FILE 967
//*  ISRED424 - z/OS V2R4 version of ISREDDE4                       *   FILE 967
//*  ISRPXASM - SAMPLIB member with language keywords for HILITE    *   FILE 967
//*  ISRUAASE - Allocation panel to prevent PDSE without mem gens   *   FILE 967
//*  ISRUAA24 - z/OS V2R4 version of ISRUAASE                       *   FILE 967
//*  ISRUDSL0 - Data set list to process VSAM for block deletes     *   FILE 967
//*  ISRUDS24 - z/OS V2R4 version of ISRUDSL0                       *   FILE 967
//*  ISRUMVC  - Copy dataset panel with other dataset primed        *   FILE 967
//*  ISRUUDL0 - UDLIST panel to reset UID(0) to user's default UID  *   FILE 967
//*  ISRUUD24 - z/OS V2R4 version of ISRUUDL0                       *   FILE 967
//*  ISRUULP  - UDLIST panel to reset UID(0) to user's default UID  *   FILE 967
//*  ISRUUL24 - z/OS V2R4 version of ISRUULP                        *   FILE 967
//*  ISRV01   - Message member to go along with ISRUAASE for PDSEs  *   FILE 967
//*  MULTITSO - Enterprise Systems Journal article in binary format *   FILE 967
//*  SHAREZIP - Binary member .zip file of CUCI SHARE presentations *   FILE 967
//*  UMBPXISJ - RECEIVE/APPLY UMBPXIS usermod for ISHELL UID(0)     *   FILE 967
//*  UMISCLMJ - RECEIVE/APPLY UMISCLM usermod for SISPLPA VSCR      *   FILE 967
//*  UMISPCMJ - RECEIVE/APPLY UMISPCM usermod for ISPCMDS abbrev's  *   FILE 967
//*  UMISRHIJ - RECEIVE/APPLY UMISRHI usermod for CUCI HIGHLITE     *   FILE 967
//*  UMISRPDJ - RECEIVE/APPLY UMISRHI usermod for PDSE allocate bug *   FILE 967
//*  UMISRPXJ - RECEIVE/APPLY UMISRPX usermod for SAMPLIB hilite    *   FILE 967
//*  UMISRUDJ - RECEIVE/APPLY UMISRUD usermod for ISRUDSL0 VSAM del *   FILE 967
//*  UMISRUUJ - RECEIVE/APPLY UMISRUU usermod for UDLIST UID(0)     *   FILE 967
//*  UMISRVCJ - RECEIVE/APPLY UMISRVC usermod for copy other DSN    *   FILE 967
//*  UMUSRCFJ - RECEIVE/APPLY UMUSRCF usermod for USRCCONF dialog   *   FILE 967
//*  USR@KYWD - Rexx to process keyword file for USRCCONF options   *   FILE 967
//*  USRCCONF - Rexx exec to drive USRCCONF dialog                  *   FILE 967
//*  USRCCVWK - Rexx exec to view USRCCONF keyword file             *   FILE 967
//*  USRCMOD  - Rexx exec to process USRCCONF keyword sections      *   FILE 967
//*  USRDEL34 - Rexx exec to process VSAM for block deletes         *   FILE 967
//*  USREDDEM - Rexx called from ISREDDE2/4 to set HILITE and NULLS *   FILE 967
//*  USREDDEX - Rexx called from ISREDDE2/4 to process HIGHLITE cmd *   FILE 967
//*  USRHCALN - Help panel for calendar options                     *   FILE 967
//*  USRHFORC - Help panel for FORCE options                        *   FILE 967
//*  USRHILIT - Rexx exec to process EDIT language highlighting     *   FILE 967
//*  USRL00   - Message member for CUCI messages                    *   FILE 967
//*  USRPCONF - USRCCONF primary panel                              *   FILE 967
//*  USRPLICM - Rexx exec to process // end-of-line comments in PLI *   FILE 967
//*  USRPMOD  - CUCI Define ISPF Settings Not in ISPCCONF panel     *   FILE 967
//*  USRPMODQ - Calendar Colors and Options                         *   FILE 967
//*  USRPMOD1 - PFKeys and PFkey Labels panel                       *   FILE 967
//*  USRPMOD2 - Calendar Colors and Options panel                   *   FILE 967
//*  USRPMOD3 - Modify MEMLIST, DSLIST, and UDLIST SRCHFOR Options  *   FILE 967
//*  USRPMOD4 - UDLIST Directory List and Mount Table Options       *   FILE 967
//*  USRPMOD8 - Panel for Browse/View/EDIT/EDSET Options            *   FILE 967
//*  USRPMOD9 - Panel for ISPF Miscellaneous Options                *   FILE 967
//*  USRUDSLI - Rexx exec to process )INIT section of ISRUDSL0      *   FILE 967
//*  USRUDSLP - Rexx exec to process )PROC section of ISRUDSL0      *   FILE 967
//*  USRUMNO2 - UDLIST Mount Table by File System/Mount Point Cols  *   FILE 967
//*  USRUMVC  - Rexx exec to prime Other Dataset on ISRUMVC panel   *   FILE 967
//*  USRUUID0 - Common exec to reset UID from 0 back to default     *   FILE 967
//*  USRUULO2 - UDLIST Directory List Column Arrangement            *   FILE 967
//*  USR0Y002 - Keyword File Member help panel                      *   FILE 967
//*  USR0Y004 - Output File Content for Keyword File help panel     *   FILE 967
//*  USR0Y007 - Output Keyword File help panel                      *   FILE 967
//*                                                                 *   FILE 967
```
