---
title: Tracelog
description: Tracelog (Tracelog.exe) is an event tracing controller that runs in a Command Prompt window. This section describes Tracelog, explains its command syntax, and provides practical examples for its use.
ms.assetid: aa3c144d-260b-44d2-b41c-d18be40ba541
keywords: ["Tracelog WDK", "software tracing WDK , Tracelog", "tracing WDK , Tracelog", "event tracing controller WDK Tracelog", "trace session management WDK Tracelog"]
---

# Tracelog


Tracelog (Tracelog.exe) is an event tracing controller that runs in a Command Prompt window. This section describes Tracelog, explains its command syntax, and provides practical examples for its use.

<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Where can I get Tracelog?</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Tracelog (Tracelog.exe) is included when you install the WDK, Visual Studio, and the Windows SDK for desktop apps. For information about downloading the kits, see [Windows Hardware Downloads](http://go.microsoft.com/fwlink/p/?linkid=290798).</p>
<p><strong>Windows Driver Kit (WDK) 8</strong> (installation path)</p>
<p>%WindowsSdkDir%\tools\x64\tracelog.exe</p>
<p>%WindowsSdkDir%\tools\x86\tracelog.exe</p>
<p><strong>Windows Driver Kit (WDK) 8.1</strong> (installation path)</p>
<p>%WindowsSdkDir%\bin\x64\tracelog.exe</p>
<p>%WindowsSdkDir%\bin\x86\tracelog.exe</p>
<div class="alert">
<strong>Note</strong>  The Visual Studio environment variable, %WindowsSdkDir%, represents the path to the Windows kits directory where the kits are installed, for example, C:\Program Files (x86)\Windows Kits\8.1.
</div>
<div>
 
</div></td>
</tr>
</tbody>
</table>

 

## <span id="What_you_can_do_with_Tracelog"></span><span id="what_you_can_do_with_tracelog"></span><span id="WHAT_YOU_CAN_DO_WITH_TRACELOG"></span>What you can do with Tracelog


You can use Tracelog in a Command Prompt window as an event tracing controller.

**Note**  To control a trace session on Windows Server 2003 and later versions of Windows, you must be a member of the Performance Log Users group or the Administrators group on the computer (**Run as administrator**).

 

Tracelog features include:

-   Starts and stops [trace sessions](trace-session.md), including private trace sessions, [NT Kernel Logger trace sessions](nt-kernel-logger-trace-session.md), and [Global Logger trace sessions](global-logger-trace-session.md)

-   Configures and changes the properties of trace sessions

-   Enables and disables [trace providers](trace-provider.md)

-   Flushes trace session buffers

-   Lists running (real-time) trace sessions

-   Lists [registered trace providers](registered-provider.md)

-   Measures time spent in deferred procedure calls (DPCs) and interrupt service routines (ISRs)

Tracelog produces an event trace log (.etl) file that contains the trace messages generated by the provider during the trace session. The messages are stored in binary format in the file. To display the trace messages in a readable format, use [TraceView](traceview.md) or [Tracefmt](tracefmt.md).

Tracelog controls kernel-mode and private (user-mode) trace sessions, and special sessions such as the [NT Kernel Logger trace session](nt-kernel-logger-trace-session.md) and the [Global Logger trace session](global-logger-trace-session.md).

Tracelog runs on Windows 2000 and later versions of Windows.

Many of the features of Tracelog are also available in [TraceView](traceview.md), a tool included in the Windows Driver Kit (WDK) that has a graphical user interface in addition to a command-line interface.

## <span id="in_this_section"></span>In this section


-   [**Tracelog Command Syntax**](tracelog-command-syntax.md)
-   [Tracelog Displays](tracelog-displays.md)
-   [Tracelog Examples](tracelog-examples.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[devtest\devtest]:%20Tracelog%20%20RELEASE:%20%2811/17/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




