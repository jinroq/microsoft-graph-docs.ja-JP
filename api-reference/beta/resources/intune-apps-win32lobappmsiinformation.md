---
title: win32LobAppMsiInformation リソースの種類
description: Win32 アプリケーションの MSI アプリケーションのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 1753df68ab1f4b0e1649c16a4a7fa0ad49941bf9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326139"
---
# <a name="win32lobappmsiinformation-resource-type"></a>win32LobAppMsiInformation リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Win32 アプリケーションの MSI アプリケーションのプロパティが含まれています。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|productCode|String|MSI の製品コードです。|
|productVersion|String|MSI 製品のバージョンです。|
|upgradeCode|String|Msi ファイルは、コードをアップグレードします。|
|requiresReboot|ブール型|かどうか、MSI アプリケーションには、インストールの完了に再起動するコンピューターが必要です。|
|packageType|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|MSI パッケージの種類です。 可能な値は、`perMachine`、`perUser`、`dualPurpose` です。|

## <a name="relationships"></a>関係
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
  "packageType": "String"
}
```





