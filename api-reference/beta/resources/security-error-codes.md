---
title: Microsoft Graph セキュリティ API のエラー応答
description: Microsoft Graph セキュリティ API のエラーは、標準の HTTP 206 の部分的なコンテンツ状態コードを使用して返され、警告ヘッダーによって配信されます。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 52b7c375bd3e0c6a367f1150a21bb96ef84437ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549000"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft Graph セキュリティ API のエラー応答

Microsoft Graph セキュリティ API のエラーは、標準の HTTP 206 の部分的なコンテンツ状態コードを使用して返され、警告ヘッダーによって配信されます。

## <a name="errors"></a>エラー

Microsoft Graph セキュリティ API は、すべてのデータプロバイダーから複数の応答を受け取るフェデレーションサービスです。 Microsoft Graph セキュリティ API で HTTP エラーが受信されると、次の形式の警告ヘッダーが返されます。
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

この警告ヘッダーは、いずれかのデータプロバイダーが2xx または404以外のエラーコードを返した場合にのみクライアントに返されます。 次に例を示します。

- リソースへのアクセス許可が付与されていない場合、httpstatuscode (403) が返されることがあります。
- プロバイダーがタイムアウトになると、httpstatuscode (504) が警告ヘッダーに返されます。
- 内部プロバイダエラーが発生した場合は、httpstatuscode エラー (500) が警告ヘッダーで使用されます。

データプロバイダーが2xx または404を返した場合は、これらのコードが正常に終了したか、またはデータが検出されなかった場合は、警告ヘッダーに表示されません。 フェデレーションシステムでは、404が見つからない場合は、1つまたはいくつかのプロバイダーのみがデータを認識できる回数である必要があります。

## <a name="example"></a>例

ユーザーが要求`security/alerts/{alert_id}`します。

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

404と200の両方が想定される条件であるため、警告ヘッダーには次の内容が含まれています。

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **注:** 各 HTTP ヘッダーはサブアイテムのコレクションであるため、ユーザーは警告ヘッダーを列挙してすべてのアイテムをチェックできます。

## <a name="constraints"></a>制約

`$top` odata クエリパラメーターには、1000通知の制限があり、odata クエリ`$top`  +  `$skip`パラメーターの組み合わせは、6000通知を超えることはできません。 たとえば、 `/security/alerts?$top=10&$skip=5990`は`200 OK`応答コード`/security/alerts?$top=10&$skip=5991`を返しますが、応答コードを`400 Bad Request`返します。

この制限の回避策は、 `$filter` OData クエリパラメーターを Microsoft Graph セキュリティ API の`eventDateTime` alert エンティティので使用し、dateTime 値を`?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}`最後 (6000th) 通知で置き換えることです。 また、 `eventDateTime`の範囲を設定することもできます。たとえば、 *alerts? $ filter = eventdatetime **gt** 2018-11-**11**T00:00: 00.000 z_amp_eventdatetime **lt** 2018-11-**12**T00:00: 00.000 z*

## <a name="see-also"></a>関連項目

承認の問題が発生している場合は、「 [authorization and the Microsoft Graph Security API](/graph/security-authorization)」を参照してください。
