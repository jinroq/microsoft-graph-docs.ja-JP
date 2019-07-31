---
title: win32LobAppMsiInformation リソースの種類
description: Win32 アプリ用の MSI アプリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d993306cdd5f6c69d373669ed83fab6f986497df
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971656"
---
# <a name="win32lobappmsiinformation-resource-type"></a>win32LobAppMsiInformation リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 アプリ用の MSI アプリのプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|productCode|String|MSI 製品コード。|
|productVersion|String|MSI 製品バージョン。|
|upgradeCode|String|MSI アップグレードコード。|
|requiresReboot|Boolean|MSI アプリがインストールを完了するためにコンピューターを再起動する必要があるかどうか。|
|packageType|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|MSI パッケージの種類。 可能な値は、`perMachine`、`perUser`、`dualPurpose` です。|
|productName|文字列型 (String)|MSI 製品名。|
|publisher|String|MSI パブリッシャー。|

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





