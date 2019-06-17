---
title: iosSingleSignOnSettings リソースの種類
description: シングルサインオンの iOS Kerberos 認証設定
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11875bb07b87cf8c9415660f5961dafa73f54f57
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995617"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

シングルサインオンの iOS Kerberos 認証設定

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|allowedAppsList プロパティ|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|このログインの使用が許可されているアプリ識別子のリスト。 このフィールドを省略した場合、ログインはデバイス上のすべてのアプリケーションに適用されます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|allowedUrls|文字列コレクション|このログインを使用するために一致する必要がある HTTP Url のリスト。 IOS 9.0 以降では、ワイルドカード文字を使用することができます。|
|displayName|String|受信側デバイスに表示されるログイン設定の表示名。|
|kerberosPrincipalName|String|Kerberos プリンシパル名。 指定しない場合、プロファイルのインストール時にユーザーに対してプロンプトが表示されます。|
|kerberosRealm|String|Kerberos 領域名。 大文字小文字を区別します。|

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





