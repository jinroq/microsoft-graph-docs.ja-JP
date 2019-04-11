---
title: iosSingleSignOnSettings リソースの種類
description: シングルサインオンの iOS Kerberos 認証設定
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12d0e424870d81b762e0e6d9b58df4a942055123
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775563"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

シングルサインオンの iOS Kerberos 認証設定

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|allowedappslist プロパティ|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|このログインの使用が許可されているアプリ識別子のリスト。 このフィールドを省略した場合、ログインはデバイス上のすべてのアプリケーションに適用されます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|allowedUrls|String コレクション|このログインを使用するために一致する必要がある HTTP url のリスト。 iOS 9.0 以降では、ワイルドカード文字を使用することができます。|
|displayName|String|受信側デバイスに表示されるログイン設定の表示名。|
|kerberosPrincipalName|文字列|Kerberos プリンシパル名。 指定しない場合、プロファイルのインストール時にユーザーに対してプロンプトが表示されます。|
|kerberosRealm|文字列|Kerberos 領域名。 大文字小文字を区別します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```





