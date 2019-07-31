---
title: iosWebContentFilterSpecificWebsitesAccess リソースの種類
description: Ios の組み込みブラウザーに URL ブックマークをインストールする、iOS Web コンテンツフィルター設定の種類を表します。 この例は、教師が iOS デバイスで構成されているブラウザーのブックマークを使用して web サイトにアクセスして、他のサイトにアクセスできないようにするための教室のクラスです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 32cf57ba7ab96a68914ceeaf0693162ef9ab8e69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001055"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>iosWebContentFilterSpecificWebsitesAccess リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Ios の組み込みブラウザーに URL ブックマークをインストールする、iOS Web コンテンツフィルター設定の種類を表します。 この例は、教師が iOS デバイスで構成されているブラウザーのブックマークを使用して web サイトにアクセスして、他のサイトにアクセスできないようにするための教室のクラスです。


[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|固有の Webwebonly|[Iosbookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション|組み込みのブラウザーとユーザーにインストールされる URL ブックマークは、ブックマークを介して web サイトにのみアクセスできます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|websiteList|[Iosbookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション|組み込みのブラウザーとユーザーにインストールされる URL ブックマークは、ブックマークを介して web サイトにのみアクセスできます。 このコレクションには、最大で 500 個の要素を含めることができます。|

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





