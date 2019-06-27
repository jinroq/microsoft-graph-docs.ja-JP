---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: グループ別の Office 365 グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a165087479abdab0445a362524b31c3c531eb631
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268678"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a>reportRoot: getOffice365GroupsActivityDetail

グループ別の Office 365 グループ アクティビティに関する詳細を取得します。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :--------------------------------------- |
| 委任 (職場または学校アカウント)     | Reports.Read.All                         |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                           |
| アプリケーション                            | Reports.Read.All                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a>関数パラメーター

要求 URL に、次のうちの 1 つのパラメーターと有効な値を指定します。

| パラメーター | 型   | 説明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | 文字列 | レポートを集計する期間の長さを指定します。 {period_value} でサポートされている値は D7、D30、D90、D180 です。 これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。 |
| date      | 日付   | 何らかのアクティビティを実行したユーザーを表示する日付を指定します。 {date_value} は YYYY-MM-DD の形式にします。 このレポートは、過去 30 日間のみ利用可能であり、{date_value} はその範囲内の日付である必要があります。 |

> **注:** URL に期間または日付を設定する必要があります。

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明                              |
| :------------ | :--------------------------------------- |
| Authorization | ベアラー {トークン}。必須。                |
| If-None-Match | この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。 省略可能。 |

## <a name="response"></a>応答

成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。 その URL は、応答の `Location` ヘッダー内にあります。

事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。

この CSV ファイルには、次の列ヘッダーがあります。

- レポートの更新日
- グループ表示名
- 削除済み
- 所有者のプリンシパル名
- 最後のアクティビティ日付
- グループの種類
- メンバー数
- 外部メンバー数
- Exchange の受信メール数
- SharePoint のアクティブなファイル数
- Yammer に投稿されたメッセージ数
- Yammer の開封済みメッセージ数
- Yammer で「いいね!」されたメッセージ数
- Exchange メールボックスのアイテム合計数
- 使用済み Exchange メールボックス ストレージ (バイト)
- SharePoint の合計ファイル数
- SharePoint の使用済みサイト ストレージ (バイト)
- レポート期間

## <a name="example"></a>例

#### <a name="request"></a>要求

要求の例を次に示します。

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```

#### <a name="response"></a>応答

応答の例を次に示します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivityuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivityuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
