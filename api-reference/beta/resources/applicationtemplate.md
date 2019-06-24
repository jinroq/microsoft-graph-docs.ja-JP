---
title: applicationTemplate リソースの種類
description: Azure AD アプリケーションギャラリーのアプリケーションを表します。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a8e1f4cb365f86df32e32ed568aa3a96d1c090f
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147927"
---
# <a name="applicationtemplate-resource-type"></a>applicationTemplate リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[AZURE AD アプリケーションギャラリー](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list)のアプリケーションを表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
|[ApplicationTemplate の一覧表示](../api/applicationtemplate-list.md)|[applicationTemplate](applicationtemplate.md)|ApplicationTemplate オブジェクトのリストを取得します。|
| [ApplicationTemplate の取得](../api/applicationtemplate-get.md) | [applicationTemplate](applicationtemplate.md) | ApplicationTemplate オブジェクトのプロパティとリレーションシップを読み取ります。 |
|[ApplicationTemplate のインスタンス化](../api/applicationtemplate-instantiate.md)|[applicationServicePrincipal](applicationserviceprincipal.md)| Azure AD アプリケーションギャラリーからディレクトリにアプリケーションのインスタンスを追加します。|


## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|categories|String collection|アプリケーションのカテゴリのリスト。 サポートされている`Collaboration`値`Business Management`は`Consumer`次`Content management`の`CRM`とおり`Data services`です`Developer services`: `E-commerce`、 `Education` `ERP` `Finance` `Health` `Human resources` `IT infrastructure` `Mail` `Management`、 `Marketing`、、、、、、、 `Media` `Productivity`、、、、および`Web design & hosting` `Project management` `Telecommunications` `Tools, Travel`|
|description|String|アプリケーションの説明。|
|displayName|String|アプリケーションの名前を指定します。|
|ホームページの Url|String|アプリケーションのホームページの URL。|
|id|文字列| アプリケーションの一意識別子。 読み取り専用です。|
|logoUrl|String|このアプリケーションのロゴを取得する URL。|
|publisher|String|このアプリケーションの発行元の名前。|
|Supportedプロビジョニング型|文字列コレクション|このアプリケーションでサポートされているプロビジョニングモードのリスト。 有効な値は`sync`です。|
|supportedSingleSignOnModes|文字列コレクション|このアプリケーションでサポートされているシングルサインオンモードの一覧です。 サポートされて`password`いる`saml`値`external`は、 `oidc`、、です。|

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
