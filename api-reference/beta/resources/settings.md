---
title: リソースの種類の設定
description: ユーザーが analytics API を使用するために必要な現在の設定。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a7d534aecf6e7ffa427ea175ae06e2b1820435b2
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450794"
---
# <a name="settings-resource-type"></a>リソースの種類の設定

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Analytics API を使用するユーザーに対して現在必要な設定を表します。

Analytics API が結果を返すようにするために、ユーザーには、Microsoft Graph 用に有効になっているクラウドホスト型のメールボックスがあり、有効な MyAnalytics ライセンスを持っており、MyAnalytics を使用するようにオプトインされている必要があります。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
[設定を取得する](../api/useranalytics-get-settings.md) | [設定](settings.md) | ユーザーに対して次のプロパティ設定を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|hasGraphMailbox|Boolean|ユーザーのプライマリメールボックスがクラウドでホストされており、Microsoft Graph に対して有効になっているかどうかを指定します。|
|hasLicense|Boolean|ユーザーが MyAnalytics ライセンスが割り当てられているかどうかを指定します。|
|hasOptedOut|Boolean|ユーザーが MyAnalytics をオプトアウトしたかどうかを指定します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settings",
  "baseType": null
}-->

```json
{
  "hasGraphMailbox": true,
  "hasLicense": true,
  "hasOptedOut": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->