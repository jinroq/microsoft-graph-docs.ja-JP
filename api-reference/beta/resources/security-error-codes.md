---
title: Microsoft グラフ セキュリティ API のエラー応答
description: セキュリティ api には、Microsoft のグラフのエラーは、標準の HTTP 206 部分的なコンテンツのステータス コードを使用して返され、警告ヘッダーを経由して配信。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 52b7c375bd3e0c6a367f1150a21bb96ef84437ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921430"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft グラフ セキュリティ API のエラー応答

セキュリティ api には、Microsoft のグラフのエラーは、標準の HTTP 206 部分的なコンテンツのステータス コードを使用して返され、警告ヘッダーを経由して配信。

## <a name="errors"></a>Errors

Microsoft グラフ セキュリティ API は、すべてのデータ プロバイダーから複数の応答を受信するフェデレーション サービスです。 Microsoft グラフ セキュリティ API が HTTP エラーを受信したを送信します戻る警告ヘッダーで次の形式。<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

この警告ヘッダーはデータ プロバイダーの 1 つ以外の 2 xx または 404 エラー コードが返されるときにクライアントにのみ送信されます。 次に例を示します。

- HttpStatusCode.Forbidden (403) は、リソースへのアクセスが与えられていない場合に返される可能性があります。
- プロバイダーがタイムアウトになった場合は、警告ヘッダーの HttpStatusCode.GatewayTimeout (504) が返されます。
- 内部プロバイダ エラーが発生した場合、HttpStatusCode.InternalServerError (500) は、warning ヘッダーで使用されます。

データ プロバイダーに 2 xx または 404 が返される場合に表示されませんの警告ヘッダーのこれらのコードが成功した場合に期待どおりになっているか、それぞれのデータが見つからない場合。 フェデレートされたシステムでは、何度もデータだけがわかっている 1 つまたはいくつか、すべてではなくプロバイダーと、404 が見つかりませんが考えられます。

## <a name="example"></a>例

ユーザーが求める`security/alerts/{alert_id}`。

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

404 と 200 の両方が必要な条件であるため warning ヘッダーは、次の含まれています。

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **注:** 各 HTTP ヘッダーは、ユーザーは警告ヘッダーを列挙し、すべての項目をチェックするために、サブ項目のコレクションです。

## <a name="constraints"></a>制約

`$top` OData クエリ パラメーターには、1000 の警告との組み合わせの制限`$top`  +  `$skip` OData クエリのパラメーターは、警告が 6000 を超えることはできません。 などの`/security/alerts?$top=10&$skip=5990`を返します、`200 OK`応答コードの場合が、`/security/alerts?$top=10&$skip=5991`を返します、`400 Bad Request`応答コード。

回避制限値については、使用する、`$filter`で OData クエリのパラメーター、 `eventDateTime` Microsoft グラフ セキュリティ API から通知のエンティティを使用して`?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}`(6000th) の最後の警告で、日時の値を置き換えることです。 範囲を設定することも、 `eventDateTime`。たとえば、 *alerts?$ フィルター = eventDateTime **gt** 2018-11-**11**T00:00:00.000Z & eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*

## <a name="see-also"></a>関連項目

認証に問題がある場合は、[承認、および Microsoft のグラフのセキュリティ API](/graph/security-authorization)を参照してください。
