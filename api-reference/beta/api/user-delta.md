---
title: 'user: delta'
description: ユーザーコレクション全体を完全に読み取ることなく、新しく作成、更新、または削除されたユーザーを取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac4b3229f9057f6f310db64e6f23e1e9edd9d924
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996519"
---
# <a name="user-delta"></a><span data-ttu-id="e9a17-103">user: delta</span><span class="sxs-lookup"><span data-stu-id="e9a17-103">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9a17-104">ユーザーコレクション全体を完全に読み取ることなく、新しく作成、更新、または削除されたユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-104">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="e9a17-105">詳細は.、[変更の追跡](/graph/delta-query-overview)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e9a17-105">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9a17-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e9a17-106">Permissions</span></span>

<span data-ttu-id="e9a17-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9a17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e9a17-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e9a17-109">Permission type</span></span>      | <span data-ttu-id="e9a17-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e9a17-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9a17-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e9a17-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9a17-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9a17-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e9a17-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e9a17-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9a17-114">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9a17-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="e9a17-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e9a17-115">Application</span></span> | <span data-ttu-id="e9a17-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9a17-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9a17-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e9a17-117">HTTP request</span></span>

<span data-ttu-id="e9a17-118">変更の追跡を開始するには、ユーザー リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-118">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="e9a17-119">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e9a17-119">Query parameters</span></span>

<span data-ttu-id="e9a17-120">ユーザーの変更を追跡すると、一連の **デルタ**関数の呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-120">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="e9a17-121">任意のクエリ パラメーター (`$deltatoken` と`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e9a17-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="e9a17-122">Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。</span><span class="sxs-lookup"><span data-stu-id="e9a17-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="e9a17-123">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-123">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="e9a17-124">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="e9a17-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="e9a17-125">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e9a17-125">Query parameter</span></span>      | <span data-ttu-id="e9a17-126">種類</span><span class="sxs-lookup"><span data-stu-id="e9a17-126">Type</span></span>   |<span data-ttu-id="e9a17-127">説明</span><span class="sxs-lookup"><span data-stu-id="e9a17-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9a17-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="e9a17-128">$deltatoken</span></span> | <span data-ttu-id="e9a17-129">string</span><span class="sxs-lookup"><span data-stu-id="e9a17-129">string</span></span> | <span data-ttu-id="e9a17-p104">同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="e9a17-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e9a17-132">$skiptoken</span></span> | <span data-ttu-id="e9a17-133">string</span><span class="sxs-lookup"><span data-stu-id="e9a17-133">string</span></span> | <span data-ttu-id="e9a17-134">前の**デルタ**関数の `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="e9a17-135">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e9a17-135">OData query parameters</span></span>

<span data-ttu-id="e9a17-136">このメソッドは、応答をカスタマイズするためのオプショナルの OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="e9a17-136">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="e9a17-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="e9a17-139">`$filter` に対するサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="e9a17-139">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="e9a17-140">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="e9a17-140">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="e9a17-141">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-141">You can filter multiple objects.</span></span> <span data-ttu-id="e9a17-142">たとえば、`https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。</span><span class="sxs-lookup"><span data-stu-id="e9a17-142">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="e9a17-143">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="e9a17-143">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9a17-144">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9a17-144">Request headers</span></span>
| <span data-ttu-id="e9a17-145">名前</span><span class="sxs-lookup"><span data-stu-id="e9a17-145">Name</span></span>       | <span data-ttu-id="e9a17-146">説明</span><span class="sxs-lookup"><span data-stu-id="e9a17-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e9a17-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9a17-147">Authorization</span></span>  | <span data-ttu-id="e9a17-148">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="e9a17-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="e9a17-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9a17-149">Content-Type</span></span>  | <span data-ttu-id="e9a17-150">application/json</span><span class="sxs-lookup"><span data-stu-id="e9a17-150">application/json</span></span> |
| <span data-ttu-id="e9a17-151">Prefer</span><span class="sxs-lookup"><span data-stu-id="e9a17-151">Prefer</span></span> | <span data-ttu-id="e9a17-152">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="e9a17-152">return=minimal</span></span> <br><br><span data-ttu-id="e9a17-153">このヘッダーを指定する要求を使用すると、`deltaLink` は、最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-153">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="e9a17-154">省略可能です。</span><span class="sxs-lookup"><span data-stu-id="e9a17-154">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9a17-155">要求本文</span><span class="sxs-lookup"><span data-stu-id="e9a17-155">Request body</span></span>
<span data-ttu-id="e9a17-156">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e9a17-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9a17-157">応答</span><span class="sxs-lookup"><span data-stu-id="e9a17-157">Response</span></span>

