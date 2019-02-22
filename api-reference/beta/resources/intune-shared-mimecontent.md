---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f446983d5dfe101c89171baa776b32759726f279
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161657"
---
# <a name="mimecontent-resource-type"></a>mimeContent リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

汎用 MIME コンテンツのプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|type|String|コンテンツ MIME の種類を示します。|
|value|バイナリ|実際のコンテンツを含むバイト配列です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```




