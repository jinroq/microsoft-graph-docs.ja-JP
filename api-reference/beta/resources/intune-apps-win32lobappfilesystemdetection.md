---
title: win32LobAppFileSystemDetection リソースの種類
description: Win32 アプリを検出するためのファイルまたはフォルダーのパスが保存されています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 447195064a9d42db9756c71dfe08e333bf567b31
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993180"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a>win32LobAppFileSystemDetection リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 アプリを検出するためのファイルまたはフォルダーのパスが保存されています。


[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|path|String|Win32 基幹業務 (LoB) アプリを検出するためのファイルまたはフォルダーのパス|
|fileOrFolderName|String|Win32 基幹業務 (LoB) アプリを検出するためのファイルまたはフォルダーの名前|
|check32BitOn64System|Boolean|このファイルまたはフォルダーが、64ビットのシステム上の32ビット版アプリをチェックするためのものであるかどうかを示す値。|
|detectionType|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|ファイルシステムの検出の種類。 可能な値は、`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`、`doesNotExist` です。|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|ファイルまたはフォルダーの検出のための演算子。 可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。|
|detectionValue|String|ファイルまたはフォルダーの検出値|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```





