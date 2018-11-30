---
title: Microsoft グラフ セキュリティ API のエラー応答
description: Graph で Microsoft グラフ セキュリティ API のエラーは、標準的な HTTP 206 部分的なコンテンツのステータス コードを使用して返されます、警告ヘッダーを使用して配信されます。
ms.openlocfilehash: 35af0a1ed4c4bf7f6e1afb36039f812ab59f64dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024018"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft グラフ セキュリティ API のエラー応答

Graph で Microsoft グラフ セキュリティ API のエラーは、標準的な HTTP 206 部分的なコンテンツのステータス コードを使用して返されます、警告ヘッダーを使用して配信されます。

Microsoft グラフ セキュリティ API は、すべてのデータ プロバイダーから複数の応答を受信するフェデレーション サービスです。 Microsoft グラフ セキュリティ API が HTTP エラーを受信したを送信します戻る警告ヘッダーで次の形式。<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

この警告ヘッダーはデータ プロバイダーの 1 つ以外の 2 xx または 404 エラー コードが返されるときにクライアントにのみ送信されます。 例:

- HttpStatusCode.Forbidden (403) は、リソースへのアクセスが与えられていない場合に返される可能性があります。
- プロバイダーがタイムアウトになった場合は、警告ヘッダーの HttpStatusCode.GatewayTimeout (504) が返されます。
- 内部プロバイダ エラーが発生した場合、HttpStatusCode.InternalServerError (500) は、warning ヘッダーで使用されます。

データ プロバイダーに 2 xx または 404 が返される場合に表示されませんの警告ヘッダーのこれらのコードが成功した場合に期待どおりになっているか、それぞれのデータが見つからない場合。 フェデレートされたシステムでは、何度もデータだけがわかっている 1 つまたはいくつか、すべてではなくプロバイダーと、404 が見つかりませんが考えられます。

## <a name="example"></a>使用例

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

## <a name="see-also"></a>関連項目

認証に問題がある場合は、私たちの[ブログの投稿](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2)を参照してください。
