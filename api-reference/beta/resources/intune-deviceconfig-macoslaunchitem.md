---
title: macOSLaunchItem リソースの種類
description: MacOS 起動アイテムの一覧にあるアプリを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ffdd1d491f56051430b57c6cc3319279b31bcad
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946064"
---
# <a name="macoslaunchitem-resource-type"></a>macOSLaunchItem リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS 起動アイテムの一覧にあるアプリを表します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|path|String|起動項目へのパス。|
|と|Boolean|[ユーザーとグループ] リストのアイテムを非表示にするかどうかを指定します。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLaunchItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLaunchItem",
  "path": "String",
  "hide": true
}
```




