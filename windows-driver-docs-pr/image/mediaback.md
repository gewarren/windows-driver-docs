---
title: MediaBack element
description: The optional MediaBack element contains all parameters that are specific to the scanning of the back side of the physical media.
ms.assetid: d736c76f-7ea7-49ca-9ad9-df35924fc7b4
keywords: ["MediaBack element Imaging Devices"]
topic_type:
- apiref
api_name:
- wscn MediaBack
api_type:
- Schema
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# MediaBack element


The optional **MediaBack** element contains all parameters that are specific to the scanning of the back side of the physical media.

Usage
-----

``` syntax
<wscn:MediaBack>
  child elements
</wscn:MediaBack>
```

Attributes
----------

There are no attributes.

## Child elements


<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[<strong>ColorProcessing</strong>](colorprocessing.md)</p></td>
</tr>
<tr class="even">
<td><p>[<strong>Resolution</strong>](resolution.md)</p></td>
</tr>
<tr class="odd">
<td><p>[<strong>ScanRegion</strong>](scanregion.md)</p></td>
</tr>
</tbody>
</table>

## Parent elements


<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[<strong>MediaSides</strong>](mediasides.md)</p></td>
</tr>
</tbody>
</table>

Remarks
-------

The **MediaBack** element is valid only when the scanner supports duplex scanning and the current input source, which is defined in the [**InputSource**](inputsource.md) element, is **ADFDuplex**.

If the **MediaBack** element does not contain a [**ScanRegion**](scanregion.md) element, the WSD Scan Service should use 0 as the offsets and the width and height of the [**InputMediaSize**](inputmediasize.md), if given. If **ScanRegion** is missing and **InputMediaSize** is not specified or cannot be determined by the scan device, you can determine the implementation.

If the input source is **ADFDuplex** and the **MediaBack** element is missing, all parameters that are specified in [**MediaFront**](mediafront.md) will apply to the back side scanning as well.

## <span id="see_also"></span>See also


[**ColorProcessing**](colorprocessing.md)

[**InputMediaSize**](inputmediasize.md)

[**InputSource**](inputsource.md)

[**MediaFront**](mediafront.md)

[**MediaSides**](mediasides.md)

[**Resolution**](resolution.md)

[**ScanRegion**](scanregion.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bimage\image%5D:%20MediaBack%20element%20%20RELEASE:%20%2811/8/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





