---
title: プロビジョニングオブジェクトサマリーリソースの種類
description: Azure AD プロビジョニングサービスとそれに関連付けられているプロパティによって実行される処理を表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 26c217720692b0d36cfa0acf7537b757c92399ac
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349414"
---
# <a name="provisioningobjectsummary-resource-type"></a>プロビジョニングオブジェクトサマリーリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD プロビジョニングサービスとそれに関連付けられているプロパティによって実行される処理を表します。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [リストのプロビジョニングオブジェクトの概要](../api/provisioningobjectsummary-list.md) | [/プロビジョニングオブジェクトの概要](provisioningobjectsummary.md) | テナントで発生したすべてのプロビジョニングイベントの一覧を取得します。 |


## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|action|String|アクティビティ名または操作名 (たとえば、Create user、group にメンバーを追加) を示します。 ログに記録されたアクティビティの一覧については、「Azure AD activity list」を参照してください。|
|activityDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|changeId|String|このサイクルでのこの変更の一意の ID です。|
|cycleId|String|ジョブ反復ごとの一意の ID。|
|durationInMilliseconds|Int32|このプロビジョニングアクションが終了するのにかかった時間を示します。 ミリ秒単位で測定します。|
|id|String| アクティビティの一意の ID を示します。 これは読み取り専用の GUID です。|
|initiatedBy|[開始者](initiator.md)|このプロビジョニングを開始したユーザーの詳細。|
|jobId|String|プロビジョニングジョブ全体の一意の ID。|
|modifiedProperties|[modifiedProperty](modifiedproperty.md)コレクション|このプロビジョニングアクションでこのオブジェクトに対して変更された各プロパティの詳細。|
|説明手順|指定[手順](provisioningstep.md)のコレクション|プロビジョニングの各ステップの詳細。|
|sourceIdentity|[provisionedIdentity](provisionedidentity.md)|準備されているソースオブジェクトの詳細。|
|sourceSystem|[説明](provisioningsystemdetails.md)|準備中のオブジェクトのソースシステムの詳細。|
|statusInfo|[statusBase](statusbase.md)|プロビジョニング状態の詳細。|
|targetIdentity|[provisionedIdentity](provisionedidentity.md)|準備されているターゲットオブジェクトの詳細。|
|targetSystem|[説明](provisioningsystemdetails.md)|プロビジョニング対象のオブジェクトのターゲットシステムの詳細。|
|tenantId|String|一意の Azure AD テナント ID。|

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "action": "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