<span data-ttu-id="e9a17-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-158">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="e9a17-159">応答には`nextLink` URLまたは`deltaLink` URLも含まれます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-159">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="e9a17-160">もし`nextLink` URL が返された場合:</span><span class="sxs-lookup"><span data-stu-id="e9a17-160">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="e9a17-161">セッションで取得するデータに追加ページがあることを示しています。</span><span class="sxs-lookup"><span data-stu-id="e9a17-161">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="e9a17-162">アプリケーションは`deltaLink` URL が応答に含まれるまで`nextLink` URLを使用して要求を続けます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-162">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="e9a17-163">応答には、最初のデルタクエリ要求と同じ一連のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9a17-163">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="e9a17-164">これにより、デルタサイクルを開始するときに、オブジェクトの現在の完全な状態をキャプチャできます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-164">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="e9a17-165">もし`deltaLink` URL が返された場合:</span><span class="sxs-lookup"><span data-stu-id="e9a17-165">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="e9a17-166">これは、返されるリソースの既存の状態に関するデータがこれ以上ないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-166">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="e9a17-167">`deltaLink` URL を、次回のラウンドでリソースへの変更について学ぶために保存して使ってください。</span><span class="sxs-lookup"><span data-stu-id="e9a17-167">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="e9a17-168">`Prefer:return=minimal` ヘッダーを指定して、`deltaLink`発行後に変更されたプロパティのみをレスポンス値に含めるように選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-168">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="e9a17-169">デフォルト：初期デルタリクエストと同じプロパティを返します</span><span class="sxs-lookup"><span data-stu-id="e9a17-169">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="e9a17-170">デフォルトでは、`deltaLink`または`nextLink`を使用したリクエストは、最初のデルタクエリで選択されたものと同じプロパティを次のように返します:</span><span class="sxs-lookup"><span data-stu-id="e9a17-170">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="e9a17-171">プロパティを変更した場合は、応答には新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-171">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="e9a17-172">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-172">This includes properties being set to null value.</span></span>
- <span data-ttu-id="e9a17-173">プロパティが変更されていない場合は、古い値が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9a17-173">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="e9a17-174">プロパティが設定されたことがない場合は、応答にまったく含まれません。</span><span class="sxs-lookup"><span data-stu-id="e9a17-174">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="e9a17-175">**注意:** この動作では、応答を見ても、プロパティが変化しているかどうかを判断することはできません。</span><span class="sxs-lookup"><span data-stu-id="e9a17-175">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="e9a17-176">また、デルタ応答は、[例 2](#example-2-selecting-three-properties)に示すように、すべてのプロパティ値を含むため、サイズが大きくなる傾向があります。</span><span class="sxs-lookup"><span data-stu-id="e9a17-176">Also, the delta responses tend to be large because they contain all property values  - as shown in [Example 2](#example-2-selecting-three-properties).</span></span>

### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="e9a17-177">代替案：変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="e9a17-177">Alternative: return only the changed properties</span></span>

<span data-ttu-id="e9a17-178">オプションのリクエストヘッダを追加すると、- `prefer:return=minimal` - 次のようになります:</span><span class="sxs-lookup"><span data-stu-id="e9a17-178">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="e9a17-179">プロパティを変更した場合は、応答には新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-179">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="e9a17-180">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-180">This includes properties being set to null value.</span></span>
- <span data-ttu-id="e9a17-181">プロパティが変更されていない場合、そのプロパティは応答にまったく含まれません。</span><span class="sxs-lookup"><span data-stu-id="e9a17-181">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="e9a17-182">(既定の動作と異なる)</span><span class="sxs-lookup"><span data-stu-id="e9a17-182">(Different from the default behavior.)</span></span>

