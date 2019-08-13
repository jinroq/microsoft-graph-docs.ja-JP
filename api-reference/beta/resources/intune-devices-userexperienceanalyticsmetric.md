---
title: userExperienceAnalyticsMetric リソースの種類
description: User experience analytics 指標には、ユーザーの anlaytics カテゴリの指標のスコアと単位が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 307e8c9430c5eb8d0d7bd6bc51bc772dacb6392b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371525"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a>userExperienceAnalyticsMetric リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

User experience analytics 指標には、ユーザーの anlaytics カテゴリの指標のスコアと単位が含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト userExperienceAnalyticsMetrics](../api/intune-devices-userexperienceanalyticsmetric-list.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)コレクション|[UserExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[UserExperienceAnalyticsMetric を取得する](../api/intune-devices-userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|[UserExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[UserExperienceAnalyticsMetric を作成する](../api/intune-devices-userexperienceanalyticsmetric-create.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|新しい[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)オブジェクトを作成します。|
|[UserExperienceAnalyticsMetric の削除](../api/intune-devices-userexperienceanalyticsmetric-delete.md)|None|[UserExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)を削除します。|
|[UserExperienceAnalyticsMetric の更新](../api/intune-devices-userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|[UserExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|ユーザー experience analytics 指標の一意識別子。|
|displayName|String|ユーザー experience analytics 指標の名前。|
|value|2 行分|ユーザー experience analytics 指標の値。|
|本体|String|ユーザー experience analytics 指標の単位。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetric"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "String (identifier)",
  "displayName": "String",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "String"
}
```



