---
title: グループに対する増分の変更を取得する
description: デルタのクエリは、追加、削除、またはグループに一連のデルタ関数の呼び出しを使用して更新のクエリを実行できます。 グループへの変更を検出するデルタ ・ クエリを有効に
ms.openlocfilehash: b043d62e0d99b4d71e25a8367abc731d39ad6d45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092351"
---
# <a name="get-incremental-changes-for-groups"></a><span data-ttu-id="067b4-104">グループに対する増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="067b4-104">Get incremental changes for groups</span></span>

<span data-ttu-id="067b4-p102">[デルタ クエリ](./delta-query-overview.md)では、一連の[デルタ](/graph/api/group-delta?view=graph-rest-1.0)関数呼び出しを使用して、グループへの追加、削除、または更新に対してクエリを実行できます。デルタ クエリを使用すると、Microsoft Graph からグループのセット全体をフェッチして、変更を比較せずに、グループへの変更を検出できます。</span><span class="sxs-lookup"><span data-stu-id="067b4-p102">[Delta query](./delta-query-overview.md) lets you query for additions, deletions, or updates to groups, by way of a series of [delta](/graph/api/group-delta?view=graph-rest-1.0) function calls. Delta query enables you discover changes to groups without having to fetch the entire set of groups from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="067b4-p103">同期するグループとローカル プロファイル ストアを使用するクライアントは、最初の完全同期とその後の増分同期の両方でデルタ クエリを使用できます。通常なら、クライアントはテナント内のすべてのグループの最初の完全同期を実行し、その後、グループへの増分の変更を定期的に取得します。</span><span class="sxs-lookup"><span data-stu-id="067b4-p103">Clients using synchronizing groups with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the groups in a tenant, and subsequently, get incremental changes to groups periodically.</span></span>

## <a name="tracking-group-changes"></a><span data-ttu-id="067b4-109">グループ変更の追跡</span><span class="sxs-lookup"><span data-stu-id="067b4-109">Tracking group changes</span></span>

<span data-ttu-id="067b4-p104">グループ変更の追跡は、**デルタ**関数を使用した、1 つ以上の GET 要求のラウンドです。GET 要求は、次を含めることを除き、[グループの一覧表示](/graph/api/group-list?view=graph-rest-1.0)とほぼ同じ方法で実行します。</span><span class="sxs-lookup"><span data-stu-id="067b4-p104">Tracking group changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list groups](/graph/api/group-list?view=graph-rest-1.0), except that you include the following:</span></span>

- <span data-ttu-id="067b4-112">**デルタ**関数。</span><span class="sxs-lookup"><span data-stu-id="067b4-112">The **delta** function.</span></span>
- <span data-ttu-id="067b4-113">以前の GET **デルタ**関数呼び出しからの[状態トークン](./delta-query-overview.md) (*deltaToken* または *skipToken*)。</span><span class="sxs-lookup"><span data-stu-id="067b4-113">A [state token](./delta-query-overview.md) (*deltaToken* or *skipToken*) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="067b4-114">例</span><span class="sxs-lookup"><span data-stu-id="067b4-114">Example</span></span>

<span data-ttu-id="067b4-115">次の例は、グループへの変更を追跡するための一連の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="067b4-115">The following example shows a series  requests to track changes to groups:</span></span>

