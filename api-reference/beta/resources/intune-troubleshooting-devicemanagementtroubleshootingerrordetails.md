---
title: Devicemanagementトラブルシューティングエラーの詳細リソースの種類
description: エラーとその修復に関する詳細情報を含むオブジェクト。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4759665d96940d806e283cd5b59caed7fee63d32
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988196"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a>Devicemanagementトラブルシューティングエラーの詳細リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エラーとその修復に関する詳細情報を含むオブジェクト。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|context|String|まだ文書化されていません|
|エラー|String|まだ文書化されていません|
|failureDetails|String|問題の詳細な説明。|
|修復|String|この問題を修復する方法の詳細な説明。|
|リソース|[Devicemanagementのトラブルシューティング Errorresource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)コレクション|このエラーについての有用なドキュメントへのリンクを示します。|

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





