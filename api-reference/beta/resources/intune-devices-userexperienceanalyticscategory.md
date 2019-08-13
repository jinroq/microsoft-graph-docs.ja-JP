---
title: userExperienceAnalyticsCategory リソースの種類
description: User experience analytics category エンティティには、カテゴリのさまざまな指標のスコアと洞察が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c04f2caaa7b9ee6c093a58e4c8123250113b3a9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329647"
---
# <a name="userexperienceanalyticscategory-resource-type"></a>userExperienceAnalyticsCategory リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

User experience analytics category エンティティには、カテゴリのさまざまな指標のスコアと洞察が含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[UserExperienceAnalyticsCategory を取得する](../api/intune-devices-userexperienceanalyticscategory-get.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|[UserExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[UserExperienceAnalyticsCategory の更新](../api/intune-devices-userexperienceanalyticscategory-update.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|[UserExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|ユーザー experience analytics カテゴリの一意識別子。|
|displayName|String|ユーザー experience analytics カテゴリの名前。|
|overallScore|Int32|ユーザー experience analytics カテゴリの全体的なスコア。|
|insights|[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)コレクション|ユーザー experience analytics カテゴリの洞察。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|metricValues|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)コレクション|ユーザー experience analytics カテゴリのメトリック値。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```



