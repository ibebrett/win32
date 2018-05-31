---
Description: You can use the EnumFonts and EnumFontFamilies functions to enumerate the fonts that are available in a printer-compatible memory device context.
ms.assetid: d68de203-2d5f-4a28-bb57-1dda9fcb078a
title: Checking the Text Capabilities of a Device
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Checking the Text Capabilities of a Device

You can use the [EnumFonts](/windows/win32/Wingdi/nf-wingdi-enumfontsa?branch=master) and [EnumFontFamilies](/windows/win32/Wingdi/nf-wingdi-enumfontfamiliesa?branch=master) functions to enumerate the fonts that are available in a printer-compatible memory device context. You can also use the [GetDeviceCaps](/windows/win32/Wingdi/nf-wingdi-getdevicecaps?branch=master) function to retrieve information about the text capabilities of a device. By calling the [**GetDeviceCaps**](gdi.GetDeviceCaps) function with the NUMFONTS index, you can determine the minimum number of fonts supported by a printer. (An individual printer may support more fonts than specified in the return value from **GetDeviceCaps** with the NUMFONTS index.) By using the TEXTCAPS index, you can identify many of the text capabilities of the specified device.

 

 


