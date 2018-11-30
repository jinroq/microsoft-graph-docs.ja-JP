---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
ms.openlocfilehash: 16d191bb53f7546598b7869e8bc28be07cc4f604
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070893"
---
# <a name="applistitem-resource-type"></a>appListItem リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理対象アプリケーションの一覧にあるアプリを表します
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|名前|文字列型 (String)|アプリケーション名|
|発行元|文字列型 (String)|アプリケーションの発行元|
|appStoreUrl|文字列型 (String)|アプリケーションのストア URL|
|appId|文字列型 (String)|アプリケーションのアプリケーションまたはバンドルの識別子|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```





