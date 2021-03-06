---
title: Vertex Shader Stage
description: Vertex Shader Stage
ms.assetid: 310ef24a-7647-4f5e-b89f-a3ff330d5df4
---

# Vertex Shader Stage


The vertex shader stage processes vertices by performing operations such as transformations, skinning, and lighting. Vertex shaders always operate on a single input vertex and produce a single output vertex. This stage of the rendering pipeline must always be active.

The Direct3D runtime calls the following driver functions to create, set up, and destroy the vertex shader:

[**CalcPrivateShaderSize**](https://msdn.microsoft.com/library/windows/hardware/ff538315)

[**CreateVertexShader(D3D10)**](https://msdn.microsoft.com/library/windows/hardware/ff540720)

[**DestroyShader**](https://msdn.microsoft.com/library/windows/hardware/ff552805)

[**VsSetConstantBuffers**](https://msdn.microsoft.com/library/windows/hardware/ff570573)

[**VsSetSamplers**](https://msdn.microsoft.com/library/windows/hardware/ff570574)

[**VsSetShader**](https://msdn.microsoft.com/library/windows/hardware/ff570575)

[**VsSetShaderResources**](https://msdn.microsoft.com/library/windows/hardware/ff570576)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[display\display]:%20Vertex%20Shader%20Stage%20%20RELEASE:%20%282/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




