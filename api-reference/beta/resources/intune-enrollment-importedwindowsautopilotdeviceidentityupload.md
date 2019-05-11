---
title: importedWindowsAutopilotDeviceIdentityUpload リソースの種類
description: アップロードを使用して windows 自動操縦デバイスをインポートします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5651df7238cf8e4e535b47d8c1aa1cac5d72725
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941549"
---
# <a name="importedwindowsautopilotdeviceidentityupload-resource-type"></a>importedWindowsAutopilotDeviceIdentityUpload リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アップロードを使用して windows 自動操縦デバイスをインポートします。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト importedWindowsAutopilotDeviceIdentityUploads](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-list.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)コレクション|[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ImportedWindowsAutopilotDeviceIdentityUpload を取得する](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-get.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ImportedWindowsAutopilotDeviceIdentityUpload を作成する](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-create.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|新しい[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトを作成します。|
|[ImportedWindowsAutopilotDeviceIdentityUpload の削除](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-delete.md)|None|[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)を削除します。|
|[ImportedWindowsAutopilotDeviceIdentityUpload の更新](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-update.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトのプロパティを更新します。|
|[autopilotDeviceStream 関数](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream.md)|String|自動操縦装置ストリームを使用して、アップロード要求を作成します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|String|オブジェクトの GUID|
|createdDateTimeUtc|DateTimeOffset|エンティティが作成された日時。|
|status|[importedWindowsAutopilotDeviceIdentityUploadStatus](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|アップロードの状態。 可能な値は、`noUpload`、`pending`、`complete`、`error` です。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) コレクション|このアップロードの一部としてのすべての自動操縦デバイスのコレクションです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "String (identifier)",
  "createdDateTimeUtc": "String (timestamp)",
  "status": "String"
}
```




