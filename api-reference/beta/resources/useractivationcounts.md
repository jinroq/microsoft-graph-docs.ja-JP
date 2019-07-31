---
title: userActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9c1dbbaa6a429a90a54f8af5f3b380ff58c86dab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007495"
---
# <a name="useractivationcounts-resource-type"></a>userActivationCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   | 説明                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | String | "Office 365 ProPlus"、"Project Client"、"Visio Pro for Office 365" などの製品の種類。 |
| lastActivatedDate | 日付   | 最新のライセンス認証の日付。       |
| ws           | Int64  | Windows のアクティブ化回数。 この番号には、Windows コンピューターのすべてのライセンス認証が含まれます。 |
| Mac               | Int64  | Mac OS のアクティブ化回数。          |
| windows10Mobile   | Int64  | Windows 10 mobile のライセンス認証回数。 |
| ios               | Int64  | IOS のアクティブ化回数。             |
| android           | Int64  | Android デバイスのアクティブ化回数。  |
| activatedOnSharedComputer   | Boolean | ユーザーが以前に共有コンピューターで製品を使用した場合は True。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```
