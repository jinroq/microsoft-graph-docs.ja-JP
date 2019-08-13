---
title: configurationManagerClientInformation リソースの種類
description: SCCM から同期された Configuration manager クライアント情報
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae7d36b353b989d4256294872fba4c4f225d2668
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371542"
---
# <a name="configurationmanagerclientinformation-resource-type"></a>configurationManagerClientInformation リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

SCCM から同期された Configuration manager クライアント情報

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|clientIdentifier|String|SCCM からの Configuration Manager クライアント Id|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String"
}
```



