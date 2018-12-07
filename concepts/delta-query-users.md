---
title: ユーザーに対する増分の変更を取得する
description: デルタ クエリでは、一連のデルタ関数呼び出しを使用して、ユーザーへの追加、削除、または更新に対してクエリを実行できます。デルタ クエリを使用すると、Microsoft Graph からユーザーのセット全体をフェッチして、変更を比較せずに、ユーザーへの変更を検出できます。
ms.openlocfilehash: 4b0237d01ad806a72c80c55522b06d4b37dc3a44
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092393"
---
# <a name="get-incremental-changes-for-users"></a>ユーザーに対する増分の変更を取得する

[デルタ クエリ](./delta-query-overview.md)では、一連の[デルタ](/graph/api/user-delta?view=graph-rest-1.0)関数呼び出しを使用して、ユーザーへの追加、削除、または更新に対してクエリを実行できます。デルタ クエリを使用すると、Microsoft Graph からユーザーのセット全体をフェッチして、変更を比較せずに、ユーザーへの変更を検出できます。

同期するユーザーとローカル プロファイル ストアを使用するクライアントは、最初の完全同期とその後の増分同期の両方でデルタ クエリを使用できます。通常なら、クライアントはテナント内のすべてのユーザーの最初の完全同期を実行し、その後、ユーザーへの増分の変更を定期的に取得します。

## <a name="tracking-user-changes"></a>ユーザー変更の追跡

ユーザー変更の追跡は、**デルタ**関数を使用した、1 つ以上の GET 要求のラウンドです。GET 要求は、次を含めることを除き、[ユーザーの一覧表示](/graph/api/user-list?view=graph-rest-1.0)とほぼ同じ方法で実行します。

- **デルタ**関数。
- 以前の GET **デルタ**関数呼び出しからの[状態トークン](./delta-query-overview.md) (_deltaToken_ または _skipToken_)。

## <a name="example"></a>例

次の例は、ユーザーへの変更を追跡するための一連の要求を示しています。

1. [最初の要求](#initial-request)と[応答](#initial-response)
2. [nextLink 要求](#nextlink-request)と[応答](#nextlink-response)
3. [最後の nextLink 要求](#final-nextlink-request)と[応答](#final-nextlink-response)
4. [deltaLink 要求](#deltalink-request)と [deltaLink 応答](#deltalink-response)

## <a name="initial-request"></a>最初の要求

ユーザー リソースの変更の追跡を開始するには、ユーザー リソースにデルタ関数を含む要求を実行します。

以下の点に注意してください。

- オプションの $Select クエリ パラメーターは、クエリ パラメーターが将来の要求に自動的に含まれる方法をデモンストレーションする要求に含まれています。
- 最初の要求には、状態トークンは含まれません。状態トークンはそれ以降の要求で使用されます。

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

## <a name="initial-response"></a>最初の応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](/graph/api/resources/user?view=graph-rest-1.0) コレクション オブジェクトを返します。ユーザーのセット全体が大きすぎると仮定した場合、応答には nextLink 状態トークンも含まれます。

この例では、セッションで取得するデータの追加ページがあることを示す nextLink URL が返されます。最初の要求からの $select クエリ パラメーターは、nextLink URL にエンコードされます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Testuser1",
      "givenName":"John",
      "surname":"Doe",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Testuser2",
      "givenName":"Jane",
      "surname":"Doe",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    }
  ]
}
```

## <a name="nextlink-request"></a>nextLink 要求

2 番目の要求は、前の応答から返された `skipToken` を指定します。`$select` パラメーターは、`skipToken` によってエンコードされ含まれるため必須ではないことに注意してください。

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a>nextLink 応答

応答には `nextLink` および `skipToken` が含まれ、利用可能な他のユーザーがあることを示しています。deltaLink URL が応答で返されるまで、nextLink URL を使用して要求を実行し続けます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Testuser3",
      "givenName":"Pat",
      "surname":"Doe",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Testuser4",
      "givenName":"Meghan",
      "surname":"Doe",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

## <a name="final-nextlink-request"></a>最後の nextLink 要求

3 番目の要求は、最後の同期要求から返された最新の `skipToken` を引き続き使用します。 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhaOYDE2VPA4vxIPA90-P6OzGd6Rvku5fDgBRIGS
```

## <a name="final-nextlink-response"></a>最後の nextLink 応答

deltaLink URL が返されると、返されるリソースの既存の状態に関するデータはなくなります。以降の要求では、アプリケーションは deltaLink URL を使用して、リソースへの変更点について説明します。`deltaToken` を保存して、ユーザーへの変更を検出するために要求 URL で使用します。 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser5",
      "givenName":"Al",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Testuser6",
      "givenName":"Sam",
      "surname":"Doe",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

## <a name="deltalink-request"></a>deltaLink 要求

[最後の応答](#final-nextlink-response)からの `deltaToken` を使用すると、最後の要求以降に (追加、削除、または更新によって) 変更されたユーザーを取得できます。

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a>deltaLink 応答

変更が行われなかった場合は、結果のない同じ `deltaToken` が返されます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": []
}
```

変更が行われた場合は、変更されたユーザーのコレクションを含む、同じ `deltaToken` が返されます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser7",
      "givenName":"Joe",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "id":"8ffff70c-1c63-4860-b963-e34ec660931d",
      "@removed": {
         "reason": "changed"
      }
    }
  ]
}
```

上記のサンプル応答に関する注意事項:

- ユーザーが削除されると、項目には `"reason": "changed"` の値が含まれた `@removed` のコメントが含まれます。

- ユーザーが完全に削除されると、項目には `"reason": "deleted"` の値が含まれた `@removed` のコメントが含まれます。

- ユーザーを作成または復元しても、コメントはありません。

## <a name="see-also"></a>関連項目
[Microsoft Graph デルタ クエリ](delta-query-overview.md)の概要。