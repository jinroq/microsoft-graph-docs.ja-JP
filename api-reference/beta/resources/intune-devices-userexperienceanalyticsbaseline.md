---
title: userExperienceAnalyticsBaseline リソースの種類
description: User experience analytics baseline エンティティには、ユーザー experience analytics のスコアを比較するための基準値が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce77b448d381547bfc77b6a27e1e9935f252be5e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371528"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a>userExperienceAnalyticsBaseline リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

User experience analytics baseline エンティティには、ユーザー experience analytics のスコアを比較するための基準値が含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト userExperienceAnalyticsBaselines](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)コレクション|[UserExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[UserExperienceAnalyticsBaseline を取得する](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|[UserExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[UserExperienceAnalyticsBaseline を作成する](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|新しい[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトを作成します。|
|[UserExperienceAnalyticsBaseline の削除](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|None|[UserExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)を削除します。|
|[UserExperienceAnalyticsBaseline の更新](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|[UserExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|ユーザー experience analytics のベースラインの一意の識別子。|
|displayName|String|ユーザー experience analytics のベースラインの名前。|
|overallScore|Int32|ユーザー experience analytics のベースラインの全体的なスコア。|
|overallRegressionThreshold|Int32|ユーザー experience analytics のベースラインの全体的な回帰しきい値。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|ユーザー experience analytics デバイスのブートパフォーマンス指標。|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|ユーザー操作分析のベストプラクティスの指標。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
  "overallRegressionThreshold": 1024
}
```



