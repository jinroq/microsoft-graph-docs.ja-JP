---
title: win32LobAppRegistryDetection リソースの種類
description: Win32 アプリを検出するためのレジストリプロパティが含まれています
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c249a21075a2d2647fbb0cbcc53bf7c541a155f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534480"
---
# <a name="win32lobappregistrydetection-resource-type"></a>win32LobAppRegistryDetection リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 アプリを検出するためのレジストリプロパティが含まれています


[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|check32BitOn64System|ブール値|このレジストリパスが、64ビットシステムの32ビットアプリをチェックするためのものであるかどうかを示す値。|
|キーパス|String|Win32 基幹業務 (LoB) アプリを検出するためのレジストリキーのパス|
|valueName|String|レジストリ値の名前|
|detectionType|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|レジストリデータ検出の種類。 可能な値は `notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version` です。|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|レジストリデータを検出するための演算子。 可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。|
|detectionValue|String|レジストリの検出値|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```





