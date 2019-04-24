---
title: iosWebContentFilterSpecificWebsitesAccess リソースの種類
description: ios の組み込みブラウザーに URL ブックマークをインストールする、ios Web コンテンツフィルター設定の種類を表します。 この例は、教師が iOS デバイスで構成されているブラウザーのブックマークを使用して web サイトにアクセスして、他のサイトにアクセスできないようにするための教室のクラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7d5b60af9a3b17923faac4dd0136ef6a9bc1591
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460472"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>iosWebContentFilterSpecificWebsitesAccess リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ios の組み込みブラウザーに URL ブックマークをインストールする、ios Web コンテンツフィルター設定の種類を表します。 この例は、教師が iOS デバイスで構成されているブラウザーのブックマークを使用して web サイトにアクセスして、他のサイトにアクセスできないようにするための教室のクラスです。


[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|固有の webwebonly|[iosbookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション|組み込みのブラウザーとユーザーにインストールされる URL ブックマークは、ブックマークを介して web サイトにのみアクセスできます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|websiteList|[iosbookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション|組み込みのブラウザーとユーザーにインストールされる URL ブックマークは、ブックマークを介して web サイトにのみアクセスできます。 このコレクションには、最大で 500 個の要素を含めることができます。|

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





