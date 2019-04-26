---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: グループ別の Yammer グループ アクティビティに関する詳細を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e6f606bca46428861c46b94471ea06b990a5f472
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331526"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a>reportRoot: getYammerGroupsActivityDetail

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グループ別の Yammer グループ アクティビティに関する詳細を取得します。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。

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
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
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
- グループ表示名
- 削除済み
- 所有者のプリンシパル名
- 最後のアクティビティ日付
- グループの種類
- Office 365 接続
- メンバー数
- 投稿数
- 読み取り数
- 「いいね!」の数
- レポート期間

### <a name="json"></a>JSON

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** オブジェクトを返します。

この要求の既定のページサイズは200アイテムです。

## <a name="example"></a>例

### <a name="csv"></a>CSV

CSV を出力する例を次に示します。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a>応答

応答の例を次に示します。

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a>JSON

次の例は、JSON を返します。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a>応答

応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
      "reportPeriod": "7"
    }
  ]
}
```
