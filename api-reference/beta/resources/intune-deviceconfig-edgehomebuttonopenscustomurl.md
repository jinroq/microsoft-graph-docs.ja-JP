---
title: edgeHomeButtonOpensCustomURL リソースの種類
description: '[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。'
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f16f883622ace795628d7c34214cc4b5d12017e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989795"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a>edgeHomeButtonOpensCustomURL リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[ホーム] ボタンを表示します。[ホーム] ボタンをクリックすると、特定の URL が読み込まれます。


[EdgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ホームボタン Customurl|String|読み込む特定の URL。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```





