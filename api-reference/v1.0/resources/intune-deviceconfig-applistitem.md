---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb81c8edfae3f9b33be4636e9fd7f15fa758e789
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253079"
---
# <a name="applistitem-resource-type"></a>appListItem リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理対象アプリケーションの一覧にあるアプリを表します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|name|String|アプリケーション名|
|発行元|String|アプリケーションの発行元|
|appStoreUrl|String|アプリケーションのストア URL|
|appId|文字列型 (String)|アプリケーションのアプリケーションまたはバンドルの識別子|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



