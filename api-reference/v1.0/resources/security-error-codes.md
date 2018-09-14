# <a name="security-api-error-responses"></a>セキュリティ API のエラー応答

Microsoft Graph のセキュリティ API のエラーは、標準の HTTP ステータス コードを使用して返され、警告ヘッダーを介して配信されます。

セキュリティ API は、すべてのデータ プロバイダーから複数の応答を受信するフェデレーション サービスです。 セキュリティ API は HTTP エラーを受信すると、次の形式の警告ヘッダーを送信して返します。 <!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

この警告ヘッダーは、データ プロバイダーの 1 つが 2 xx または 404 以外のエラー コードを返すときにのみ、クライアントに送信して返されます。 例:

- リソースへのアクセスが与えられていない場合は、HttpStatusCode.Forbidden (403) が返される場合があります。
- プロバイダーがタイムアウトになった場合は、警告ヘッダー内に HttpStatusCode.GatewayTimeout (504) が返されます。
- 内部プロバイダ エラーが発生した場合は、警告ヘッダー内で HttpStatusCode.InternalServerError (500) が使用されます。

データ プロバイダーが 2xx または 404 を返す場合は、それは警告ヘッダーに表示されません。なぜなら、2xx は成功した場合、404 はデータが見つからない場合に想定されるコードであるからです。 フェデレーション システムでは、多くの場合、データが 1 つまたはいくつかのプロバイダーには知られていても、すべてのプロバイダーには知られていないため、データが見つからない場合の 404 が返されることが想定されます。

## <a name="example"></a>例

ユーザーが `security/alerts/{alert_id}` を求めます。

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

404 と 200 の両方は想定される条件であるため、警告ヘッダーには次のものが含まれます。 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/29000",    (usual timeout limit is set at 29 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **注:** 各 HTTP ヘッダーはサブ項目のコレクションであるため、ユーザーは警告ヘッダーを列挙して、すべての項目をチェックすることができます。

## <a name="see-also"></a>関連項目

承認に問題がある場合は、私たちの[ブログ記事](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2)をご覧ください。
