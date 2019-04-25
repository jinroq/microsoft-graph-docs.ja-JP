---
title: ユーザーに対する増分の変更を取得する
description: デルタ クエリでは、一連のデルタ関数呼び出しを使用して、ユーザーへの追加、削除、または更新に対してクエリを実行できます。デルタ クエリを使用すると、Microsoft Graph からユーザーのセット全体をフェッチして、変更を比較せずに、ユーザーへの変更を検出できます。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: b4f79951f79393e22c40ef9a4f55e29e0145ccea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526336"
---
# <a name="get-incremental-changes-for-users"></a><span data-ttu-id="e3449-104">ユーザーに対する増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="e3449-104">Get incremental changes for users</span></span>

<span data-ttu-id="e3449-p102">[デルタ クエリ](./delta-query-overview.md)では、一連の[デルタ](/graph/api/user-delta?view=graph-rest-1.0)関数呼び出しを使用して、ユーザーへの追加、削除、または更新に対してクエリを実行できます。デルタ クエリを使用すると、Microsoft Graph からユーザーのセット全体をフェッチして、変更を比較せずに、ユーザーへの変更を検出できます。</span><span class="sxs-lookup"><span data-stu-id="e3449-p102">[Delta query](./delta-query-overview.md) lets you query for additions, deletions, or updates to users, by way of a series of [delta](/graph/api/user-delta?view=graph-rest-1.0) function calls. Delta query enables you discover changes to users without having to fetch the entire set of users from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="e3449-p103">同期するユーザーとローカル プロファイル ストアを使用するクライアントは、最初の完全同期とその後の増分同期の両方でデルタ クエリを使用できます。通常なら、クライアントはテナント内のすべてのユーザーの最初の完全同期を実行し、その後、ユーザーへの増分の変更を定期的に取得します。</span><span class="sxs-lookup"><span data-stu-id="e3449-p103">Clients using synchronizing users with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the users in a tenant, and subsequently, get incremental changes to users periodically.</span></span>

## <a name="tracking-user-changes"></a><span data-ttu-id="e3449-109">ユーザー変更の追跡</span><span class="sxs-lookup"><span data-stu-id="e3449-109">Tracking user changes</span></span>

<span data-ttu-id="e3449-p104">ユーザー変更の追跡は、**デルタ**関数を使用した、1 つ以上の GET 要求のラウンドです。GET 要求は、次を含めることを除き、[ユーザーの一覧表示](/graph/api/user-list?view=graph-rest-1.0)とほぼ同じ方法で実行します。</span><span class="sxs-lookup"><span data-stu-id="e3449-p104">Tracking user changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list users](/graph/api/user-list?view=graph-rest-1.0), except that you include the following:</span></span>

- <span data-ttu-id="e3449-112">**デルタ**関数。</span><span class="sxs-lookup"><span data-stu-id="e3449-112">The **delta** function.</span></span>
- <span data-ttu-id="e3449-113">以前の GET **デルタ**関数呼び出しからの[状態トークン](./delta-query-overview.md) (_deltaToken_ または _skipToken_)。</span><span class="sxs-lookup"><span data-stu-id="e3449-113">A [state token](./delta-query-overview.md) (_deltaToken_ or _skipToken_) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="e3449-114">例</span><span class="sxs-lookup"><span data-stu-id="e3449-114">Example</span></span>

<span data-ttu-id="e3449-115">次の例は、ユーザーへの変更を追跡するための一連の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3449-115">The following example shows a series  requests to track changes to users:</span></span>

1. <span data-ttu-id="e3449-116">[最初の要求](#initial-request)と[応答](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="e3449-116">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="e3449-117">[nextLink 要求](#nextlink-request)と[応答](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="e3449-117">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="e3449-118">[最後の nextLink 要求](#final-nextlink-request)と[応答](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="e3449-118">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="e3449-119">[deltaLink 要求](#deltalink-request)と [deltaLink 応答](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="e3449-119">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="e3449-120">最初の要求</span><span class="sxs-lookup"><span data-stu-id="e3449-120">Initial request</span></span>

<span data-ttu-id="e3449-121">ユーザー リソースの変更の追跡を開始するには、ユーザー リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="e3449-121">To begin tracking changes in the user resource, you make a request including the delta function on the user resource.</span></span>

<span data-ttu-id="e3449-122">以下の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="e3449-122">Note the following:</span></span>

- <span data-ttu-id="e3449-123">オプションの $Select クエリ パラメーターは、クエリ パラメーターが将来の要求に自動的に含まれる方法をデモンストレーションする要求に含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3449-123">The optional $select query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="e3449-p105">最初の要求には、状態トークンは含まれません。状態トークンはそれ以降の要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e3449-p105">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

## <a name="initial-response"></a><span data-ttu-id="e3449-126">最初の応答</span><span class="sxs-lookup"><span data-stu-id="e3449-126">Initial response</span></span>

<span data-ttu-id="e3449-p106">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](/graph/api/resources/user?view=graph-rest-1.0) コレクション オブジェクトを返します。ユーザーのセット全体が大きすぎると仮定した場合、応答には nextLink 状態トークンも含まれます。</span><span class="sxs-lookup"><span data-stu-id="e3449-p106">If successful, this method returns `200 OK` response code and [user](/graph/api/resources/user?view=graph-rest-1.0) collection object in the response body. Assuming the entire set of users is too large, the response will also include a nextLink state token.</span></span>

