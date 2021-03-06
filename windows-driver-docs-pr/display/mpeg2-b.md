---
title: MPEG2\_B
description: MPEG2\_B
ms.assetid: 7d67f0ef-a5eb-40db-9f00-6f652d28e530
keywords: ["MPEG2_B restricted profile WDK DirectX VA"]
---

# MPEG2\_B


## <span id="ddk_mpeg2_b_gg"></span><span id="DDK_MPEG2_B_GG"></span>


The MPEG2\_B restricted profile contains a set of features required for support of MPEG-2 video Main Profile and an associated DVD subpicture using front-end buffer-to-buffer subpicture blending. Alpha-blending source and destination surfaces are supported with width and height of at least 720 and 576, respectively. Support of this profile is currently encouraged, but not required.

Because the [MPEG2\_A](mpeg2-a.md) restricted profile is defined by a relaxation of the accelerator requirements of the MPEG2\_B profile, all accelerators that support the MPEG2\_B profile must support the MPEG2\_A profile.

The restrictions for MPEG2\_B are defined by the restrictions listed for MPEG2\_A, except for the following additional restrictions.

### <span id="Restrictions_on_DXVA_ConnectMode"></span><span id="restrictions_on_dxva_connectmode"></span><span id="RESTRICTIONS_ON_DXVA_CONNECTMODE"></span>Restrictions on DXVA\_ConnectMode

These values of the *bDXVA\_Func* variable must be supported: 1 (picture decoding), 2 (alpha-blend data loading), or 3 (alpha-blend combination).

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Structure Member</th>
<th align="left">Value</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><strong>wRestrictedMode</strong></p></td>
<td align="left"><p>DXVA_RESTRICTED_MODE_MPEG2_B</p></td>
</tr>
</tbody>
</table>

 

### <span id="Restrictions_on_DXVA_ConfigAlphaLoad_and_DXVA_ConfigAlphaCombine"></span><span id="restrictions_on_dxva_configalphaload_and_dxva_configalphacombine"></span><span id="RESTRICTIONS_ON_DXVA_CONFIGALPHALOAD_AND_DXVA_CONFIGALPHACOMBINE"></span>Restrictions on DXVA\_ConfigAlphaLoad and DXVA\_ConfigAlphaCombine

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Structure Member</th>
<th align="left">Value</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><strong>bConfigBlendType</strong> (DXVA_ConfigAlphaCombine)</p></td>
<td align="left"><p>Zero (front-end buffer-to-buffer blending)</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>bConfigDataType</strong> (DXVA_ConfigAlphaLoad)</p></td>
<td align="left"><p>Zero, 1, or 3 (at the accelerator's discretion)</p></td>
</tr>
</tbody>
</table>

 

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[display\display]:%20MPEG2_B%20%20%20RELEASE:%20%282/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




