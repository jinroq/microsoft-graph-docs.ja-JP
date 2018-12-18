---
title: userActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: dkershaw10
ms.openlocfilehash: 396f6182d000df6d701e8c0cbad3dd02a258c4c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322919"
---
# <a name="useractivationcounts-resource-type"></a>userActivationCounts リソースの種類

## <a name="properties"></a>Properties

| プロパティ          | 種類   | 説明                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | String | 「Office 365 用リソース"、「プロジェクト クライアント」など、製品の種類または"Office 365"の Visio Pro です。 |
| lastActivatedDate | 日付   | 最新のアクティブ化の日付です。       |
| windows           | Int64  | [Windows のライセンス認証の数です。 この数値には、任意の Windows コンピューターですべてのアクティブ化が含まれます。 |
| Mac               | Int64  | Mac OS のライセンス認証の数です。          |
| windows10Mobile   | Int64  | ライセンス認証カウント 10 の Windows のモバイルです。 |
| ios               | Int64  | IOS のライセンス認証の数です。             |
| android           | Int64  | Android デバイス上のアクティブ化の数。  |
| activatedOnSharedComputer   | ブール型 | ユーザーが共有する前にコンピューターに製品を使用する場合は true にします。 |

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
