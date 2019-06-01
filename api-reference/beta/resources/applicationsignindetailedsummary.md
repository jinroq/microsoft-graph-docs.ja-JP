---
title: applicationSignInDetailedSummary リソースの種類-Microsoft Graph API
description: アプリケーションサインインの詳細な概要を表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4d4fcd00e305c19f1d445738a22125cc8addc143
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657638"
---
# <a name="applicationsignindetailedsummary-resource-type"></a>applicationSignInDetailedSummary リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションサインインの詳細な概要を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [ApplicationSignInDetailedSummary を取得する](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | **ApplicationSignInDetailedSummary**オブジェクトのプロパティとリレーションシップを読み取ります。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|aggregatedEventDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|appDisplayName|String|ユーザーがサインインしたアプリケーションの名前。|
|appId|String|ユーザーがサインインしたアプリケーションの ID。|
|id|文字列| サインインアクティビティを表す一意の ID。|
|signInCount|Int64|アプリケーションによって作成されたサインインの数。|
|status|[signInStatus](signinstatus.md)|サインイン状態の詳細。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
}-->

```json
{
  "aggregatedEventDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "id": "String (identifier)",
  "signInCount": 1024,
  "status": {"@odata.type": "microsoft.graph.signInStatus"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