1. <span data-ttu-id="067b4-116">[最初の要求](#initial-request)と[応答](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="067b4-116">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="067b4-117">[nextLink 要求](#nextlink-request)と[応答](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="067b4-117">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="067b4-118">[最後の nextLink 要求](#final-nextlink-request)と[応答](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="067b4-118">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="067b4-119">[deltaLink 要求](#deltalink-request)と [deltaLink 応答](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="067b4-119">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="067b4-120">最初の要求</span><span class="sxs-lookup"><span data-stu-id="067b4-120">Initial request</span></span>

<span data-ttu-id="067b4-121">グループ リソースの変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="067b4-121">To begin tracking changes in the group resource, you make a request including the delta function on the group resource.</span></span>

<span data-ttu-id="067b4-122">以下の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="067b4-122">Note the following:</span></span>

- <span data-ttu-id="067b4-123">オプションの `$select` クエリ パラメーターが要求に含められているのは、クエリ パラメーターが将来の要求に自動的に含まれる方法を示すためです。</span><span class="sxs-lookup"><span data-stu-id="067b4-123">The optional `$select` query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="067b4-124">オプションの `$expand` クエリ パラメーターが含められているのは、グループのメンバーをグループ オブジェクトと共に取り出す方法を示すためです。</span><span class="sxs-lookup"><span data-stu-id="067b4-124">The optional `$expand` query parameter is included to show how group members can be retrieved together with group objects.</span></span> <span data-ttu-id="067b4-125">それにより、グループのユーザーの追加や削除など、メンバーシップの変更を追跡できます。</span><span class="sxs-lookup"><span data-stu-id="067b4-125">This allows tracking of membership changes, such as when users are added or removed from groups.</span></span>
- <span data-ttu-id="067b4-p106">最初の要求には、状態トークンは含まれません。状態トークンはそれ以降の要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="067b4-p106">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

## <a name="initial-response"></a><span data-ttu-id="067b4-128">最初の応答</span><span class="sxs-lookup"><span data-stu-id="067b4-128">Initial response</span></span>

<span data-ttu-id="067b4-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](/graph/api/resources/group?view=graph-rest-1.0) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="067b4-129">If successful, this method returns `200 OK` response code and [group](/graph/api/resources/group?view=graph-rest-1.0) collection object in the response body.</span></span> <span data-ttu-id="067b4-130">グループ セット全体が大きすぎて 1 つの応答では収まらない場合、状態トークンが含まれる `nextLink` も含められます。</span><span class="sxs-lookup"><span data-stu-id="067b4-130">If the entire set of groups is too large to fit in one response, a `nextLink` containing a state token will also be included.</span></span>

<span data-ttu-id="067b4-131">この例の場合、`nextLink` が含められました。元の `$select` および `$expand` クエリ パラメーターは、状態トークンの中にエンコードされています。</span><span class="sxs-lookup"><span data-stu-id="067b4-131">In this example, a `nextLink` was included; the original `$select` and `$expand` query parameters are encoded in the state token.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

><span data-ttu-id="067b4-132">**注:** 、`members@delta`プロパティは、- TestGroup1 - の最初のグループ オブジェクトに含まれているし、2 つの現在のメンバー グループが含まれています。</span><span class="sxs-lookup"><span data-stu-id="067b4-132">**Note:** The `members@delta` property is included in the first group object - TestGroup1 - and contains the two current members of the group.</span></span> <span data-ttu-id="067b4-133">TestGroup2 にはメンバーがないため、このグループにはそのプロパティが含まれていません。</span><span class="sxs-lookup"><span data-stu-id="067b4-133">TestGroup2 does not contain that property because the group does not have any members.</span></span>

## <a name="nextlink-request"></a><span data-ttu-id="067b4-134">nextLink 要求</span><span class="sxs-lookup"><span data-stu-id="067b4-134">nextLink request</span></span>

<span data-ttu-id="067b4-135">2 番目の要求では、前の応答の `nextLink` を使用しています。それには、`skipToken` が含まれています。</span><span class="sxs-lookup"><span data-stu-id="067b4-135">The second request uses the `nextLink` from the previous response, which contains the `skipToken`.</span></span> <span data-ttu-id="067b4-136">`$select` パラメーターと `$expand` パラメーターは、トークンの中にエンコードされているため、明示的には存在しないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="067b4-136">Notice the `$select` and `$expand` parameters are not explicitly present as they are encoded in the token.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a><span data-ttu-id="067b4-137">nextLink 応答</span><span class="sxs-lookup"><span data-stu-id="067b4-137">nextLink response</span></span>

<span data-ttu-id="067b4-138">応答には新たな `skipToken` 値を指定した別の `nextLink` が含まれています。これは、利用可能な他のグループがあることを示しています。</span><span class="sxs-lookup"><span data-stu-id="067b4-138">The response contains another `nextLink` with a new `skipToken` value, indicating there are more groups available.</span></span> <span data-ttu-id="067b4-139">最後の応答で `deltaLink` URL が返されるまで、`nextLink` URL を使用して要求の発行を続けます。</span><span class="sxs-lookup"><span data-stu-id="067b4-139">You continue making requests using the `nextLink` URL until a `deltaLink` URL is returned in the final response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "3c8ac7c4-d365-4df9-abfa-356a9dd7763c"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="final-nextlink-request"></a><span data-ttu-id="067b4-140">最後の nextLink 要求</span><span class="sxs-lookup"><span data-stu-id="067b4-140">Final nextLink request</span></span>

<span data-ttu-id="067b4-141">3 番目の要求では、最新の `nextLink` を再び使用します。</span><span class="sxs-lookup"><span data-stu-id="067b4-141">The third request again uses the latest `nextLink`.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a><span data-ttu-id="067b4-142">最後の nextLink 応答</span><span class="sxs-lookup"><span data-stu-id="067b4-142">Final nextLink response</span></span>

<span data-ttu-id="067b4-143">最後に、`deltaLink` URL が返されます。これは、グループの既存の状態ではそれ以上のデータがないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="067b4-143">Finally, the `deltaLink` URL is returned, which means there is no more data for the existing state of groups.</span></span> <span data-ttu-id="067b4-144">アプリケーションは、その後の要求のため、`deltaLink` およびそれに含まれる `deltaToken` 値を使用して、グループに対する新たな変更について調べます。</span><span class="sxs-lookup"><span data-stu-id="067b4-144">For future requests, the application uses the `deltaLink` and the `deltaToken` value it contains to learn about new changes to groups.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a><span data-ttu-id="067b4-145">deltaLink 要求</span><span class="sxs-lookup"><span data-stu-id="067b4-145">deltaLink request</span></span>

<span data-ttu-id="067b4-146">[最後の応答](#final-nextlink-response)の `deltaLink` を使用することにより、最後の要求以降にグループに対して加えられた、実質的な新たな変更を入手できます。</span><span class="sxs-lookup"><span data-stu-id="067b4-146">Using the `deltaLink` from the [last response](#final-nextlink-response), you will be able to get net new changes to groups since the last request.</span></span> <span data-ttu-id="067b4-147">変更内容には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="067b4-147">Changes include:</span></span>
- <span data-ttu-id="067b4-148">新たに作成されたグループ オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="067b4-148">Newly created group objects.</span></span>
- <span data-ttu-id="067b4-149">削除されたグループ オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="067b4-149">Deleted group objects.</span></span>
- <span data-ttu-id="067b4-150">プロパティに変更が加えられたグループ オブジェクト (**displayName** が変更されたなど)。</span><span class="sxs-lookup"><span data-stu-id="067b4-150">Group objects for which a property has changed (e.g. **displayName** has been modified).</span></span>
- <span data-ttu-id="067b4-151">メンバー オブジェクトが追加または削除されたグループ オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="067b4-151">Group objects for which member objects have been added or removed.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a><span data-ttu-id="067b4-152">deltaLink 応答</span><span class="sxs-lookup"><span data-stu-id="067b4-152">deltaLink response</span></span>

<span data-ttu-id="067b4-153">変更がなかった場合は、結果なしで `deltaLink` が返されます。`value` プロパティは空になります。</span><span class="sxs-lookup"><span data-stu-id="067b4-153">If no changes have occurred, a `deltaLink` is returned with no results - the `value` property is empty.</span></span> <span data-ttu-id="067b4-154">アプリケーションでは将来の呼び出しに備えて、以前のリンクを新しいリンクに必ず置き換えてください。</span><span class="sxs-lookup"><span data-stu-id="067b4-154">Make sure to replace the previous link in the application with the new one for use in future calls.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

<span data-ttu-id="067b4-155">変更があった場合は、変更されたグループのコレクションが含められます。</span><span class="sxs-lookup"><span data-stu-id="067b4-155">If changes have occurred, a collection of changed groups is included.</span></span> <span data-ttu-id="067b4-156">さらに応答には、`nextLink` (取得対象の変更のページが複数ある場合) と `deltaLink` のどちらかも含まれています。</span><span class="sxs-lookup"><span data-stu-id="067b4-156">The response also contains either a `nextLink` - in case there are multiple pages of changes to retrieve - or a `deltaLink`.</span></span> <span data-ttu-id="067b4-157">`nextLinks` の後もそれまでと同じパターンを実装し、最後の `deltaLink` を将来の呼び出しに備えて保持しておいてください。</span><span class="sxs-lookup"><span data-stu-id="067b4-157">You should implement the same pattern of following the `nextLinks` as before and persist the final `deltaLink` for future calls.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
          {
              "displayName": "TestGroup3",
              "description": "A test group for change tracking",
              "id": "2e5807ce-58f3-4a94-9b37-ffff2e085957",
              "members@delta": [
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
                      "@removed": {
                          "reason": "deleted"
                      }
                  },
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "37de1ae3-408f-4702-8636-20824abda004"
                  }
              ]
          }
      ]
}
```

<span data-ttu-id="067b4-158">上記のサンプル応答に関する注意事項:</span><span class="sxs-lookup"><span data-stu-id="067b4-158">Some things to note about the example response above:</span></span>

- <span data-ttu-id="067b4-159">オブジェクトは、当初 `$select` および `$expand` のクエリ パラメーターで指定されたのと同じプロパティ セットを伴って返されます。</span><span class="sxs-lookup"><span data-stu-id="067b4-159">The objects are returned with the same set of properties originally specified via the `$select` and `$expand` query parameters.</span></span>

- <span data-ttu-id="067b4-160">変更されたプロパティと変更されていないプロパティの両方が含まれています。</span><span class="sxs-lookup"><span data-stu-id="067b4-160">Both changed and unchanged properties are included.</span></span> <span data-ttu-id="067b4-161">上記の例の場合、`description` プロパティの値は新しいものになっていますが、`displayName` プロパティは変更されていません。</span><span class="sxs-lookup"><span data-stu-id="067b4-161">In the example above, the `description` property has a new value, while the `displayName` property has not changed.</span></span>

- <span data-ttu-id="067b4-162">`members@delta` には、メンバーシップに対して加えられた変更内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="067b4-162">`members@delta` contains any changes to membership.</span></span>

  - <span data-ttu-id="067b4-163">リスト中の最初のユーザーが、メンバーシップを削除するか、またはユーザー オブジェクト自体を削除することにより、グループから削除されました。</span><span class="sxs-lookup"><span data-stu-id="067b4-163">The first user in the list has been removed from the group - either by removing the membership or by deleting the user object itself.</span></span> <span data-ttu-id="067b4-164">`@removed` プロパティがそのことを記述しています。</span><span class="sxs-lookup"><span data-stu-id="067b4-164">The `@removed` property describes that.</span></span>

  - <span data-ttu-id="067b4-165">2 番目のユーザーはグループに追加されました。</span><span class="sxs-lookup"><span data-stu-id="067b4-165">The second user has been added to the group.</span></span>

## <a name="paging-through-members-in-a-large-group"></a><span data-ttu-id="067b4-166">大規模グループ内のメンバー間のページング</span><span class="sxs-lookup"><span data-stu-id="067b4-166">Paging through members in a large group</span></span>

<span data-ttu-id="067b4-167">`members@delta` プロパティは、`$select` クエリ パラメーターが指定されていない場合、または `$expand=members` パラメーターが明示的に指定されている場合、既定でグループ オブジェクトに含められます。</span><span class="sxs-lookup"><span data-stu-id="067b4-167">The `members@delta` property is included in group objects by default, when the `$select` query parameter has not been specified, or when the `$expand=members` parameter is explicitly specified.</span></span> <span data-ttu-id="067b4-168">メンバー数の多いグループの場合、1 つの応答に全メンバーが収まらないことがあります。このセクションでは、そのような状況を処理するために実装しなければならないパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="067b4-168">For groups with many members it is possible that all members cannot fit into a single response; in this section we describe the pattern you should implement to handle such cases.</span></span>

><span data-ttu-id="067b4-169">**注:** このパターンは、グループ状態を最初に取得する際にも、それ以降にデルタ変更を取得するために呼び出す際にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="067b4-169">**Note:** This pattern applies to both the initial retrieval of group state as well as to subsequent calls to get delta changes.</span></span>

<span data-ttu-id="067b4-170">グループの初期状態のすべてを取得するため、またはそれ以降にデルタ変更を取得するために、次のデータ クエリを実行しているとします。</span><span class="sxs-lookup"><span data-stu-id="067b4-170">Let's assume you are executing the following delta query - either to capture the initial full state of groups, or later on to get delta changes:</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

1. <span data-ttu-id="067b4-171">Microsoft Graph は、`members@delta` プロパティに多くのメンバーが含まれる 1 つのグループ オブジェクトのみ含まれる応答を返すことがあります。</span><span class="sxs-lookup"><span data-stu-id="067b4-171">Microsoft Graph may return a response that contains just one group object, with a large list of members in the `members@delta` property:</span></span>

<span data-ttu-id="067b4-172">**最初のページ**</span><span class="sxs-lookup"><span data-stu-id="067b4-172">**First page**</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "37de1ae3-408f-4702-8636-20824abda004"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

2. <span data-ttu-id="067b4-173">`nextLink` をたどる際、再び同じグループ オブジェクトが含まれる応答を受け取ることがあります。</span><span class="sxs-lookup"><span data-stu-id="067b4-173">When you follow the `nextLink` you may receive a response again containing the same group object.</span></span> <span data-ttu-id="067b4-174">同じプロパティ値が返されますが、展開された `members@delta` プロパティの内容は、異なるユーザー リストになっています。</span><span class="sxs-lookup"><span data-stu-id="067b4-174">The same property values will be returned but the expanded `members@delta` property now contains a different list of users.</span></span>

<span data-ttu-id="067b4-175">**2 番目のページ**</span><span class="sxs-lookup"><span data-stu-id="067b4-175">**Second page**</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "c08a463b-7b8a-40a4-aa31-f9bf690b9551",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "23423fa6-821e-44b2-aae4-d039d33884c2"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

3. <span data-ttu-id="067b4-176">このようにしてメンバー リスト全体が返され、他のグループが応答に出現し始めます。</span><span class="sxs-lookup"><span data-stu-id="067b4-176">Eventually, the entire member list will be returned in this fashion, and other groups will start showing up in the response.</span></span>

<span data-ttu-id="067b4-177">このパターンを処理する際には、次のベスト プラクティスに従うことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="067b4-177">We recommend the following best practices to correctly handle this pattern:</span></span>
- <span data-ttu-id="067b4-178">常に `nextLink` をたどり、各グループの状態をローカルでマージします。同じグループに関連する複数の応答を受信したなら、アプリケーションの中でその応答を使用してメンバーシップ リスト全体を作成します。</span><span class="sxs-lookup"><span data-stu-id="067b4-178">Always follow `nextLink` and locally merge each group's state: as you receive responses related to the same group, use them to build the full membership list in your application.</span></span>
- <span data-ttu-id="067b4-179">特定の応答シーケンスを前提にしないようにするのが最善です。</span><span class="sxs-lookup"><span data-stu-id="067b4-179">It is best not to assume a specific sequence of the responses.</span></span> <span data-ttu-id="067b4-180">`nextLink` シーケンスのどこにでも同じグループが出現する可能性があると想定し、マージ ロジックの中でそれを処理します。</span><span class="sxs-lookup"><span data-stu-id="067b4-180">Assume that the same group could show up anywhere in the `nextLink` sequence and handle that in your merge logic.</span></span>


## <a name="see-also"></a><span data-ttu-id="067b4-181">関連項目</span><span class="sxs-lookup"><span data-stu-id="067b4-181">See also</span></span>
<span data-ttu-id="067b4-182">[Microsoft Graph デルタ クエリ](delta-query-overview.md)の概要。</span><span class="sxs-lookup"><span data-stu-id="067b4-182">[Microsoft Graph delta query](delta-query-overview.md) overview.</span></span>
