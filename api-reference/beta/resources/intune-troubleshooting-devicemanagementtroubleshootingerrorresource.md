---
title: devicemanagementのトラブルシューティング errorresource リソースの種類
description: 'オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25d97a6d085b9f1b7e0b1ab73361be3ac7ae74d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155560"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>devicemanagementのトラブルシューティング errorresource リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|text|String|まだ文書化されていません|
|link|String|web リソースへのリンク。 次のいずれかのフォーマッタを含めることができます。 {{UPN}}、{{deviceguid}}、{{userguid}}|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```




