---
title: windowsKioskActiveDirectoryGroup リソースの種類
description: キオスクの構成の Azure ディレクトリ グループを識別するに使用するクラス
ms.openlocfilehash: 18e876b50bdc8c8946bd511348d6ed3a6fc8fe5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068259"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a>windowsKioskActiveDirectoryGroup リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

キオスクの構成の Azure ディレクトリ グループを識別するに使用するクラス

[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|グループ名|String|この構成にキオスクがロックアウトされている AD グループの名前|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





