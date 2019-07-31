---
title: detectedApp リソースの種類
description: 管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。 非管理対象アプリは、会社所有のデバイスにのみ表示されます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d48b205a01444184634ebaaff1a39b76b551859f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999984"
---
# <a name="detectedapp-resource-type"></a>detectedApp リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。 非管理対象アプリは、会社所有のデバイスにのみ表示されます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[detectedApps のリスト](../api/intune-devices-detectedapp-list.md)|[detectedApp](../resources/intune-devices-detectedapp.md) コレクション|[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[detectedApp の取得](../api/intune-devices-detectedapp-get.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[detectedApp の作成](../api/intune-devices-detectedapp-create.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。|
|[detectedApp の削除](../api/intune-devices-detectedapp-delete.md)|なし|[detectedApp](../resources/intune-devices-detectedapp.md) を削除します。|
|[detectedApp の更新](../api/intune-devices-detectedapp-update.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|検出されたアプリケーションの一意識別子。 これは、アプリケーションの作成時に、Intune によって自動的に生成されます。 読み取り専用です。|
|displayName|String|検出されたアプリケーションの名前。 読み取り専用|
|version|String|検出されたアプリケーションのバージョン。 読み取り専用|
|sizeInByte|Int64|検出されたアプリケーションのサイズ (バイト単位)。 読み取り専用です|
|deviceCount|Int32|このアプリケーションがインストールされているデバイスの数|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) コレクション|検出されたアプリケーションがインストールされているデバイス|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```





