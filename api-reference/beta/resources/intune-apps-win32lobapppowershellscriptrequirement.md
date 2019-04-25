---
title: win32LobAppPowerShellScriptRequirement リソースの種類
description: Win32 アプリを検出するための PowerShell スクリプトのプロパティが含まれています
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3a3a7abc3c20320e6f197354caf560b6212a5e9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534557"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a>win32LobAppPowerShellScriptRequirement リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 アプリを検出するための PowerShell スクリプトのプロパティが含まれています


[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出の演算子。 可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。|
|detectionValue|String|[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出値|
|displayName|String|このルールの一意の表示名|
|enforceSignatureCheck|ブール値|署名チェックを適用するかどうかを示す値|
|runAs32Bit|ブール値|このスクリプトを32ビットとして実行する必要があるかどうかを示す値。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|スクリプトを実行する実行コンテキストの種類を示します。 可能な値は、`system`、`user` です。|
|scriptcontent|String|Win32 基幹業務 (LoB) アプリを検出するための、base64 でエンコードされたスクリプトの内容|
|detectionType|[win32LobAppPowerShellScriptDetectionType](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|スクリプト出力の検出の種類。 可能な値は、`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version`、`boolean` です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```





