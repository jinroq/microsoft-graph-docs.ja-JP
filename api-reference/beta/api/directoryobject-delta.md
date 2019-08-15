---
title: 'directoryObject: delta'
description: 単一のデルタクエリで、次の種類の新規作成、更新、または削除されたディレクトリオブジェクトを取得します。ユーザー、グループ、組織の連絡先。 詳細は変更の追跡をご覧ください。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cd3bdefee1877283a9ffcac8864e7fea47f55170
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417446"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="9d01f-104">directoryObject: delta</span><span class="sxs-lookup"><span data-stu-id="9d01f-104">directoryObject: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d01f-105">単一のデルタクエリで、次の種類の新規作成、更新、または削除されたディレクトリオブジェクトを取得します。[ユーザー](../resources/user.md)、[グループ](../resources/group.md)、[組織の連絡先](../resources/orgcontact.md)。</span><span class="sxs-lookup"><span data-stu-id="9d01f-105">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="9d01f-106">詳細は.、[変更の追跡](/graph/delta-query-overview)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9d01f-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d01f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9d01f-107">Permissions</span></span>

<span data-ttu-id="9d01f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d01f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d01f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d01f-110">Permission type</span></span>      | <span data-ttu-id="9d01f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d01f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d01f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d01f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d01f-113">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d01f-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="9d01f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d01f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d01f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d01f-115">Not supported.</span></span>  |
|<span data-ttu-id="9d01f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d01f-116">Application</span></span> | <span data-ttu-id="9d01f-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d01f-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d01f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d01f-118">HTTP request</span></span>

<span data-ttu-id="9d01f-119">変更の追跡を開始するには、directoryObjects リソースにデルタ関数を含む要求を行います。</span><span class="sxs-lookup"><span data-stu-id="9d01f-119">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="9d01f-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d01f-120">Query parameters</span></span>

