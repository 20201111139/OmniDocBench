| Constant                   | Value   | Meaning                                                                            |
|----------------------------|---------|------------------------------------------------------------------------------------|
| kAlertStdAlertOKButton     |         | The OK push button. The default text for this push button is ~OK                   |
| kAlertStdAlertCancelButton |         | The Cancel push button (optional). The default text for this push button is Cancel |
| kAlertStdAlertOtherButton  |         | A third push button (optional). The default text for this push button is           |
| kAlertStdAlertHelpButton   |         | The Help push button (optional).                                                   |

## Creating Dialog Boxes

Dialog boxes may be created in one of two ways:

- Using the function GetNewDialog which takes descriptive information about the dialog from dialog ('DLOG and extended dialog ('dlgx ) resources. The resource ID of the DLOG and resources must be the same; and is passed in the first parameter of this function.
- NewDialog, NewColorDialog, NewFeaturesDialog, which take descriptive information passed in the parameters of those functions. Using

## Historical Note

The extended dialog resource and the NewFeaturesDialog function were introduced with OS 8 and the Appearance Manager. NewFeaturesDialog should be used to create Appearance-compliant dialogs. Unlike NewDialog and NewColorDialog, it has parameter containing the same flags you would set in an extended resource flags dialog

If NULL is specified as the second parameter in the GetNewDialog call, GetNewDialog itself creates a nonrelocatable block for the when the user dismisses the dialog   However; in order to avoid fragmentation effects, you should ordinarily allocate your own memory for modeless dialog box dialog structures (just as you would for window structure) and specify the pointer to that memory block in the second parameter of the GetNewDialog call. heap

Regardless of which method is used to create the dialog; a dialog structure and a window structure will be created, and pointer to the dialog structure will be returned to the calling function.

## The Structure Dialog

The dialog structure created by the  GetNewDialog call is defined by the data type DialogRecord:

struct DialogRecord

```
WindowRecord window ; Dialog window record Handle items ; Item Iist resource TEHandle Current editable text item SInt16 editField; Editable text item number minus SInt16 editOpen; (Used internally SInt16 aDefItem ; Default push button item number
```

typedef struct DialogRecord DialogRecord;

typedef DialogRecord #DialogPeek ;

Note that the dialog   structure  includes window structure   field. The Dialog   Manager sets the windowKind field of this window structure to kDialogWindowKind.