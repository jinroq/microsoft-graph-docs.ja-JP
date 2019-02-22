---
title: win32LobAppMsiInformation リソースの種類
description: Win32 アプリ用の MSI アプリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f330111a3e924e54cf23c30cd98d20e85cb38022
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158647"
---
# <a name="win32lobappmsiinformation-resource-type"></a>win32LobAppMsiInformation リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 アプリ用の MSI アプリのプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|productCode|String|MSI 製品コード。|
|productVersion|String|MSI 製品バージョン。|
|upgradeCode|String|MSI アップグレードコード。|
|requiresReboot|ブール値|MSI アプリがインストールを完了するためにコンピューターを再起動する必要があるかどうか。|
|packagetype|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|MSI パッケージの種類。 可能な値は `perMachine`、`perUser`、`dualPurpose` です。|
|productName|String|MSI 製品名。|
|publisher|文字列型 (String)|MSI パブリッシャー。|

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




