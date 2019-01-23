---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bfc7815e7f893294a72b88f67054702e1fb7347e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399263"
---
# <a name="managedappstatusraw-resource-type"></a>managedAppStatusRaw リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

組織アプリの保護と構成についての型指定されていない進捗レポートを表します。


[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedAppStatusRaws のリスト](../api/intune-mam-managedappstatusraw-list.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedAppStatusRaw の取得](../api/intune-mam-managedappstatusraw-get.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|進捗レポートのフレンドリ名。 [managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します|
|id|String|エンティティのキー。 [managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します|
|version|String|エンティティのバージョン。 [managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します|
|content|[Json](../resources/intune-mam-json.md)|進捗レポートの内容。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```




