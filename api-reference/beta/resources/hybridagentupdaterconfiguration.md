---
title: hybridAgentUpdaterConfiguration リソースの種類
description: hybridAgentUpdaterConfiguration リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c3efdd55f432add28f6d13797a0f73b4458b966
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841249"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a>hybridAgentUpdaterConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナント管理者は、各 onPremisesPublishingProfile に対して、エージェントが更新を受信したり、エージェントに対して更新プログラムを適用したりできる時間枠を構成できます。 OnPremisesPublishingProfile に対して指定された hybridAgentUpdaterConfiguration は、その onPremisesPublishingProfile 内のすべてのエージェントに適用されます。

たとえば、onPremisesPublishingProfile のエージェントの種類が "プロビジョニング" の場合、手順は次のようになります。

1) テナント管理者は、次の n 日間、プロビジョニングエージェントの更新を受信しないように構成できます。
2) テナント管理者は、エージェントが更新を recive できる更新ウィンドウ (開始時刻と終了時刻) を構成できます。
3) テナント管理者は、allowUpdateConfigurationOverride をプロビジョニングするために updater configutration を上書きし、次に使用可能な更新プログラムを受信するために alows を有効にすることができます。

Updater 構成で指定された DateTime/Time 情報は、evaluvation 中にエージェントによって報告されるローカルタイムゾーンに変換されます。

エージェントの更新は、以下の優先順位の一覧に従います。

1) AllowUpdateConfigurationOverride が true に設定されている場合、テナントによって設定された updater 構成はスキップされ、エージェントの次のバージョンが利用可能になったとき (優先度 1) に更新が送信されます。
2) 延期更新が設定されている場合は、更新日時 (優先度 2) までエージェントは更新されません。
3) [更新] ウィンドウが設定されている場合、エージェントはその時間枠に1日24時間 (優先度 3) でのみ更新されます。
4) 有効な updater 構成がテナントによって設定されていない場合は、エージェントの次のバージョンが利用可能になったときに更新が受信されます。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|allowUpdateConfigurationOverride|Boolean|更新プログラムがスキップされ、エージェントの次のバージョンが利用可能になったときにエージェントが更新を受信するかどうかを示します。|
|deferUpdateDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|updateWindow|[updateWindow](updatewindow.md)||

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
  "baseType": null
}-->

```json
{
  "allowUpdateConfigurationOverride": true,
  "deferUpdateDateTime": "String (timestamp)",
  "updateWindow": {"@odata.type": "microsoft.graph.updateWindow"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hybridAgentUpdaterConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
