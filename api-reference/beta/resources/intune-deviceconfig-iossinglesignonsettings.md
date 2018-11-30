---
title: iosSingleSignOnSettings リソースの種類
description: iOS は単一のサインオンでの Kerberos 認証の設定
ms.openlocfilehash: a63848dc27afd037a6834a67c0736f86c06ac1fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072958"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS は単一のサインオンでの Kerberos 認証の設定
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|allowedAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|このログインを使用するのには許可されているアプリケーションの識別子の一覧です。 このフィールドを省略すると、ログインは、デバイス上のすべてのアプリケーションに適用されます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|allowedUrls|String コレクション|このログインを使用するために一致する必要がある HTTP Url の一覧です。 9.0 以降、iOS でワイルドカード文字を使用することがあります。|
|displayName|String|受信側デバイスに表示されるログインの設定の表示名。|
|kerberosPrincipalName|String|Kerberos プリンシパルの名前です。 指定しない場合、プロファイルのインストール時にいずれかの入力が求められます。|
|kerberosRealm|String|Kerberos レルムの名前です。 大文字小文字を区別します。|

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





