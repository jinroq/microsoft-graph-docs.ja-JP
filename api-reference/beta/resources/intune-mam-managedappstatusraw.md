---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7c609c8ac1a228be588c5bdfe93cca7d42069da
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781541"
---
# <a name="managedappstatusraw-resource-type"></a>managedAppStatusRaw リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

組織アプリの保護と構成についての型指定されていない進捗レポートを表します。


[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedAppStatusRaws のリスト](../api/intune-mam-managedappstatusraw-list.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get managedAppStatusRaw](../api/intune-mam-managedappstatusraw-get.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。|

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





