---
title: servicePlanInfo リソースの種類
description: 購読済み SKU に関連付けられているサービスプランに関する情報が含まれます。 SubscribedSku **** エンティティの serviceplans プロパティは、 **serviceplans info**のコレクションです。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5aa721ce300338e68ca284f4f4ed11b1f66faad2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034385"
---
# <a name="serviceplaninfo-resource-type"></a>servicePlanInfo リソースの種類

購読済み SKU に関連付けられているサービスプランに関する情報が含まれます。 [SubscribedSku](subscribedsku.md)エンティティの**serviceplans**プロパティは、 **serviceplans info**のコレクションです。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|servicePlanId|Guid|サービス プランの一意識別子。|
|Serviceplan の名前|String|サービス プランの名前。|
|プロビジョニング状態|String|サービス プランのプロビジョニング状況。 可能な値:<br/>"Success"-サービスは完全にプロビジョニングされています。<br/>[無効]-サービスが無効になっています。<br/>"PendingInput"-サービスはまだ準備されていません。サービスの確認を待っている。<br/>"PendingActivation"-サービスはプロビジョニングされていますが、管理者による明示的なライセンス認証が必要です (たとえば、Intune_O365 Service plan)。<br/>"PendingProvisioning"-Microsoft では、製品 SKU に新しいサービスが追加されていますが、テナントではまだアクティブ化されていません。|
|appliesTo|String|サービスプランを割り当てることができるオブジェクトです。 可能な値:<br/>"User"-サービスプランを個々のユーザーに割り当てることができます。<br/>"Company"-サービスプランは、テナント全体に割り当てることができます。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
