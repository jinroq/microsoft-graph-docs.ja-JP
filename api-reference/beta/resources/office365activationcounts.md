---
title: office365ActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7bc21be693a5c68ecd5c6a1e4e44d53c9261acdb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505467"
---
# <a name="office365activationcounts-resource-type"></a>office365ActivationCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   | 説明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportrefreshdate | Date   | コンテンツの最新の日付。          |
| productType       | String | "office 365 ProPlus"、"Project Client"、"Visio Pro for Office 365" などの製品の種類。 |
| ws           | Int64  | Windows のアクティブ化回数。 この番号には、Windows コンピューターのすべてのライセンス認証が含まれます。 |
| Mac               | Int64  | Mac OS のアクティブ化回数。          |
| android           | Int64  | Android デバイスのアクティブ化回数。  |
| ios               | Int64  | iOS のアクティブ化回数。             |
| windows10Mobile   | Int64  | Windows 10 mobile のライセンス認証回数。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
