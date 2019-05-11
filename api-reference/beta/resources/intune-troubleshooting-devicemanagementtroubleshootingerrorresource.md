---
title: Devicemanagementのトラブルシューティング Errorresource リソースの種類
description: 'オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。'
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 712832420b556517be8ef053cc6cd292acfeed86
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939848"
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

## <a name="relationships"></a>関係
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




