---
title: 詳細情報リソースの種類
description: 関連付けられている id またはシステムに関する任意の情報を含むことができるプロパティバッグ。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d3a6726c2151376d858f7962527e4dc6f9b53e7
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349412"
---
# <a name="detailsinfo-resource-type"></a>詳細情報リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

関連付けられている id またはシステムに関する任意の情報を含むことができるプロパティバッグ。 これには、プロビジョニングされているプロパティの詳細、またはソース/ターゲットシステムを含めることができます。

## <a name="properties"></a>プロパティ
[詳細**情報**] リソースは、 **ApplicationId**、 **ObjectId**、 **UPN**などの追加のプロパティを含む JSON 文字列です。 プロパティのセットは、プロビジョニングされているリソースの種類によって異なります。 この例については、「リストの内容の[概要](../api/provisioningobjectsummary-list.md)」をお示します。

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detailsInfo",
  "openType": true,
 "optionalProperties": [
 
 ],
}-->
``` json
{
  "@odata.type": "microsoft.graph.detailsInfo"
}
```
