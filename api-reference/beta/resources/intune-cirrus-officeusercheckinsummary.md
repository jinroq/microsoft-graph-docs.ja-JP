---
title: officeUserCheckinSummary リソースの種類
description: テナントのチェックイン統計を記述するエンティティ。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b74d7508c9ef3b1d7183c806783e567cb75859ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526385"
---
# <a name="officeusercheckinsummary-resource-type"></a>officeUserCheckinSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

テナントのチェックイン統計を記述するエンティティ。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|succeededUserCount|Int32|過去3か月間の成功したユーザーチェックインの合計数。|
|failedUserCount|Int32|過去3か月間のユーザーチェックに失敗した合計数。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



