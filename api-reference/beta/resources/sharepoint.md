---
title: Microsoft Graph で SharePoint サイトを開く
description: Microsoft Graph の SharePoint API は、以下の基本的なシナリオをサポートしています。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 9edab0f8e4207dac2a88943a0a2cd1cbe58b97e3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583915"
---
# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>Microsoft Graph で SharePoint サイトを開く

Microsoft Graph の SharePoint API は、以下の基本的なシナリオをサポートしています。

* SharePoint **サイト**、**リスト**、および**ドライブ** (ドキュメント ライブラリ) へのアクセス
* **サイト** リソースの読み取り専用サポート (新しいサイトは作成できません)
* **リスト**、**listItem** および **driveItem** の読み取り/書き込みサポート
* SharePoint ID、URL、または相対パスでリソースを指定する

SharePoint API は、次の 3 つの主要なリソースの種類を公開します。

* [サイト](site.md) _(最上位のオブジェクト)_
* [リスト](list.md)
* [ListItem](listitem.md)

次に、listItem リソースの例を示します。

```json
{
  "fields": {
    "Title": "Access card",
    "Employee": "Ryan Gregg",
    "EmployeeId": "10",
    "CardSerial": "01235492",
    "Alias": "RGregg",
    "ID": 1,
    "ContentType": "Item",
    "Modified": "2016-09-19T23:15:25-07:00",
    "Created": "2016-09-19T23:15:25-07:00"
  },
  "createdBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "createdDateTime": "2016-09-20T06:15:25Z",
  "eTag": "48e941c3-9515-4c48-9760-c07c90c79d48,1",
  "id": "4",
  "lastModifiedBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "lastModifiedDateTime": "2016-09-20T06:15:25Z",
}
```

リソースでは、次の異なる 3 つの方法でデータを公開します。

* _プロパティ_ (**id** や **name** など) は単純な値を公開します。
* _ファセット_(**フィールド** や **createdBy** など) は複雑な値を公開します。
* _参照_ (**items** など) はその他のリソースのコレクションを指します。

`?expand=fields` などの _expand_ クエリ パラメーターで、URL 内の参照を展開することができます。
`?select=id,name` などの _select_ クエリ パラメーターで、特定のプロパティやファセットを要求することができます。
既定では、プロパティとファセットはほとんどが返されるのに対し、参照はいずれも表示されません。
効率を高めるには、注目すべきデータだけに _select_ と _expand_ を返すことをお勧めします。

## <a name="sharepoint-api-root-resources"></a>SharePoint API のルート リソース

以下は、`https://graph.microsoft.com/beta` に関する例です。

| パス                                   | 説明
|:---------------------------------------|:------------------------------------
| /sites/root                            | 組織の既定の[サイト][]
| /sites/{site-id}                       | ID を使って特定の[サイト][]にアクセスする
| /sites/{site-id}/drive                 | 指定した[サイト][]の既定の[ドライブ](drive.md) (ドキュメント ライブラリ) にアクセスする
| /sites/{site-id}/drives                | [サイト][]の下にある[ドライブ](drive.md) (ドキュメント ライブラリ) を列挙する。
| /sites/{site-id}/sites                 | [サイト][]の下のサブサイトを列挙する。
| /sites/{site-id}/lists                 | [サイト](site.md)の下の[リスト](list.md)を列挙する。
| /sites/{site-id}/lists/{list-id}/items | [リスト](list.md)の下の [listItem](listitem.md) を列挙する。
| /groups/{group-id}/sites/root          | グループのチーム [サイト][]にアクセスする

サイトは、SharePoint のホスト名の後にコロンとサイトへの相対パスを入れる形で指定できます。最後にコロン (:) を入れるとリソースモデル指定画面に戻れます (オプション)。

| パス                                           | 説明
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | https://contoso.sharepoint.com/teams/hr に関連付けられているサイト
| /sites/contoso.sharepoint.com:/teams/hr:/drive | このサイトの既定の[ドライブ](drive.md)にアクセスする

## <a name="note-for-existing-sharepoint-developers"></a>既存の SharePoint 開発者向けのメモ

Microsoft Graph の SharePoint API は、CSOM API と大きく異なる点がいくつかあります。
[サイト][] リソースは `SPWeb` にマッピングされます。
サイト コレクションのルート [サイト][] (`SPWeb`) には、`SPSite` に関する情報を含む [siteCollection](sitecollection.md) ファセットが含まれています。
サイトの ID はそのサイト コレクション内でのみ一意であり、ID でサイトを指定する場合、サイト コレクション識別子とサイト識別子の両方を指定する必要があります。

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id},{spweb-id}/
```
ホスト名のみで作成された URL は、既定のサイト コレクションのルート サイト (`SPWeb`) をポイントします。

```http
GET https://graph.microsoft.com/beta/sites/{hostname}
```

ホスト名と siteCollection (`SPSite`) ID のみで作成された URL は、指定したサイト コレクションのルート サイト (`SPWeb`) をポイントします。

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id}
```

[サイト]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: sitecollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
