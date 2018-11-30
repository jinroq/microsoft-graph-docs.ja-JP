---
title: office365ActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: e53a979ac627735ef63a24e1823d83f4c9fe9f7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073094"
---
# <a name="office365activationcounts-resource-type"></a>office365ActivationCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   | 説明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | コンテンツの最新の日付。          |
| productType       | String | 「Office 365 用リソース"、「プロジェクト クライアント」など、製品の種類または"Office 365"の Visio Pro です。 |
| windows           | Int64  | [Windows のライセンス認証の数です。 この数値には、任意の Windows コンピューターですべてのアクティブ化が含まれます。 |
| Mac               | Int64  | Mac OS のライセンス認証の数です。          |
| android           | Int64  | Android デバイス上のアクティブ化の数。  |
| ios               | Int64  | IOS のライセンス認証の数です。             |
| windows10Mobile   | Int64  | ライセンス認証カウント 10 の Windows のモバイルです。 |

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
