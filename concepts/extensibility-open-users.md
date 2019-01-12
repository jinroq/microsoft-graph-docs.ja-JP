---
title: オープン拡張機能を使用してカスタム データをユーザーに追加する
description: '*オープン拡張機能*の使用方法について、具体例を使ってデモンストレーションします。 '
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 69b0918dba3159a552e2b00d4f54b21e67d017e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867264"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a>オープン拡張機能を使用してカスタム データをユーザーに追加する
*オープン拡張機能*の使用方法について、具体例を使ってデモンストレーションします。 

デスクトップやモバイルなど、多種のクライアント プラットフォームで利用できるアプリケーションをビルドしているとします。アプリにサインインするときのデバイスに関係なく一貫性を確保できるように、ユーザー自身で UI エクスペリエンスを構成できるようにしたいと考えています。これは、ほとんどのアプリで一般的な要件です。 

このシナリオでは、以下の操作を行う方法を紹介します。

1. ユーザーに関する何らかのローミング プロファイル情報を表すオープン拡張機能を追加します。
2. ユーザーに対してクエリを実行し、ローミング プロファイルを返します。
3. ユーザーのローミング プロファイル情報 (オープン拡張機能値) を変更します。
4. ユーザーのローミング プロファイル情報を削除します。

>**注:** このトピックでは、*user* リソースにおいてオープン拡張機能を追加、読み取り、更新、削除する方法を示します。これらの方法は、*administrativeUnit*、*contact*、*device*、*event*、*group*、*group event*、*group post*、*organizaton* の各リソース型でもサポートされています。  
これらのリソース型のいずれかを使用して、次の例の要求を簡単に更新できます。次の例に示されている応答は、わかりやすくするために途中までしか示されていない場合があります。 

## <a name="1-add-roaming-profile-information"></a>1.ローミング プロファイル情報を追加する
ユーザーがアプリにサインインし、アプリの外観を構成します。これらのアプリ設定はローミングされ、アプリにサインインするためにユーザーが使用するデバイスに関わらず同じエクスペリエンスになるようにする必要があります。ここでは、ユーザーのリソースにローミング プロファイル情報を追加する方法を示します。

##### <a name="request"></a>要求
```http
POST https://graph.microsoft.com/v1.0/me/extensions
Content-type: application/json
{
    "@odata.type":"microsoft.graph.openTypeExtension",
    "extensionName":"com.contoso.roamingSettings",
    "theme":"dark",
    "color":"purple",
    "lang":"Japanese"
}
```
##### <a name="response"></a>応答
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a>2.ローミング プロファイル情報を取得する
ユーザーが別のデバイスからアプリにサインインするときに、アプリはユーザーのプロファイル詳細とローミング設定を取得できます。これは、ユーザーのリソースを取得し、拡張ナビゲーション プロパティを展開することによって行えます。

##### <a name="request"></a>要求
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
##### <a name="response"></a>応答
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420

{
    "id": "84b80893-8749-40a3-97b7-68513b600544",
    "displayName": "John Smith",
    "mail": "john@contoso.com",
    "mobilePhone": "1-555-6589",
    "extensions": [
        {
            "@odata.type": "#microsoft.graph.openTypeExtension",
            "extensionName": "com.contoso.roamingSettings",
            "id": "com.contoso.roamingSettings",
            "theme": "dark",
            "color": "purple",
            "lang": "Japanese"
        }
    ]
}
```
>**注:** 複数の拡張機能がある場合、対象の拡張機能を取得するために *id* でフィルター処理できます。

## <a name="3-change-roaming-profile-information"></a>3.ローミング プロファイル情報を変更する
ユーザーは、ローミング プロファイル情報を変更することができます。オープン拡張機能の値で ```PATCH``` を使用して更新できます。 

##### <a name="request"></a>要求
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

##### <a name="response"></a>応答
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a>4.ユーザーのローミング プロファイルを削除する
ローミング プロファイルがもはや不要であるとユーザーが判断する場合、削除できます。オープン拡張機能の値で ```DELETE``` 要求を使用して行えます。

##### <a name="request"></a>要求
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a>応答
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用したリソースへのカスタム データの追加](extensibility-overview.md)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](extensibility-schema-groups.md)
- [openTypeExtension リソース タイプ](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [オープン拡張機能を作成する](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [オープン拡張機能を取得する](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [オープン拡張機能を更新する](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [オープン拡張機能を削除する](/graph/api/opentypeextension-delete?view=graph-rest-1.0)