<span data-ttu-id="e3449-p107">この例では、セッションで取得するデータの追加ページがあることを示す nextLink URL が返されます。最初の要求からの $select クエリ パラメーターは、nextLink URL にエンコードされます。</span><span class="sxs-lookup"><span data-stu-id="e3449-p107">In this example, a nextLink URL is returned indicating there are additional pages of data to be retrieved in the session. The $select query parameter from the initial request is encoded into the nextLink URL.</span></span>

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

## <a name="nextlink-request"></a><span data-ttu-id="e3449-131">nextLink 要求</span><span class="sxs-lookup"><span data-stu-id="e3449-131">nextLink request</span></span>

<span data-ttu-id="e3449-p108">2 番目の要求は、前の応答から返された `skipToken` を指定します。`$select` パラメーターは、`skipToken` によってエンコードされ含まれるため必須ではないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="e3449-p108">The second request specifies the `skipToken` returned from the previous response. Notice the `$select` parameter is not required, as the `skipToken` encodes and includes it.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a><span data-ttu-id="e3449-134">nextLink 応答</span><span class="sxs-lookup"><span data-stu-id="e3449-134">nextLink response</span></span>

<span data-ttu-id="e3449-p109">応答には `nextLink` および `skipToken` が含まれ、利用可能な他のユーザーがあることを示しています。deltaLink URL が応答で返されるまで、nextLink URL を使用して要求を実行し続けます。</span><span class="sxs-lookup"><span data-stu-id="e3449-p109">The response contains a `nextLink` and another `skipToken`, indicating there are more users available. You continue making requests using the nextLink URL until a deltaLink URL is returned in the response.</span></span>

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

## <a name="final-nextlink-request"></a><span data-ttu-id="e3449-137">最後の nextLink 要求</span><span class="sxs-lookup"><span data-stu-id="e3449-137">Final nextLink request</span></span>

<span data-ttu-id="e3449-138">3 番目の要求は、最後の同期要求から返された最新の `skipToken` を引き続き使用します。</span><span class="sxs-lookup"><span data-stu-id="e3449-138">The third request continues to use the latest `skipToken` returned from the last sync request.</span></span> 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhaOYDE2VPA4vxIPA90-P6OzGd6Rvku5fDgBRIGS
```

## <a name="final-nextlink-response"></a><span data-ttu-id="e3449-139">最後の nextLink 応答</span><span class="sxs-lookup"><span data-stu-id="e3449-139">Final nextLink response</span></span>

<span data-ttu-id="e3449-p110">deltaLink URL が返されると、返されるリソースの既存の状態に関するデータはなくなります。以降の要求では、アプリケーションは deltaLink URL を使用して、リソースへの変更点について説明します。`deltaToken` を保存して、ユーザーへの変更を検出するために要求 URL で使用します。</span><span class="sxs-lookup"><span data-stu-id="e3449-p110">When the deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource. Save the `deltaToken` and use it in the request URL to discover changes to users.</span></span> 

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

## <a name="deltalink-request"></a><span data-ttu-id="e3449-143">deltaLink 要求</span><span class="sxs-lookup"><span data-stu-id="e3449-143">deltaLink request</span></span>

<span data-ttu-id="e3449-144">[最後の応答](#final-nextlink-response)からの `deltaToken` を使用すると、最後の要求以降に (追加、削除、または更新によって) 変更されたユーザーを取得できます。</span><span class="sxs-lookup"><span data-stu-id="e3449-144">Using the `deltaToken` from the [last response](#final-nextlink-response), you will be able to get changed (by being added, deleted, or updated) users since the last request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a><span data-ttu-id="e3449-145">deltaLink 応答</span><span class="sxs-lookup"><span data-stu-id="e3449-145">deltaLink response</span></span>

<span data-ttu-id="e3449-146">変更が行われなかった場合は、結果のない同じ `deltaToken` が返されます。</span><span class="sxs-lookup"><span data-stu-id="e3449-146">If no changes have occurred, the same `deltaToken` is returned with no results.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": []
}
```

<span data-ttu-id="e3449-147">変更が行われた場合は、変更されたユーザーのコレクションを含む、同じ `deltaToken` が返されます。</span><span class="sxs-lookup"><span data-stu-id="e3449-147">If changes have occurred, the same `deltaToken` is returned including a collection of changed users.</span></span>

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

<span data-ttu-id="e3449-148">上記のサンプル応答に関する注意事項:</span><span class="sxs-lookup"><span data-stu-id="e3449-148">Some things to note about the example response above:</span></span>

- <span data-ttu-id="e3449-149">ユーザーが削除されると、項目には `"reason": "changed"` の値が含まれた `@removed` のコメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e3449-149">When the user is deleted, the item contains an annotation: `@removed` with value of `"reason": "changed"`.</span></span>

- <span data-ttu-id="e3449-150">ユーザーが完全に削除されると、項目には `"reason": "deleted"` の値が含まれた `@removed` のコメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e3449-150">When the user is permanently deleted, the item contains an annotation: `@removed` with value of `"reason": "deleted"`.</span></span>

- <span data-ttu-id="e3449-151">ユーザーを作成または復元しても、コメントはありません。</span><span class="sxs-lookup"><span data-stu-id="e3449-151">When the user is created, or restored, there is no annotation.</span></span>

## <a name="see-also"></a><span data-ttu-id="e3449-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3449-152">See also</span></span>
<span data-ttu-id="e3449-153">[Microsoft Graph デルタ クエリ](delta-query-overview.md)の概要。</span><span class="sxs-lookup"><span data-stu-id="e3449-153">[Microsoft Graph delta query](delta-query-overview.md) overview.</span></span>
