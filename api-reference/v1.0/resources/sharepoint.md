# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>Microsoft Graph で SharePoint サイトを開く

Microsoft Graph の SharePoint API は、以下の基本的なシナリオをサポートしています。

* SharePoint **サイト**および**ドライブ** (ドキュメント ライブラリ) へのアクセス
* **サイト** リソースの読み取り専用機能 (新しいサイトは作成できません)
* **driveItems** の読み取り/書き込みサポート
* SharePoint ID、URL、または相対パスでリソースを指定する

## <a name="sharepoint-api-root-resources"></a>SharePoint API のルート リソース

以下は、`https://graph.microsoft.com/v1.0` に関する例です。

| パス                                   | 説明
|:---------------------------------------|:------------------------------------
| /sites/root                            | 組織の既定の[サイト][]
| /sites/{site-id}                       | ID を使って特定の[サイト][]にアクセスする
| /sites/{site-id}/drive                 | 指定した[サイト][]の既定の[ドライブ](drive.md) (ドキュメント ライブラリ) にアクセスする
| /sites/{site-id}/drives                | [サイト][]の下にある[ドライブ](drive.md) (ドキュメント ライブラリ) を列挙する。
| /sites/{site-id}/sites                 | [サイト][]の下のサブサイトを列挙する。
| /groups/{group-id}/sites/root          | グループのチーム [サイト][]にアクセスする

サイトは、SharePoint のホスト名の後にコロンとサイトへの相対パスを入れる形で指定できます。最後にコロン (:) を入れるとリソースモデル指定画面に戻れます (オプション)。

| パス                                           | 説明
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | https://contoso.sharepoint.com/teams/hr に関連付けられているサイト
| /sites/contoso.sharepoint.com:/teams/hr:/drive | このサイトの既定の[ドライブ](drive.md)にアクセスする

## <a name="note-for-existing-sharepoint-developers"></a>既存の SharePoint 開発者向けのメモ

Microsoft Graph の SharePoint API は、CSOM API と大きく異なる点がいくつかあります。[サイト][]のリソースは `SPWeb` にマッピングされます。サイト コレクションのルート[サイト][] (`SPWeb`) には、`SPSite` に関する情報を含む [siteCollection](sitecollection.md) ファセットが含まれています。サイトの ID はそのサイト コレクション内でのみ一意であり、ID でサイトを指定する場合、サイト コレクション識別子とサイト識別子の両方を指定する必要があります。

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id},{spweb-id}/
```
ホスト名のみで作成された URL は、既定のサイト コレクションのルート サイト (`SPWeb`) をポイントします。

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname}
```

ホスト名と siteCollection (`SPSite`) ID のみで作成された URL は、指定したサイト コレクションのルート サイト (`SPWeb`) をポイントします。

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id}
```

[サイト]: site.md
[drive]: drive.md
[siteCollection]: siteCollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
