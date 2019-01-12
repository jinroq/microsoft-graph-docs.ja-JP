---
title: iosSingleSignOnSettings リソースの種類
description: iOS は単一のサインオンでの Kerberos 認証の設定
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54c5656de6262692324cce8ab71a0e100672c050
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952672"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS は単一のサインオンでの Kerberos 認証の設定
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
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





