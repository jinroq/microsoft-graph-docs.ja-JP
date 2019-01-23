---
title: deviceManagementTroubleshootingErrorDetails リソースの種類
description: エラーとその修復に関する詳細情報を含むオブジェクトです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9cdda64170afc739c23f1b258e5f2f1b31158662
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430334"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a>deviceManagementTroubleshootingErrorDetails リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エラーとその修復に関する詳細情報を含むオブジェクトです。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|context|String|まだ文書化されていません|
|failure|String|まだ文書化されていません|
|failureDetails|String|失敗の原因の詳細な説明です。|
|改善計画|String|この問題を修正する方法についての詳細な説明です。|
|resources|[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)コレクション|この障害に関する役に立つドキュメントにリンクします。|

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




