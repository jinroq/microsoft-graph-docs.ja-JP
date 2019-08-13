---
title: 'group: delta'
description: グループメンバーシップの変更を含む、新しく作成、更新、または削除されたグループを取得します。グループコレクション全体の完全な読み取りを実行する必要はありません。 詳細については、「デルタクエリの使用」を参照してください。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bb95f0a3bb94dd9583fd06d98916ce6b9feea4ec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326416"
---
# <a name="group-delta"></a><span data-ttu-id="b473a-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="b473a-104">group: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b473a-105">グループメンバーシップの変更を含む、新しく作成、更新、または削除されたグループを取得します。グループコレクション全体の完全な読み取りを実行する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="b473a-105">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="b473a-106">詳細については、「[デルタクエリの使用](/graph/delta-query-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b473a-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="b473a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b473a-107">Permissions</span></span>

<span data-ttu-id="b473a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b473a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b473a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b473a-110">Permission type</span></span>      | <span data-ttu-id="b473a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b473a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b473a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b473a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b473a-113">Directory.accessasuser.all。すべて、ディレクトリの読み取り、すべてのディレクトリを読み取ることができます。すべてを示します。.</span><span class="sxs-lookup"><span data-stu-id="b473a-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="b473a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b473a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b473a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b473a-115">Not supported.</span></span>    |
|<span data-ttu-id="b473a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b473a-116">Application</span></span> | <span data-ttu-id="b473a-117">。すべて、ディレクトリの読み取り、すべてのディレクトリの読み取り、すべてのディレクトリを取得します。</span><span class="sxs-lookup"><span data-stu-id="b473a-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b473a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b473a-118">HTTP request</span></span>

<span data-ttu-id="b473a-119">変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="b473a-119">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="b473a-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b473a-120">Query parameters</span></span>

<span data-ttu-id="b473a-p104">グループで変更の追跡を実行するときには、1 つまたは複数の **delta** 関数の呼び出しが必要になります。クエリ パラメーター (`$deltatoken` および `$skiptoken` 以外) を使用する場合は、そのパラメーターを最初の **delta** 要求に指定する必要があります。指定されたパラメーターは、Microsoft Graph を使って自動的にエンコードされ、応答の `nextLink` または `deltaLink` URL のトークン部分として指定されます。</span><span class="sxs-lookup"><span data-stu-id="b473a-p104">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="b473a-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="b473a-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="b473a-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="b473a-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="b473a-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b473a-126">Query parameter</span></span> | <span data-ttu-id="b473a-127">種類</span><span class="sxs-lookup"><span data-stu-id="b473a-127">Type</span></span>  |<span data-ttu-id="b473a-128">説明</span><span class="sxs-lookup"><span data-stu-id="b473a-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b473a-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="b473a-129">$deltatoken</span></span> | <span data-ttu-id="b473a-130">string</span><span class="sxs-lookup"><span data-stu-id="b473a-130">string</span></span> | <span data-ttu-id="b473a-p105">同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="b473a-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="b473a-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="b473a-133">$skiptoken</span></span> | <span data-ttu-id="b473a-134">string</span><span class="sxs-lookup"><span data-stu-id="b473a-134">string</span></span> | <span data-ttu-id="b473a-135">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="b473a-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="b473a-136">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b473a-136">OData query parameters</span></span>

