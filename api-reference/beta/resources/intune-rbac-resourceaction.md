---
title: resourceAction リソースの種類
description: リソースに対して許可され、許可されていないアクションのセット。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a07701a516c1ebdaf78e98b97be47d37b876c945
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369291"
---
# <a name="resourceaction-resource-type"></a>resourceAction リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

リソースに対して許可され、許可されていないアクションのセット。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|allowedResourceActions|文字列コレクション|許可されるアクション|
|notAllowedResourceActions|文字列コレクション|許可されていないアクション。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



