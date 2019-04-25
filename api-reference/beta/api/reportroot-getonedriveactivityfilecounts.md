---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fd595786e98b6b70380af668902c9013bf58eb76
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545947"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a>reportRoot: getOneDriveActivityFileCounts

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :--------------------------------------- |
| 委任 (職場または学校のアカウント)     | Reports.Read.All                         |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                           |
| アプリケーション                            | Reports.Read.All                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a>関数パラメーター

要求 URL に、次のパラメーターと有効な値を指定します。

| パラメーター | 型   | 説明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | 文字列 | レポートを集計する期間の長さを指定します。 {period_value} でサポートされている値は D7、D30、D90、D180 です。 これらの値は、D*n* の形式 (*n* はレポートを集計する日数) に従います。 必須。 |

このメソッドは、 `$format`応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートします。 既定の出力の種類は、text/csv です。 ただし、出力の種類を指定する場合は、OData $format クエリパラメーターを text/csv または application/json に設定します。

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
- 表示済みまたは編集済み
- 同期済み
- 社内で共有済み
- 外部で共有済み
- レポート日付
- レポート期間

### <a name="json"></a>JSON

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**[siteactivitysummary](../resources/siteactivitysummary.md)** オブジェクトを返します。

## <a name="example"></a>例

### <a name="csv"></a>CSV

CSV を出力する例を次に示します。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a>JSON

次の例は、JSON を返します。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a>応答

応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 1997, 
      "synced": 24756, 
      "sharedInternally": 7, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
