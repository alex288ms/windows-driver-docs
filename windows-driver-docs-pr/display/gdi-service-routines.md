---
title: GDI Service Routines
description: GDI Service Routines
ms.assetid: ca4fbb84-33a8-498f-8549-c8aaf87429fd
keywords: ["GDI WDK Windows 2000 display , service routines", "graphics drivers WDK Windows 2000 display , service routines", "drawing WDK GDI , service routines", "service routines WDK GDI"]
---

# GDI Service Routines


## <span id="ddk_gdi_service_routines_gg"></span><span id="DDK_GDI_SERVICE_ROUTINES_GG"></span>


GDI exports many service routines, whose names have the form **Eng***Xxx*. The driver dynamically links to *win32k.sys* to directly access these routines. GDI service routines include surface management, rendering simulations, and path, palette, font, and text services. These services are discussed in detail in [GDI Support Services](gdi-support-services.md).

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[display\display]:%20GDI%20Service%20Routines%20%20RELEASE:%20%282/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




