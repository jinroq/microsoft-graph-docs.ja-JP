---
title: Devicemanagementのトラブルシューティング Errorresource リソースの種類
description: 'オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。'
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6aa8493638a4cdcc486cce0a0036328a2ff359e1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988189"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>Devicemanagementのトラブルシューティング Errorresource リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|text|String|まだ文書化されていません|
|link|String|Web リソースへのリンク。 次のいずれかのフォーマッタを含めることができます。 {{UPN}}、{{DeviceGUID}}、{{UserGUID}}|

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





