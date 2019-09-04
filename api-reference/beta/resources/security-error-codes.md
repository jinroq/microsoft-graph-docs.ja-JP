---
title: Microsoft Graph セキュリティ API のエラー応答
description: Microsoft Graph セキュリティ API のエラーは、標準の HTTP 206 の部分的なコンテンツ状態コードを使用して返され、警告ヘッダーによって配信されます。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 2291f0009c7d54a62ac30d448a9f97ff8935a569
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726313"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft Graph セキュリティ API のエラー応答

Microsoft Graph セキュリティ API のエラーは、標準の HTTP 206 の部分的なコンテンツ状態コードを使用して返され、警告ヘッダーによって配信されます。

## <a name="errors"></a>Errors

Microsoft Graph セキュリティ API は、すべてのデータプロバイダーから複数の応答を受け取るフェデレーションサービスです。 Microsoft Graph セキュリティ API で HTTP エラーが受信されると、次の形式の警告ヘッダーが返されます。
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

この警告ヘッダーは、いずれかのデータプロバイダーが2xx または404以外のエラーコードを返した場合にのみクライアントに返されます。 次に例を示します。

- リソースへのアクセス許可が付与されていない場合、HttpStatusCode (403) が返されることがあります。
- プロバイダーがタイムアウトになると、HttpStatusCode (504) が警告ヘッダーに返されます。
- 内部プロバイダエラーが発生した場合は、HttpStatusCode エラー (500) が警告ヘッダーで使用されます。

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

## <a name="threat-indicator-bulk-action-errors"></a>脅威インジケーターの一括アクションエラー

一括操作 (作成、更新、および削除) は、2つの異なる潜在的なエラーコードを生成できます。  400エラーコードは、提供された本文にシリアル化中にエラーが発生したことを示します。また、206エラーコードは、プロバイダーに対してフェデレーションアウトされたときに1つ以上の一括操作が失敗したことを示します。 応答には、脅威インテリジェンスインジケーターごとに個別のプロバイダーからの成功/エラーデータが含まれます。 警告とは異なり、潜在的なすべてのエラー情報は、脅威インジケーターの一括アクションに対する応答の本文内に含まれます。

## <a name="constraints"></a>制約

`$top` Odata クエリパラメーターには、1000通知の制限があり、odata クエリ`$top`  +  `$skip`パラメーターの組み合わせは、6000通知を超えることはできません。 例えば、`/security/alerts?$top=10&$skip=5990` は応答コード `200 OK` を返しますが、`/security/alerts?$top=10&$skip=5991` は応答コード `400 Bad Request` を返します。

この制限の回避策は、 `$filter` OData クエリパラメーターを Microsoft GRAPH セキュリティ API の`eventDateTime` alert エンティティので使用し、dateTime 値を`?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}`最後 (6000th) 通知で置き換えることです。 また、 `eventDateTime`の範囲を設定することもできます。たとえば、*警告? $filter = eventdatetime **gt** 2018-11-**11**T00:00: 00.000 z&eventdatetime **lt** 2018-11-**12**T00:00: 00.000 z*

## <a name="see-also"></a>関連項目

承認の問題が発生している場合は、「 [authorization and The Microsoft Graph SECURITY API](/graph/security-authorization)」を参照してください。
