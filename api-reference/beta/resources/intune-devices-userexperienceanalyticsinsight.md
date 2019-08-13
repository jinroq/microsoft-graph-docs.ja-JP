---
title: userExperienceAnalyticsInsight リソースの種類
description: ユーザーの分析に関する分析情報は、ユーザー環境分析のスコアを向上させるための推奨事項です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 36277b147e7eabc6f28aef3877538ebbc429f381
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341234"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a>userExperienceAnalyticsInsight リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザーの分析に関する分析情報は、ユーザー環境分析のスコアを向上させるための推奨事項です。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|userExperienceAnalyticsMetricId|String|ユーザー experience analytics に関する洞察の一意の識別子。|
|insightId|String|ユーザー experience analytics に関する洞察の一意の識別子。|
|value|[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)コレクション|ユーザーが分析する分析に関する洞察の価値。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
  "userExperienceAnalyticsMetricId": "String",
  "insightId": "String",
  "value": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble"
    }
  ]
}
```



