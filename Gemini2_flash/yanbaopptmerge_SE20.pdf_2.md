```markdown
# 20.2 Defect Amplification and Removal

• Defect Amplification Model

<table>
    <tr>
        <th colspan="1"></th>
        <th colspan="1">Defects</th>
        <th colspan="1">Detection</th>
        <th colspan="1"></th>
    </tr>
    <tr>
        <td>Errors from <br>Previous step</td>
        <td>Errors passed through</td>
        <td rowspan="3">Percent <br>Efficiency</td>
        <td rowspan="3">Errors passed <br>To next step</td>
    </tr>
    <tr>
        <td></td>
        <td>Amplified errors 1:x</td>
    </tr>
    <tr>
        <td></td>
        <td>Newly generated errors</td>
    </tr>
    <tr>
     <td colspan="4" align="center">Development step</td>
    </tr>
</table>

• Assume that an error uncovered during design will cost 1.5 monetary unit to correct. Relative to this cost, the same error uncovered just before testing commences will cost 6.5 units; during testing, 15 units; and after release, between 67 and 100 units.

• A number of studies indicate that design activities introduce between 50% - 65% of all errors during the software process. However, formal review technique have been shown to be up to 75% effective in uncovering design flaws.
```