<span data-ttu-id="b473a-137">このメソッドは、応答をカスタマイズするためのオプションの OData クエリパラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="b473a-137">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="b473a-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="b473a-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="b473a-140">を使用`$expand=members`して、メンバーシップの変更を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="b473a-140">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="b473a-141">`$filter` に対するサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="b473a-141">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="b473a-142">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="b473a-142">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="b473a-143">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="b473a-143">You can filter multiple objects.</span></span> <span data-ttu-id="b473a-144">たとえば、`https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。</span><span class="sxs-lookup"><span data-stu-id="b473a-144">For example, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="b473a-145">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="b473a-145">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b473a-146">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b473a-146">Request headers</span></span>

| <span data-ttu-id="b473a-147">名前</span><span class="sxs-lookup"><span data-stu-id="b473a-147">Name</span></span>       | <span data-ttu-id="b473a-148">説明</span><span class="sxs-lookup"><span data-stu-id="b473a-148">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b473a-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="b473a-149">Authorization</span></span>  | <span data-ttu-id="b473a-150">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="b473a-150">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="b473a-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b473a-151">Content-Type</span></span>  | <span data-ttu-id="b473a-152">application/json</span><span class="sxs-lookup"><span data-stu-id="b473a-152">application/json</span></span> |
| <span data-ttu-id="b473a-153">Prefer</span><span class="sxs-lookup"><span data-stu-id="b473a-153">Prefer</span></span> | <span data-ttu-id="b473a-154">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="b473a-154">return=minimal</span></span> <br><br><span data-ttu-id="b473a-155">このヘッダーを指定する要求を使用すると、`deltaLink` は、最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="b473a-155">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="b473a-156">省略可能です。</span><span class="sxs-lookup"><span data-stu-id="b473a-156">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b473a-157">要求本文</span><span class="sxs-lookup"><span data-stu-id="b473a-157">Request body</span></span>

<span data-ttu-id="b473a-158">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b473a-158">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="b473a-159">応答</span><span class="sxs-lookup"><span data-stu-id="b473a-159">Response</span></span>

<span data-ttu-id="b473a-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b473a-160">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="b473a-161">応答には、 `nextLink` url または`deltaLink` url のいずれかの状態トークンも含まれます。</span><span class="sxs-lookup"><span data-stu-id="b473a-161">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="b473a-162">もし`nextLink` URL が返された場合:</span><span class="sxs-lookup"><span data-stu-id="b473a-162">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="b473a-163">セッションで取得するデータに追加ページがあることを示しています。</span><span class="sxs-lookup"><span data-stu-id="b473a-163">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="b473a-164">アプリケーションは`deltaLink` URL が応答に含まれるまで`nextLink` URLを使用して要求を続けます。</span><span class="sxs-lookup"><span data-stu-id="b473a-164">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="b473a-165">応答には、最初のデルタクエリ要求と同じ一連のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b473a-165">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="b473a-166">これにより、デルタサイクルを開始するときに、オブジェクトの現在の完全な状態をキャプチャできます。</span><span class="sxs-lookup"><span data-stu-id="b473a-166">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="b473a-167">もし`deltaLink` URL が返された場合:</span><span class="sxs-lookup"><span data-stu-id="b473a-167">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="b473a-168">これは、返されるリソースの既存の状態に関するデータがこれ以上ないことを示します。</span><span class="sxs-lookup"><span data-stu-id="b473a-168">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="b473a-169">`deltaLink` URL を、次回のラウンドでリソースへの変更について学ぶために保存して使ってください。</span><span class="sxs-lookup"><span data-stu-id="b473a-169">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="b473a-170">`Prefer:return=minimal` ヘッダーを指定して、`deltaLink`発行後に変更されたプロパティのみをレスポンス値に含めるように選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="b473a-170">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="b473a-171">デフォルト：初期デルタリクエストと同じプロパティを返します</span><span class="sxs-lookup"><span data-stu-id="b473a-171">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="b473a-172">デフォルトでは、`deltaLink`または`nextLink`を使用したリクエストは、最初のデルタクエリで選択されたものと同じプロパティを次のように返します:</span><span class="sxs-lookup"><span data-stu-id="b473a-172">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="b473a-173">プロパティを変更した場合は、応答には新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b473a-173">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="b473a-174">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b473a-174">This includes properties being set to null value.</span></span>
- <span data-ttu-id="b473a-175">プロパティが変更されていない場合は、古い値が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="b473a-175">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="b473a-176">プロパティが設定されたことがない場合は、応答にまったく含まれません。</span><span class="sxs-lookup"><span data-stu-id="b473a-176">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="b473a-177">**注意:** この動作では、応答を見ても、プロパティが変化しているかどうかを判断することはできません。</span><span class="sxs-lookup"><span data-stu-id="b473a-177">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="b473a-178">また、デルタ応答は-以下の[2番目の例](#request-2)に示されるようにすべてのプロパティ値を含むため、大きくなる傾向があります 。</span><span class="sxs-lookup"><span data-stu-id="b473a-178">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="b473a-179">代替案：変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="b473a-179">Alternative: return only the changed properties</span></span>

<span data-ttu-id="b473a-180">オプションのリクエストヘッダを追加すると、- `prefer:return=minimal` - 次のようになります:</span><span class="sxs-lookup"><span data-stu-id="b473a-180">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="b473a-181">プロパティを変更した場合は、応答には新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b473a-181">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="b473a-182">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b473a-182">This includes properties being set to null value.</span></span>
- <span data-ttu-id="b473a-183">プロパティが変更されていない場合、そのプロパティは応答にまったく含まれません。</span><span class="sxs-lookup"><span data-stu-id="b473a-183">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="b473a-184">(既定の動作と異なる)</span><span class="sxs-lookup"><span data-stu-id="b473a-184">(Different from the default behavior.)</span></span>

> <span data-ttu-id="b473a-185">**注意:** ヘッダーは、デルタサイクルのどの時点でも `deltaLink`要求に追加できます。</span><span class="sxs-lookup"><span data-stu-id="b473a-185">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="b473a-186">ヘッダーは応答に含まれる一連のプロパティにのみ影響し、デルタクエリの実行方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="b473a-186">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="b473a-187">以下の[三番目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b473a-187">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="b473a-188">例</span><span class="sxs-lookup"><span data-stu-id="b473a-188">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="b473a-189">要求 1</span><span class="sxs-lookup"><span data-stu-id="b473a-189">Request 1</span></span>

<span data-ttu-id="b473a-190">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b473a-190">The following is an example of the request.</span></span> <span data-ttu-id="b473a-191">`$select`パラメータがないため、デフォルトのプロパティセットが追跡されて返されます。</span><span class="sxs-lookup"><span data-stu-id="b473a-191">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b473a-192">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b473a-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b473a-193">C#</span><span class="sxs-lookup"><span data-stu-id="b473a-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b473a-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b473a-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b473a-195">目的-C</span><span class="sxs-lookup"><span data-stu-id="b473a-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b473a-196">Java</span><span class="sxs-lookup"><span data-stu-id="b473a-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-1"></a><span data-ttu-id="b473a-197">応答 1</span><span class="sxs-lookup"><span data-stu-id="b473a-197">Response 1</span></span>

<span data-ttu-id="b473a-198">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b473a-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="b473a-199">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b473a-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b473a-200">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b473a-200">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="b473a-201">グループ内の member オブジェクトの id を含む*メンバー @ delta*プロパティが存在することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b473a-201">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
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
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="b473a-202">要求 2</span><span class="sxs-lookup"><span data-stu-id="b473a-202">Request 2</span></span>

<span data-ttu-id="b473a-203">次の例は、デフォルトの応答動作で、変更追跡のために3つのプロパティを選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="b473a-203">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b473a-204">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b473a-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_with_selelct"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b473a-205">C#</span><span class="sxs-lookup"><span data-stu-id="b473a-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-with-selelct-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b473a-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b473a-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-with-selelct-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b473a-207">目的-C</span><span class="sxs-lookup"><span data-stu-id="b473a-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-with-selelct-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b473a-208">Java</span><span class="sxs-lookup"><span data-stu-id="b473a-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-with-selelct-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="b473a-209">応答 2</span><span class="sxs-lookup"><span data-stu-id="b473a-209">Response 2</span></span>

<span data-ttu-id="b473a-210">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b473a-210">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="b473a-211">3つのプロパティすべてがレスポンスに含まれており、`deltaLink`が取得されてからどのプロパティが変更されたのかはわかりません。</span><span class="sxs-lookup"><span data-stu-id="b473a-211">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="b473a-212">要求 3</span><span class="sxs-lookup"><span data-stu-id="b473a-212">Request 3</span></span>

<span data-ttu-id="b473a-213">次の例は、最初のリクエストが代替の最小限の応答の変更追跡のために3つのプロパティを選択していることを示しています。</span><span class="sxs-lookup"><span data-stu-id="b473a-213">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b473a-214">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b473a-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_minimal"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b473a-215">C#</span><span class="sxs-lookup"><span data-stu-id="b473a-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b473a-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b473a-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b473a-217">目的-C</span><span class="sxs-lookup"><span data-stu-id="b473a-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b473a-218">Java</span><span class="sxs-lookup"><span data-stu-id="b473a-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-3"></a><span data-ttu-id="b473a-219">応答 3</span><span class="sxs-lookup"><span data-stu-id="b473a-219">Response 3</span></span>

<span data-ttu-id="b473a-220">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b473a-220">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="b473a-221">この`mailNickname`プロパティは含まれていないことに注意してください 。つまり、最後のデルタクエリ以降変更されていません;`displayName`と`description` が含まれており、それらの値は変更されていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="b473a-221">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="b473a-222">関連項目</span><span class="sxs-lookup"><span data-stu-id="b473a-222">See also</span></span>

- <span data-ttu-id="b473a-223">[デルタクエリを使用してMicrosoft Graphデータの変更を追跡します](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="b473a-223">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="b473a-224">[グループに対する増分の変更を取得](/graph/delta-query-groups)します。</span><span class="sxs-lookup"><span data-stu-id="b473a-224">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
