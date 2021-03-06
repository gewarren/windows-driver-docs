---
title: CompressionQualityFactorSupported element
description: The required CompressionQualityFactorSupported element specifies the range of compression quality factors that the scan device supports.
ms.assetid: f82ae450-b948-463e-a6a8-aaea0575ddb9
keywords: ["CompressionQualityFactorSupported element Imaging Devices"]
topic_type:
- apiref
api_name:
- wscn CompressionQualityFactorSupported
api_type:
- Schema
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# CompressionQualityFactorSupported element


The required **CompressionQualityFactorSupported** element specifies the range of compression quality factors that the scan device supports.

Usage
-----

``` syntax
<wscn:CompressionQualityFactorSupported>
  child elements
</wscn:CompressionQualityFactorSupported>
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
<td><p>[<strong>MaxValue</strong>](maxvalue.md)</p></td>
</tr>
<tr class="even">
<td><p>[<strong>MinValue</strong>](minvalue.md)</p></td>
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
<td><p>[<strong>DeviceSettings</strong>](devicesettings.md)</p></td>
</tr>
</tbody>
</table>

Remarks
-------

The compression quality factor is an integer value that you use for a lossy compression type to determine the amount of acceptable image loss during compression. The higher the requested fidelity, the larger the resulting file size will be.

[**MinValue**](minvalue.md)[**MaxValue**](maxvalue.md)

The minimum and maximum compression quality factors that the scan device supports are specified in the [**MinValue**](minvalue.md) and [**MaxValue**](maxvalue.md) elements, respectively. **MinValue** and **MaxValue** must be integers from 1 through 100. A value of 100 means that the device should use the least amount of compression that it supports to produce the highest quality image. Currently, JPEG compression is the only supported lossy compression type.

## <span id="see_also"></span>See also


[**DeviceSettings**](devicesettings.md)

[**MaxValue**](maxvalue.md)

[**MinValue**](minvalue.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bimage\image%5D:%20CompressionQualityFactorSupported%20element%20%20RELEASE:%20%2811/8/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