<span data-ttu-id="9d01f-121">変更の追跡では、1回以上の**デルタ**関数呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="9d01f-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="9d01f-122">任意のクエリ パラメーター (`$deltatoken` と`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d01f-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="9d01f-123">Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。</span><span class="sxs-lookup"><span data-stu-id="9d01f-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="9d01f-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="9d01f-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="9d01f-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="9d01f-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d01f-126">Query parameter</span></span> | <span data-ttu-id="9d01f-127">種類</span><span class="sxs-lookup"><span data-stu-id="9d01f-127">Type</span></span> |<span data-ttu-id="9d01f-128">説明</span><span class="sxs-lookup"><span data-stu-id="9d01f-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9d01f-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="9d01f-129">$deltatoken</span></span> | <span data-ttu-id="9d01f-130">string</span><span class="sxs-lookup"><span data-stu-id="9d01f-130">string</span></span> | <span data-ttu-id="9d01f-p105">同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="9d01f-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="9d01f-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="9d01f-133">$skiptoken</span></span> | <span data-ttu-id="9d01f-134">string</span><span class="sxs-lookup"><span data-stu-id="9d01f-134">string</span></span> | <span data-ttu-id="9d01f-135">前の**デルタ**関数の `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。</span><span class="sxs-lookup"><span data-stu-id="9d01f-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="9d01f-136">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d01f-136">OData query parameters</span></span>

<span data-ttu-id="9d01f-137">このメソッドは、応答をカスタマイズするためのオプショナルの OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="9d01f-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="9d01f-138">特別な`isOf`演算子`$filter`と共にを使用して、directoryobject から派生した型のサブセットをフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-138">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="9d01f-139">を使用して複数の式`or`を組み合わせることができます。これにより、1つのデルタクエリで複数の種類を追跡できます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-139">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="9d01f-140">詳細については、 [3 番目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d01f-140">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d01f-141">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d01f-141">Request headers</span></span>

| <span data-ttu-id="9d01f-142">名前</span><span class="sxs-lookup"><span data-stu-id="9d01f-142">Name</span></span>       | <span data-ttu-id="9d01f-143">説明</span><span class="sxs-lookup"><span data-stu-id="9d01f-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9d01f-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d01f-144">Authorization</span></span>  | <span data-ttu-id="9d01f-145">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="9d01f-145">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="9d01f-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d01f-146">Content-Type</span></span>  | <span data-ttu-id="9d01f-147">application/json</span><span class="sxs-lookup"><span data-stu-id="9d01f-147">application/json</span></span> |
| <span data-ttu-id="9d01f-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="9d01f-148">Prefer</span></span> | <span data-ttu-id="9d01f-149">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="9d01f-149">return=minimal</span></span> <br><br><span data-ttu-id="9d01f-150">このヘッダーを指定する要求を使用すると、`deltaLink` は、最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="9d01f-150">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="9d01f-151">省略可能です。</span><span class="sxs-lookup"><span data-stu-id="9d01f-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d01f-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d01f-152">Request body</span></span>

<span data-ttu-id="9d01f-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9d01f-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="9d01f-154">応答</span><span class="sxs-lookup"><span data-stu-id="9d01f-154">Response</span></span>

<span data-ttu-id="9d01f-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/directoryobject.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d01f-155">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="9d01f-156">応答には`nextLink` URLまたは`deltaLink` URLも含まれます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-156">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="9d01f-157">もし`nextLink` URL が返された場合:</span><span class="sxs-lookup"><span data-stu-id="9d01f-157">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="9d01f-158">セッションで取得するデータに追加ページがあることを示しています。</span><span class="sxs-lookup"><span data-stu-id="9d01f-158">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="9d01f-159">アプリケーションは`deltaLink` URL が応答に含まれるまで`nextLink` URLを使用して要求を続けます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-159">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="9d01f-160">応答には、最初のデルタクエリ要求と同じ一連のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d01f-160">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="9d01f-161">これにより、デルタサイクルを開始するときに、オブジェクトの現在の完全な状態をキャプチャできます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-161">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="9d01f-162">もし`deltaLink` URL が返された場合:</span><span class="sxs-lookup"><span data-stu-id="9d01f-162">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="9d01f-163">これは、返されるリソースの既存の状態に関するデータがこれ以上ないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9d01f-163">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="9d01f-164">`deltaLink` URL を、次回のラウンドでリソースへの変更について学ぶために保存して使ってください。</span><span class="sxs-lookup"><span data-stu-id="9d01f-164">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="9d01f-165">`Prefer:return=minimal` ヘッダーを指定して、`deltaLink`発行後に変更されたプロパティのみをレスポンス値に含めるように選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-165">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="9d01f-166">デフォルト：初期デルタリクエストと同じプロパティを返します</span><span class="sxs-lookup"><span data-stu-id="9d01f-166">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="9d01f-167">デフォルトでは、`deltaLink`または`nextLink`を使用したリクエストは、最初のデルタクエリで選択されたものと同じプロパティを次のように返します:</span><span class="sxs-lookup"><span data-stu-id="9d01f-167">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="9d01f-168">プロパティを変更した場合は、応答には新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-168">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="9d01f-169">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-169">This includes properties being set to null value.</span></span>
- <span data-ttu-id="9d01f-170">プロパティが変更されていない場合は、古い値が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d01f-170">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="9d01f-171">プロパティが設定されたことがない場合は、応答にまったく含まれません。</span><span class="sxs-lookup"><span data-stu-id="9d01f-171">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="9d01f-172">**注意:** この動作では、応答を見ても、プロパティが変化しているかどうかを判断することはできません。</span><span class="sxs-lookup"><span data-stu-id="9d01f-172">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="9d01f-173">また、デルタ応答は、すべてのプロパティ値を含むため、サイズが大きくなる傾向があります。</span><span class="sxs-lookup"><span data-stu-id="9d01f-173">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="9d01f-174">代替案：変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="9d01f-174">Alternative: return only the changed properties</span></span>

<span data-ttu-id="9d01f-175">オプションのリクエストヘッダを追加すると、- `prefer:return=minimal` - 次のようになります:</span><span class="sxs-lookup"><span data-stu-id="9d01f-175">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="9d01f-176">プロパティを変更した場合は、応答には新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-176">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="9d01f-177">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-177">This includes properties being set to null value.</span></span>
- <span data-ttu-id="9d01f-178">プロパティが変更されていない場合、そのプロパティは応答にまったく含まれません。</span><span class="sxs-lookup"><span data-stu-id="9d01f-178">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="9d01f-179">(既定の動作と異なる)</span><span class="sxs-lookup"><span data-stu-id="9d01f-179">(Different from the default behavior.)</span></span>

> <span data-ttu-id="9d01f-180">**注意:** ヘッダーは、デルタサイクルのどの時点でも `deltaLink`要求に追加できます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-180">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="9d01f-181">ヘッダーは応答に含まれる一連のプロパティにのみ影響し、デルタクエリの実行方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="9d01f-181">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="9d01f-182">例</span><span class="sxs-lookup"><span data-stu-id="9d01f-182">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="9d01f-183">要求 1</span><span class="sxs-lookup"><span data-stu-id="9d01f-183">Request 1</span></span>

<span data-ttu-id="9d01f-184">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d01f-184">The following is an example of the request.</span></span> <span data-ttu-id="9d01f-185">`$select`パラメータがないため、デフォルトのプロパティセットが追跡されて返されます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-185">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9d01f-186">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9d01f-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directory_object_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9d01f-187">C#</span><span class="sxs-lookup"><span data-stu-id="9d01f-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directory-object-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d01f-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d01f-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directory-object-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d01f-189">目的-C</span><span class="sxs-lookup"><span data-stu-id="9d01f-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directory-object-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="9d01f-190">応答 1</span><span class="sxs-lookup"><span data-stu-id="9d01f-190">Response 1</span></span>

<span data-ttu-id="9d01f-191">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9d01f-191">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="9d01f-192">フィルター `isOf`は使用されていないので、directoryobject から派生したすべての型が返されます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-192">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="9d01f-193">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="9d01f-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9d01f-194">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-194">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",      
      "jobTitle": "string"
    }
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="9d01f-195">要求 2</span><span class="sxs-lookup"><span data-stu-id="9d01f-195">Request 2</span></span>

<span data-ttu-id="9d01f-196">次の例は、代替の最小応答動作の使用法を示しています。</span><span class="sxs-lookup"><span data-stu-id="9d01f-196">The next example shows the use of the alternative minimal response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9d01f-197">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9d01f-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9d01f-198">C#</span><span class="sxs-lookup"><span data-stu-id="9d01f-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d01f-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d01f-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d01f-200">目的-C</span><span class="sxs-lookup"><span data-stu-id="9d01f-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="9d01f-201">応答 2</span><span class="sxs-lookup"><span data-stu-id="9d01f-201">Response 2</span></span>

<span data-ttu-id="9d01f-202">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9d01f-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="9d01f-203">メモ実際に変更されたプロパティのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="9d01f-203">Note only the properties that have actually changed are returned.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    }
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="9d01f-204">要求 3</span><span class="sxs-lookup"><span data-stu-id="9d01f-204">Request 3</span></span>

<span data-ttu-id="9d01f-205">次の例では、 `isOf`演算子を使用して、ユーザーエンティティとグループエンティティのみを除外する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="9d01f-205">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9d01f-206">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9d01f-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9d01f-207">C#</span><span class="sxs-lookup"><span data-stu-id="9d01f-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d01f-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d01f-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d01f-209">目的-C</span><span class="sxs-lookup"><span data-stu-id="9d01f-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="9d01f-210">応答 3</span><span class="sxs-lookup"><span data-stu-id="9d01f-210">Response 3</span></span>

<span data-ttu-id="9d01f-211">以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9d01f-211">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="9d01f-212">ユーザーオブジェクトとグループオブジェクトのみが返されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="9d01f-212">Note that only user and group objects are returned:</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    }
  ]
}
```

- <span data-ttu-id="9d01f-213">[デルタクエリを使用してMicrosoft Graphデータの変更を追跡します](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="9d01f-213">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="9d01f-214">[ユーザーの増分変更を取得します](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="9d01f-214">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
