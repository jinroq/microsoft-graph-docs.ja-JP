---
title: rolePermission リソースの種類
description: 各役割に対して許可されるアクセス許可と許可されないアクセス許可を決定する ResourceActions のセットが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cbe41bae81d165d0800a5184e1f7babedebc09d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993523"
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





