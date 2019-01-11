---
title: 'reportRoot: getOffice365GroupsActivityGroupCounts'
description: グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。
localization_priority: Normal
ms.openlocfilehash: fa48d561cdb70dbb2ce47b07444e1fd3782b1f42
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811677"
---
# <a name="reportroot-getoffice365groupsactivitygroupcounts"></a>reportRoot: getOffice365GroupsActivityGroupCounts

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。

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
GET /reports/getOffice365GroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a>関数パラメーター

要求 URL に、次のパラメーターと有効な値を指定します。

| パラメーター | Type   | 説明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | 文字列 | レポートを集計する期間の長さを指定します。 {period_value} でサポートされている値は D7、D30、D90、D180 です。 これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。 必須。 |

このメソッドをサポートしている、 `$format` 、応答をカスタマイズするのには、 [OData クエリ パラメーター](/graph/query-parameters)です。 既定の出力の種類は、テキストまたは csv です。 ただし、出力の種類を指定する場合は、設定をテキストまたは csv またはアプリケーションまたは json OData $format クエリ パラメーターを使用することができます。

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
- 合計
- アクティブ
- レポート日付
- レポート期間

### <a name="json"></a>JSON

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の**[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** オブジェクトです。

## <a name="example"></a>例

### <a name="csv"></a>CSV

次に、CSV を出力する例を示します。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a>JSON

次に、JSON を取得する例を示します。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=application/json
```

#### <a name="response"></a>応答

応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 5344, 
      "active": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
