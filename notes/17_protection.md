# PROTECTION

## Sheet

To prevent modifying some or all cells in sheet. Every cell by default has **Locked** property set.

1. Highlight ones that can be modified.
2. Right-click and select **Format Cells** (**⌘ 1**).
3. Go to **Protection** tab. Uncheck **Locked**.
   ![Format Cells Protection](/assets/format-cells-protection.png)
4. **Review &rarr; Protect Sheet**. Enter password (so can't unprotect arbitrarily) and select options.
   ![Protect Sheet](/assets/protect-sheet.png)

Won't be allowed to modify any other cells.

## Workbook (Structure)

**Review &rarr; Protect Workbook**
![Protect Workbook](/assets/protect-workbook.png)

Disallows modifying sheet name (or any other sheet property), ensuring formulas involving sheet names won't break.

Click same button again and enter password (if set up) to unprotect workbook.

## Workbook (Password)

To add password for opening workbook, **File &rarr; Passwords**.
![File Passwords](/assets/file-passwords.png)
