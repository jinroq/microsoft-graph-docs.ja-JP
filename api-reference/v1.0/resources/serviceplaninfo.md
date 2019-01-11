---
title: servicePlanInfo リソースの種類
description: 購読している SKU に関連付けられているサービス プランに関する情報が含まれています。subscribedSku エンティティの **servicePlans** プロパティは、**servicePlanInfo** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 837170881c7c093d26c5b59662e20e87b399a029
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845452"
---
# <a name="serviceplaninfo-resource-type"></a>servicePlanInfo リソースの種類

購読している SKU に関連付けられているサービス プランに関する情報が含まれています。[subscribedSku](subscribedsku.md) エンティティの **servicePlans** プロパティは、**servicePlanInfo** のコレクションです。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|servicePlanId|Guid|サービス プランの一意識別子。|
|servicePlanName|String|サービス プランの名前。|
|provisioningStatus|String|サービス プランのプロビジョニング状況。可能な値:<br/>Success - サービスは完全にプロビジョニングされます。<br/>Disabled - サービスは無効になっています。<br/>PendingInput - サービスはまだプロビジョニングされていません。サービスの確認を待っています。<br/>PendingActivation - サービスはプロビジョニングされていますが、管理者による明示的なアクティブ化が必要です (Intune_O365 サービスプランなど)<br/>PendingProvisioning - Microsoft では製品の SKU に新しいサービスを追加していますが、テナント側でまだアクティブ化されていません。|
|appliesTo|String|サービス プランを割り当てることができるオブジェクト。可能な値:<br/>User - サービス プランを個別のユーザーに割り当てることができます。<br/>Company - サービス プランをテナント全体に割り当てることができます。|

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
