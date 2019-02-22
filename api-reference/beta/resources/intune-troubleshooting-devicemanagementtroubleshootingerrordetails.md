---
title: devicemanagementトラブルシューティングエラーの詳細リソースの種類
description: エラーとその修復に関する詳細情報を含むオブジェクト。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08ad43b717a5e08229054bc10aa81a0786f4e344
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142582"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a>devicemanagementトラブルシューティングエラーの詳細リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エラーとその修復に関する詳細情報を含むオブジェクト。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|context|String|まだ文書化されていません|
|failure|String|まだ文書化されていません|
|failuredetails|String|問題の詳細な説明。|
|修復|String|この問題を修復する方法の詳細な説明。|
|resources|[devicemanagementのトラブルシューティング errorresource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)コレクション|このエラーについての有用なドキュメントへのリンクを示します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




