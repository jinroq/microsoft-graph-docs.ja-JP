---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: SharePoint サイトの使用状況に関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: aa946a67870fcbdae795ff221268b9c5b016cbd3
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639314"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a>reportRoot: getSharePointSiteUsageDetail

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

SharePoint サイトの使用状況に関する詳細を取得します。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :--------------------------------------- |
| 委任 (職場または学校アカウント)     | Reports.Read.All                         |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                           |
| アプリケーション                            | Reports.Read.All                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a>関数パラメーター

要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。

| パラメーター | 型   | 説明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | 文字列 | レポートを集計する期間の長さを指定します。 {period_value} でサポートされている値は D7、D30、D90、D180 です。 これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。 |
| date      | 日付   | 何らかのアクティビティを実行したユーザーを表示する日付を指定します。 {date_value} は YYYY-MM-DD の形式にします。 このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。 |

> **注:** URL に期間または日付を設定する必要があります。

このメソッドは、応答をカスタマイズするための `$format`、`$top`、`$skipToken` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。 既定の出力の種類は、text/csv です。 ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明               |
| :------------ | :------------------------ |
| Authorization | ベアラー {トークン}。必須。 |

## <a name="response"></a>応答

### <a name="csv"></a>CSV

成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。 その URL は、応答の `Location` ヘッダー内にあります。

事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。

この CSV ファイルには、次の列ヘッダーがあります。

- レポートの更新日
- サイト Id
- サイトの URL
- 所有者の表示名
- 削除済み
- 最後のアクティビティ日付
- ファイル数
- アクティブなファイル数
- ページ ビューの数
- アクセスしたページ数
- 使用済みストレージ (バイト)
- 割り当て済みストレージ (バイト)
- ルート Web テンプレート
- レポート期間

### <a name="json"></a>JSON

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[Sharepointsite使い方詳細](../resources/sharepointsiteusagedetail.md)** オブジェクトを返します。

この要求の既定のページサイズは200アイテムです。

## <a name="example"></a>例

### <a name="csv"></a>CSV

CSV を出力する例を次に示します。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a>応答

応答の例を次に示します。

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagedetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagedetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
```

### <a name="json"></a>JSON

次の例は、JSON を返します。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a>応答

応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagedetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagedetail_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagedetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagedetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagedetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagedetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
