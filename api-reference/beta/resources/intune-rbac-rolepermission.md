---
title: rolePermission リソースの種類
description: 各役割に対して許可されるアクセス許可と許可されないアクセス許可を決定する ResourceActions のセットが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c612e4c6201a3016b866eddc7e5e52d0b3238306
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369214"
---
# <a name="rolepermission-resource-type"></a>rolePermission リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

各役割に対して許可されるアクセス許可と許可されないアクセス許可を決定する ResourceActions のセットが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|actions|文字列コレクション|許可されたアクション-非推奨|
|resourceActions|[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション|それぞれ許可され、許可されていないアクセス許可のセットが含まれているリソースアクション。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```



