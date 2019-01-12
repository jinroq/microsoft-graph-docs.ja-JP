---
title: iosWebContentFilterAutoFilter リソースの種類
description: IOS iOS の自動フィルター機能を有効にし、その他の URL のアクセス制御では、Web コンテンツ フィルター設定の種類を表します。 構築すると、プロパティ値を持たない、iOS デバイスは、自動でフィルター処理に関係なく有効になります。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 03e3c4f51e673be1e2bada89e06a26048fe4e385
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916781"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>iosWebContentFilterAutoFilter リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

IOS iOS の自動フィルター機能を有効にし、その他の URL のアクセス制御では、Web コンテンツ フィルター設定の種類を表します。 構築すると、プロパティ値を持たない、iOS デバイスは、自動でフィルター処理に関係なく有効になります。

[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|allowedUrls|String コレクション|追加の Url のアクセス許可|
|blockedUrls|String コレクション|追加の Url アクセスのブロック|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```





