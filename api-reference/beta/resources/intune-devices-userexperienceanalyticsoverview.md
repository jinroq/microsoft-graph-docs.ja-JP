---
title: userExperienceAnalyticsOverview リソースの種類
description: User experience analytics の概要エンティティには、全体的なスコアと、すべてのカテゴリのすべてのメトリックのスコアと洞察が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff3be73059f913943236bfce8bcb4e729a39081d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371524"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a>userExperienceAnalyticsOverview リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

User experience analytics の概要エンティティには、全体的なスコアと、すべてのカテゴリのすべてのメトリックのスコアと洞察が含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[UserExperienceAnalyticsOverview を取得する](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|[UserExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[UserExperienceAnalyticsOverview の更新](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|[UserExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|ユーザー experience analytics の概要の一意の識別子。|
|overallScore|Int32|ユーザー experience analytics 総合得点。|
|deviceBootPerformanceOverallScore|Int32|ユーザーが analytics デバイスのブートパフォーマンス全体スコアを表示します。|
|bestPracticesOverallScore|Int32|ユーザー操作分析のベストプラクティス全体のスコア。|
|insights|[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)コレクション|ユーザー experience analytics insights。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": 1024,
  "deviceBootPerformanceOverallScore": 1024,
  "bestPracticesOverallScore": 1024,
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