> <span data-ttu-id="e9a17-183">**注意:** ヘッダーは、デルタサイクルのどの時点でも `deltaLink`要求に追加できます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-183">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="e9a17-184">ヘッダーは応答に含まれる一連のプロパティにのみ影響し、デルタクエリの実行方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="e9a17-184">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="e9a17-185">[例 3](#example-3-alternative-minimal-response-behavior)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9a17-185">See [Example 3](#example-3-alternative-minimal-response-behavior).</span></span>

## <a name="examples"></a><span data-ttu-id="e9a17-186">例</span><span class="sxs-lookup"><span data-stu-id="e9a17-186">Examples</span></span>

### <a name="example-1-default-properties"></a><span data-ttu-id="e9a17-187">例 1: 既定のプロパティ</span><span class="sxs-lookup"><span data-stu-id="e9a17-187">Example 1: Default properties</span></span>

#### <a name="request"></a><span data-ttu-id="e9a17-188">要求</span><span class="sxs-lookup"><span data-stu-id="e9a17-188">Request</span></span>

<span data-ttu-id="e9a17-189">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-189">The following is an example of the request.</span></span> <span data-ttu-id="e9a17-190">`$select`パラメータがないため、デフォルトのプロパティセットが追跡されて返されます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e9a17-191">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e9a17-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9a17-192">C#</span><span class="sxs-lookup"><span data-stu-id="e9a17-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9a17-193">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9a17-193">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9a17-194">目的-C</span><span class="sxs-lookup"><span data-stu-id="e9a17-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e9a17-195">Java</span><span class="sxs-lookup"><span data-stu-id="e9a17-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9a17-196">応答</span><span class="sxs-lookup"><span data-stu-id="e9a17-196">Response</span></span>

<span data-ttu-id="e9a17-197">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e9a17-197">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="e9a17-p118">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e9a17-p118">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-selecting-three-properties"></a><span data-ttu-id="e9a17-200">例 2: 3 つのプロパティの選択</span><span class="sxs-lookup"><span data-stu-id="e9a17-200">Example 2: Selecting three properties</span></span>

#### <a name="request"></a><span data-ttu-id="e9a17-201">要求</span><span class="sxs-lookup"><span data-stu-id="e9a17-201">Request</span></span>

<span data-ttu-id="e9a17-202">次の例は、既定の応答動作を使用して、変更追跡の3つのプロパティを選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="e9a17-202">The next example shows the initial request selecting three properties for change tracking, with default response behavior.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e9a17-203">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e9a17-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_select"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9a17-204">C#</span><span class="sxs-lookup"><span data-stu-id="e9a17-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9a17-205">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9a17-205">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9a17-206">目的-C</span><span class="sxs-lookup"><span data-stu-id="e9a17-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e9a17-207">Java</span><span class="sxs-lookup"><span data-stu-id="e9a17-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9a17-208">応答</span><span class="sxs-lookup"><span data-stu-id="e9a17-208">Response</span></span>

<span data-ttu-id="e9a17-209">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e9a17-209">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e9a17-210">3つのプロパティはすべて応答に含まれており、 `deltaLink`取得した後に変更されたプロパティが不明であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="e9a17-210">Note that all three properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

### <a name="example-3-alternative-minimal-response-behavior"></a><span data-ttu-id="e9a17-211">例 3: 代替の最小応答動作</span><span class="sxs-lookup"><span data-stu-id="e9a17-211">Example 3: Alternative minimal response behavior</span></span>

#### <a name="request"></a><span data-ttu-id="e9a17-212">要求</span><span class="sxs-lookup"><span data-stu-id="e9a17-212">Request</span></span>

<span data-ttu-id="e9a17-213">次の例は、変更追跡のために3つのプロパティを選択する最初の要求を示しています。これには、別の最低限の応答動作があります。</span><span class="sxs-lookup"><span data-stu-id="e9a17-213">The next example shows the initial request selecting three properties for change tracking, with alternative minimal response behavior.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e9a17-214">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e9a17-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_minimal"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9a17-215">C#</span><span class="sxs-lookup"><span data-stu-id="e9a17-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9a17-216">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9a17-216">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9a17-217">目的-C</span><span class="sxs-lookup"><span data-stu-id="e9a17-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e9a17-218">Java</span><span class="sxs-lookup"><span data-stu-id="e9a17-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9a17-219">応答</span><span class="sxs-lookup"><span data-stu-id="e9a17-219">Response</span></span>

<span data-ttu-id="e9a17-220">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e9a17-220">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e9a17-221">この`mobilePhone`プロパティは含まれていないことに注意してください 。つまり、最後のデルタクエリ以降変更されていません;`displayName`と`jobTitle` が含まれており、それらの値は変更されていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="e9a17-221">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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
## <a name="see-also"></a><span data-ttu-id="e9a17-222">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9a17-222">See also</span></span>

- <span data-ttu-id="e9a17-223">[デルタクエリを使用してMicrosoft Graphデータの変更を追跡します](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="e9a17-223">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="e9a17-224">[ユーザーの増分変更を取得します](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="e9a17-224">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
