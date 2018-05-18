---
Description: 'The CIM\_ResidesOnExtent class represents an association between a file system and the storage extent where it is located. Typically, a file system resides on a logical disk.'
audience: developer
author: 'REDMOND\\markl'
manager: 'REDMOND\\markl'
ms.assetid: '911a81e9-3032-41ff-a337-044c06d02307'
ms.prod: 'windows-server-dev'
ms.technology:
- cimwin32
- 'windows-management-instrumentation'
ms.tgt_platform: multiple
title: 'CIM\_ResidesOnExtent class'
---

# CIM\_ResidesOnExtent class

The **CIM\_ResidesOnExtent** class represents an association between a file system and the storage extent where it is located. Typically, a file system resides on a logical disk.

> \[!Important\]  
> The DMTF (Distributed Management Task Force) CIM (Common Information Model) classes are the parent classes upon which WMI classes are built. WMI currently supports only the [CIM 2.x version schemas](Http://Go.Microsoft.Com/FWLink/p/?LinkID=309367).

�

The following syntax is simplified from Managed Object Format (MOF) code and includes all of the inherited properties. Properties are listed in alphabetic order, not MOF order.

## Syntax

``` syntax
[Abstract, UUID("{10458E26-DB37-11d2-85FC-0000F8102E5F}"), AMENDMENT]
class CIM_ResidesOnExtent : CIM_Dependency
{
  CIM_FileSystem��� REF Dependent;
  CIM_StorageExtent REF Antecedent;
};
```

## Members

The **CIM\_ResidesOnExtent** class has these types of members:

-   [Properties](#properties)

### Properties

The **CIM\_ResidesOnExtent** class has these properties.

<dl> <dt>

**Antecedent**
</dt> <dd> <dl> <dt>

Data type: **CIM\_StorageExtent**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("Antecedent")
</dt> </dl>

A [**CIM\_StorageExtent**](cim-storageextent.md) that describes the storage extent.

</dd> <dt>

**Dependent**
</dt> <dd> <dl> <dt>

Data type: **CIM\_FileSystem**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("Dependent")
</dt> </dl>

A [**CIM\_FileSystem**](cim-filesystem.md) that describes the file system that is located on the storage extent.

</dd> </dl>

## Remarks

The **CIM\_ResidesOnExtent** class is derived from [**CIM\_Dependency**](cim-dependency.md).

WMI does not implement this class.

This documentation is derived from the CIM class descriptions published by the DMTF. Microsoft may have made changes to correct minor errors, conform to Microsoft SDK documentation standards, or provide more information.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista<br/>                                                                |
| Minimum supported server<br/> | Windows Server�2008<br/>                                                          |
| Namespace<br/>                | Root\\CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## See also

<dl> <dt>

[**CIM\_Dependency**](cim-dependency.md)
</dt> </dl>

�

�



