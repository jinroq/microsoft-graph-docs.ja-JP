---
title: iosWebContentFilterSpecificWebsitesAccess リソースの種類
description: IOS iOS の組み込みブラウザーに URL のブックマークをインストールする Web コンテンツのフィルター設定の種類を表します。 先生が受講者が、iOS デバイスと他のサイトへのアクセスなしで構成されているブラウザーのブックマークから web サイトを移動するようには教室では、シナリオの例です。
localization_priority: Normal
ms.openlocfilehash: 0dc3023c37311dc5fdeb2700b8a0fec58bdb4725
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844955"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>iosWebContentFilterSpecificWebsitesAccess リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

IOS iOS の組み込みブラウザーに URL のブックマークをインストールする Web コンテンツのフィルター設定の種類を表します。 先生が受講者が、iOS デバイスと他のサイトへのアクセスなしで構成されているブラウザーのブックマークから web サイトを移動するようには教室では、シナリオの例です。

[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|specificWebsitesOnly|[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション|組み込みのブラウザーやユーザーにインストールされている URL のブックマークはブックマークから web サイトにアクセスのみ許可されます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|websiteList|[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション|組み込みのブラウザーやユーザーにインストールされている URL のブックマークはブックマークから web サイトにアクセスのみ許可されます。 このコレクションには、最大で 500 個の要素を含めることができます。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```





