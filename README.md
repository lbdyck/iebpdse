# IEBPDSE is an ISPF dialog that front-ends the IBM IEBPDSE utility.

It is a fully self-contained application with the ISPF panel included
inline in the REXX code.

To use it the IEBPDSE exec must be copied into a library in your
SYSEXEC, or SYSPROC, allocations.

Then invoke it using TSO %IEBPDSE

 ## Function:  
 
 Invoke the IBM IEBPDSE utility to try to repair a PDSE (or at least report on it)

 ## Syntax:    
            %iebpdse pdse-dsname iebpdse-parms

            pdse-dsname is the pdse data set name
            iebpdse-parms are processing parms:

            ANAL      - PDSE analysis
            A           Default enabled
            BYPASS    - Bypass the IEBPDSE prompt panel
            B           Default disabled
            DUMP      - System Dump if PDSE is corrupt
            D           Default disabled
            FLUSH     - Flush PDSE pages before analysis
            F           Default enabled
            NOANAL    - Do NOT do an analysis
            NOA         Default disabled
            NODUMP    - Do NOT take a System Dump
            NOD         Default enabled
            NOFLUSH   - Do NOT flush any PDSE pages
            NOF         Default enabled
            PERF      - Do a Pending Delete process
            P           Default enabled
