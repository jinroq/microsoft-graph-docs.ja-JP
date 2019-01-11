---
title: win32LobAppFileSystemDetection リソースの種類
description: Win32 アプリケーションを検出するためにファイルまたはフォルダーのパスが含まれています
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 13a994d39ec42ddcb45bc71aac739864a6ef6dc4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849274"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a>win32LobAppFileSystemDetection リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Win32 アプリケーションを検出するためにファイルまたはフォルダーのパスが含まれています

[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|path|String|Win32 基幹業務 (LoB) アプリケーションを検出するためにファイルまたはフォルダーのパス|
|fileOrFolderName|String|Win32 基幹業務 (LoB) アプリケーションを検出するためにファイルまたはフォルダーの名前|
|check32BitOn64System|ブール型|このファイルまたはフォルダーは、64 ビット システムで 32 ビット アプリケーションをチェックするかどうかを示す値|
|detectionType|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|ファイル システムの検出の種類。 使用可能な値: `notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`。|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|ファイルまたは fodler を検出するための演算子です。 可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。|
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





