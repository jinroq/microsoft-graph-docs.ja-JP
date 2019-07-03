---
title: 'user: delta'
description: ユーザーコレクション全体を完全に読み取ることなく、新しく作成、更新、または削除されたユーザーを取得します。 詳細は変更の追跡をご覧ください。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3f6d940617e85715b1986f417993d956eab283c0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450892"
---
# <a name="user-delta"></a><span data-ttu-id="1006e-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="1006e-104">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1006e-105">ユーザーコレクション全体を完全に読み取ることなく、新しく作成、更新、または削除されたユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="1006e-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="1006e-106">詳細は.、[変更の追跡](/graph/delta-query-overview)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1006e-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="1006e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1006e-107">Permissions</span></span>

<span data-ttu-id="1006e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1006e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1006e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1006e-110">Permission type</span></span>      | <span data-ttu-id="1006e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1006e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1006e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1006e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1006e-113">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1006e-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1006e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1006e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1006e-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1006e-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="1006e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1006e-116">Application</span></span> | <span data-ttu-id="1006e-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1006e-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1006e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1006e-118">HTTP request</span></span>

<span data-ttu-id="1006e-119">変更の追跡を開始するには、ユーザー リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="1006e-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="1006e-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1006e-120">Query parameters</span></span>

<span data-ttu-id="1006e-121">ユーザーの変更を追跡すると、一連の **デルタ**関数の呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="1006e-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="1006e-122">任意のクエリ パラメーター (`$deltatoken` と`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1006e-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="1006e-123">Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。</span><span class="sxs-lookup"><span data-stu-id="1006e-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="1006e-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="1006e-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="1006e-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="1006e-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="1006e-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1006e-126">Query parameter</span></span>      | <span data-ttu-id="1006e-127">種類</span><span class="sxs-lookup"><span data-stu-id="1006e-127">Type</span></span>   |<span data-ttu-id="1006e-128">説明</span><span class="sxs-lookup"><span data-stu-id="1006e-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1006e-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="1006e-129">$deltatoken</span></span> | <span data-ttu-id="1006e-130">string</span><span class="sxs-lookup"><span data-stu-id="1006e-130">string</span></span> | <span data-ttu-id="1006e-p105">同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="1006e-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="1006e-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="1006e-133">$skiptoken</span></span> | <span data-ttu-id="1006e-134">string</span><span class="sxs-lookup"><span data-stu-id="1006e-134">string</span></span> | <span data-ttu-id="1006e-135">前の**デルタ**関数の `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。</span><span class="sxs-lookup"><span data-stu-id="1006e-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="1006e-136">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1006e-136">OData query parameters</span></span>

<span data-ttu-id="1006e-137">このメソッドは、応答をカスタマイズするためのオプショナルの OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="1006e-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="1006e-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="1006e-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="1006e-140">`$filter` に対するサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="1006e-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="1006e-141">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="1006e-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="1006e-142">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="1006e-142">You can filter multiple objects.</span></span> <span data-ttu-id="1006e-143">たとえば、`https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。</span><span class="sxs-lookup"><span data-stu-id="1006e-143">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="1006e-144">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="1006e-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1006e-145">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1006e-145">Request headers</span></span>
| <span data-ttu-id="1006e-146">名前</span><span class="sxs-lookup"><span data-stu-id="1006e-146">Name</span></span>       | <span data-ttu-id="1006e-147">説明</span><span class="sxs-lookup"><span data-stu-id="1006e-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1006e-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="1006e-148">Authorization</span></span>  | <span data-ttu-id="1006e-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="1006e-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="1006e-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1006e-150">Content-Type</span></span>  | <span data-ttu-id="1006e-151">application/json</span><span class="sxs-lookup"><span data-stu-id="1006e-151">application/json</span></span> |
| <span data-ttu-id="1006e-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="1006e-152">Prefer</span></span> | <span data-ttu-id="1006e-153">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="1006e-153">return=minimal</span></span> <br><br><span data-ttu-id="1006e-154">このヘッダーを指定する要求を使用すると、`deltaLink` は、最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="1006e-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="1006e-155">省略可能です。</span><span class="sxs-lookup"><span data-stu-id="1006e-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1006e-156">要求本文</span><span class="sxs-lookup"><span data-stu-id="1006e-156">Request body</span></span>
<span data-ttu-id="1006e-157">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1006e-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="1006e-158">応答</span><span class="sxs-lookup"><span data-stu-id="1006e-158">Response</span></span>

