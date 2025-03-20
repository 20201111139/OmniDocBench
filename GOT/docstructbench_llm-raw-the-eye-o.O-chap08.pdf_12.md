<table border=1>
<tr>
<td>Constant</td>
<td>Value</td>
<td>Meaning</td>
</tr>
</table>\section*{Creating Dialog Boxes}
Dialog boxes may be created in one of two ways:
- Using the function GetNewDialog, which takes descriptive information about the dialog from dialog ("DL06") and extended dialog ("dIg \(\mathrm{x}\) ") resources. The resource ID of the "DL06" and "dIg \(\mathrm{x}\) " resources must be the same, and is passed in the first parameter of this function.
- \(\quad\) Using NewDialog, NewColorDiaLog, or NewFeaturesDiaLog, which take descriptive information passed in the parameters of those functions.
\section*{Historical Note}
The extended dialog resource and the NewFeaturesDiaLog function were introduced with OS 8 and the Appearance Manager. NewFeaturesDiaLog should be used to create Appearance-compliant dialogs. Unlike NewDialog and NewColorDiaLog, it has a flags parameter containing the same flags you would set in an extended dialog resource.
If NULL is specified as the second parameter in the GetNewDialog call, GetNewDiaLog itself creates a nonrelocatable block for the dialog structure. Passing NULL is appropriate for modal and movable modal dialog boxes because you should dispose of the dialog box, and hence the associated dialog structure, when the user dismisses the dialog. However, in order to avoid heap fragmentation effects, you should ordinarily allocate your own memory for modelless dialog box dialog structures (just as you would for a window structure) and specify the pointer to that memory block in the second parameter of the GetNewDiaLog call.
Regardless of which method is used to create the dialog, a dialog structure and a window structure will be created, and a pointer to the dialog structure will be returned to the calling function.
\section*{The Dialog Structure}
The dialog structure created by the GetNewDiaLog call is defined by the data type DiaLogRecord:

Note that the dialog structure includes a window structure field. The Dialog Manager sets the windowkind field of this window structure to kDiaLogWindowkind.