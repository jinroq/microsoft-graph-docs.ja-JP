---
title: win32LobAppInstallExperience リソースの種類
description: Win32 アプリケーションのインストール環境のプロパティが含まれています
author: tfitzmac
ms.openlocfilehash: c24ed0536416bd330fc2928a85cb0d5fce558256
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342162"
---
# <a name="win32lobappinstallexperience-resource-type"></a>win32LobAppInstallExperience リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Win32 アプリケーションのインストール環境のプロパティが含まれています
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|アプリケーションが実行される実行コンテキストの種類を示します。 可能な値: `system`、`user`。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```