<span data-ttu-id="1006e-159">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1006e-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="1006e-160">応答には`nextLink` URLまたは`deltaLink` URLも含まれます。</span><span class="sxs-lookup"><span data-stu-id="1006e-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="1006e-161">もし`nextLink` URL が返された場合:</span><span class="sxs-lookup"><span data-stu-id="1006e-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="1006e-162">セッションで取得するデータに追加ページがあることを示しています。</span><span class="sxs-lookup"><span data-stu-id="1006e-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="1006e-163">アプリケーションは`deltaLink` URL が応答に含まれるまで`nextLink` URLを使用して要求を続けます。</span><span class="sxs-lookup"><span data-stu-id="1006e-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="1006e-164">応答には、最初のデルタクエリ要求と同じ一連のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1006e-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="1006e-165">これにより、デルタサイクルを開始するときに、オブジェクトの現在の完全な状態をキャプチャできます。</span><span class="sxs-lookup"><span data-stu-id="1006e-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="1006e-166">もし`deltaLink` URL が返された場合:</span><span class="sxs-lookup"><span data-stu-id="1006e-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="1006e-167">これは、返されるリソースの既存の状態に関するデータがこれ以上ないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1006e-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="1006e-168">`deltaLink` URL を、次回のラウンドでリソースへの変更について学ぶために保存して使ってください。</span><span class="sxs-lookup"><span data-stu-id="1006e-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="1006e-169">`Prefer:return=minimal` ヘッダーを指定して、`deltaLink`発行後に変更されたプロパティのみをレスポンス値に含めるように選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="1006e-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="1006e-170">デフォルト：初期デルタリクエストと同じプロパティを返します</span><span class="sxs-lookup"><span data-stu-id="1006e-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="1006e-171">デフォルトでは、`deltaLink`または`nextLink`を使用したリクエストは、最初のデルタクエリで選択されたものと同じプロパティを次のように返します:</span><span class="sxs-lookup"><span data-stu-id="1006e-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="1006e-172">プロパティを変更した場合は、応答には新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1006e-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="1006e-173">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="1006e-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="1006e-174">プロパティが変更されていない場合は、古い値が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="1006e-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="1006e-175">プロパティが設定されたことがない場合は、応答にまったく含まれません。</span><span class="sxs-lookup"><span data-stu-id="1006e-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="1006e-176">**注意:** この動作では、応答を見ても、プロパティが変化しているかどうかを判断することはできません。</span><span class="sxs-lookup"><span data-stu-id="1006e-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="1006e-177">また、デルタ応答は-以下の[2番目の例](#request-2)に示されるようにすべてのプロパティ値を含むため、大きくなる傾向があります 。</span><span class="sxs-lookup"><span data-stu-id="1006e-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="1006e-178">代替案：変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="1006e-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="1006e-179">オプションのリクエストヘッダを追加すると、- `prefer:return=minimal` - 次のようになります:</span><span class="sxs-lookup"><span data-stu-id="1006e-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="1006e-180">プロパティを変更した場合は、応答には新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1006e-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="1006e-181">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="1006e-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="1006e-182">プロパティが変更されていない場合、そのプロパティは応答にまったく含まれません。</span><span class="sxs-lookup"><span data-stu-id="1006e-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="1006e-183">(既定の動作と異なる)</span><span class="sxs-lookup"><span data-stu-id="1006e-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="1006e-184">**注意:** ヘッダーは、デルタサイクルのどの時点でも `deltaLink`要求に追加できます。</span><span class="sxs-lookup"><span data-stu-id="1006e-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="1006e-185">ヘッダーは応答に含まれる一連のプロパティにのみ影響し、デルタクエリの実行方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="1006e-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="1006e-186">以下の[三番目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1006e-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="1006e-187">例</span><span class="sxs-lookup"><span data-stu-id="1006e-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="1006e-188">要求 1</span><span class="sxs-lookup"><span data-stu-id="1006e-188">Request 1</span></span>

<span data-ttu-id="1006e-189">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1006e-189">The following is an example of the request.</span></span> <span data-ttu-id="1006e-190">`$select`パラメータがないため、デフォルトのプロパティセットが追跡されて返されます。</span><span class="sxs-lookup"><span data-stu-id="1006e-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1006e-191">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1006e-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1006e-192">C#</span><span class="sxs-lookup"><span data-stu-id="1006e-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1006e-193">Javascript</span><span class="sxs-lookup"><span data-stu-id="1006e-193">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1006e-194">目的-C</span><span class="sxs-lookup"><span data-stu-id="1006e-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-1"></a><span data-ttu-id="1006e-195">応答 1</span><span class="sxs-lookup"><span data-stu-id="1006e-195">Response 1</span></span>

<span data-ttu-id="1006e-196">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1006e-196">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="1006e-p119">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1006e-p119">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="1006e-199">要求 2</span><span class="sxs-lookup"><span data-stu-id="1006e-199">Request 2</span></span>

<span data-ttu-id="1006e-200">次の例は、デフォルトの応答動作で、変更追跡のために3つのプロパティを選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="1006e-200">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1006e-201">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1006e-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_select"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1006e-202">C#</span><span class="sxs-lookup"><span data-stu-id="1006e-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1006e-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="1006e-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1006e-204">目的-C</span><span class="sxs-lookup"><span data-stu-id="1006e-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="1006e-205">応答 2</span><span class="sxs-lookup"><span data-stu-id="1006e-205">Response 2</span></span>

<span data-ttu-id="1006e-206">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1006e-206">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="1006e-207">3つのプロパティすべてがレスポンスに含まれており、`deltaLink`が取得されてからどのプロパティが変更されたのかはわかりません。</span><span class="sxs-lookup"><span data-stu-id="1006e-207">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="1006e-208">要求 3</span><span class="sxs-lookup"><span data-stu-id="1006e-208">Request 3</span></span>

<span data-ttu-id="1006e-209">次の例は、最初のリクエストが代替の最小限の応答の変更追跡のために3つのプロパティを選択していることを示しています。</span><span class="sxs-lookup"><span data-stu-id="1006e-209">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1006e-210">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1006e-210">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_minimal"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1006e-211">C#</span><span class="sxs-lookup"><span data-stu-id="1006e-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1006e-212">Javascript</span><span class="sxs-lookup"><span data-stu-id="1006e-212">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1006e-213">目的-C</span><span class="sxs-lookup"><span data-stu-id="1006e-213">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-3"></a><span data-ttu-id="1006e-214">応答 3</span><span class="sxs-lookup"><span data-stu-id="1006e-214">Response 3</span></span>

<span data-ttu-id="1006e-215">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1006e-215">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="1006e-216">この`mobilePhone`プロパティは含まれていないことに注意してください 。つまり、最後のデルタクエリ以降変更されていません;`displayName`と`jobTitle` が含まれており、それらの値は変更されていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="1006e-216">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- <span data-ttu-id="1006e-217">[デルタクエリを使用してMicrosoft Graphデータの変更を追跡します](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="1006e-217">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="1006e-218">[ユーザーの増分変更を取得します](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="1006e-218">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
