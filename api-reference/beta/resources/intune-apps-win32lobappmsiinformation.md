---
title: win32LobAppMsiInformation リソースの種類
description: Win32 アプリ用の MSI アプリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ddb69d3f01c816c592617cb75ed6f9b9877f856
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790061"
---
# <a name="win32lobappmsiinformation-resource-type"></a>win32LobAppMsiInformation リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 アプリ用の MSI アプリのプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|productCode|文字列|MSI 製品コード。|
|productVersion|String|MSI 製品バージョン。|
|upgradeCode|文字列|MSI アップグレードコード。|
|requiresReboot|Boolean|MSI アプリがインストールを完了するためにコンピューターを再起動する必要があるかどうか。|
|packagetype|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|MSI パッケージの種類。 使用可能な値は、`perMachine`、`perUser`、`dualPurpose` です。|
|productName|文字列型 (String)|MSI 製品名。|
|publisher|文字列|MSI パブリッシャー。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```





