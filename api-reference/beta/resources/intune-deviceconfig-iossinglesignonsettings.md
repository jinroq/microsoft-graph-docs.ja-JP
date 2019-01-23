---
title: iosSingleSignOnSettings リソースの種類
description: iOS は単一のサインオンでの Kerberos 認証の設定
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 189fb79be741bdf6b731b1e3c2b336934db8c86b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421320"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




