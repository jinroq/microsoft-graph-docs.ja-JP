---
title: iosWebContentFilterAutoFilter リソースの種類
description: '[IOS Web コンテンツフィルターの設定] の種類を表します。これにより、iOS 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。 プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。'
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5f788dd4843b45dd7e9ed5793ef2a3c147eba429
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970354"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>iosWebContentFilterAutoFilter リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[IOS Web コンテンツフィルターの設定] の種類を表します。これにより、iOS 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。 プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。


[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|allowedUrls|文字列コレクション|アクセスできる追加 Url|
|blockedUrls|文字列コレクション|アクセスのためにブロックされる追加 Url|

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





