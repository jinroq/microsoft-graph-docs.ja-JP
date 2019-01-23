---
title: win32LobAppPowerShellScriptDetection リソースの種類
description: Win32 アプリケーションを検出する PowerShell スクリプトのプロパティが含まれています
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5c02228589042d0abf36c34c5818c5a4610514e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399641"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>win32LobAppPowerShellScriptDetection リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 アプリケーションを検出する PowerShell スクリプトのプロパティが含まれています


[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|enforceSignatureCheck|Boolean|署名チェックを強制するかどうかを示す値|
|runAs32Bit|Boolean|このスクリプトは 32 ビットとして実行するかどうかを示す値|
|scriptContent|String|Base64 にエンコードされた Win32 基幹業務 (LoB) アプリケーションを検出するためにスクリプトの内容|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```




