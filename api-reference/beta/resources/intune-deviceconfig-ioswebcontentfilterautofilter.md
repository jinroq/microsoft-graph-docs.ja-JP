---
title: iosWebContentFilterAutoFilter リソースの種類
description: '[ios Web コンテンツフィルターの設定] の種類を表します。これにより、ios 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。 プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91efedb47fff71a66d12e0d2c976d61fab2fa76c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460416"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>iosWebContentFilterAutoFilter リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[ios Web コンテンツフィルターの設定] の種類を表します。これにより、ios 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。 プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。


[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|allowedUrls|String collection|アクセスできる追加 url|
|blockedUrls|String collection|アクセスのためにブロックされる追加 url|

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





