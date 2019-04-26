---
title: 'user: delta'
description: ユーザーコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたユーザーを取得します。 詳細については、「変更履歴」を参照してください。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4f6f14c35dac4ce9601911bcf5460053a860dac1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334948"
---
# <a name="user-delta"></a><span data-ttu-id="49dc6-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="49dc6-104">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49dc6-105">ユーザーコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="49dc6-106">詳細については、「[変更履歴](/graph/delta-query-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49dc6-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="49dc6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="49dc6-107">Permissions</span></span>

<span data-ttu-id="49dc6-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49dc6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="49dc6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49dc6-110">Permission type</span></span>      | <span data-ttu-id="49dc6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="49dc6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49dc6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49dc6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49dc6-113">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49dc6-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49dc6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49dc6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49dc6-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49dc6-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="49dc6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49dc6-116">Application</span></span> | <span data-ttu-id="49dc6-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49dc6-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49dc6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49dc6-118">HTTP request</span></span>

<span data-ttu-id="49dc6-119">変更の追跡を開始するには、ユーザー リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="49dc6-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="49dc6-120">Query parameters</span></span>

<span data-ttu-id="49dc6-121">ユーザーの変更を追跡するには、1つまたは複数の**デルタ**関数呼び出しのラウンドが発生します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="49dc6-122">クエリパラメーター ( `$deltatoken`および`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="49dc6-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="49dc6-123">Microsoft Graph は、指定されたパラメーターを、 `nextLink`応答で指定`deltaLink`されたまたは URL のトークン部分に自動的にエンコードします。</span><span class="sxs-lookup"><span data-stu-id="49dc6-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="49dc6-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="49dc6-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="49dc6-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="49dc6-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="49dc6-126">Query parameter</span></span>      | <span data-ttu-id="49dc6-127">種類</span><span class="sxs-lookup"><span data-stu-id="49dc6-127">Type</span></span>   |<span data-ttu-id="49dc6-128">説明</span><span class="sxs-lookup"><span data-stu-id="49dc6-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="49dc6-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="49dc6-129">$deltatoken</span></span> | <span data-ttu-id="49dc6-130">string</span><span class="sxs-lookup"><span data-stu-id="49dc6-130">string</span></span> | <span data-ttu-id="49dc6-p105">同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="49dc6-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="49dc6-133">$skiptoken</span></span> | <span data-ttu-id="49dc6-134">string</span><span class="sxs-lookup"><span data-stu-id="49dc6-134">string</span></span> | <span data-ttu-id="49dc6-135">前の**デルタ**関数の `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="49dc6-136">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="49dc6-136">OData query parameters</span></span>

<span data-ttu-id="49dc6-137">このメソッドは、応答をカスタマイズするためのオプションの OData クエリパラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="49dc6-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="49dc6-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="49dc6-140">次のサポートに`$filter`制限があります。</span><span class="sxs-lookup"><span data-stu-id="49dc6-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="49dc6-141">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="49dc6-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="49dc6-142">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-142">You can filter multiple objects.</span></span> <span data-ttu-id="49dc6-143">たとえば、`https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。</span><span class="sxs-lookup"><span data-stu-id="49dc6-143">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="49dc6-144">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="49dc6-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49dc6-145">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49dc6-145">Request headers</span></span>
| <span data-ttu-id="49dc6-146">名前</span><span class="sxs-lookup"><span data-stu-id="49dc6-146">Name</span></span>       | <span data-ttu-id="49dc6-147">説明</span><span class="sxs-lookup"><span data-stu-id="49dc6-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49dc6-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="49dc6-148">Authorization</span></span>  | <span data-ttu-id="49dc6-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="49dc6-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="49dc6-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49dc6-150">Content-Type</span></span>  | <span data-ttu-id="49dc6-151">application/json</span><span class="sxs-lookup"><span data-stu-id="49dc6-151">application/json</span></span> |
| <span data-ttu-id="49dc6-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="49dc6-152">Prefer</span></span> | <span data-ttu-id="49dc6-153">戻り値 = 最小</span><span class="sxs-lookup"><span data-stu-id="49dc6-153">return=minimal</span></span> <br><br><span data-ttu-id="49dc6-154">を`deltaLink`使用する要求でこのヘッダーを指定すると、最後のラウンド以降に変更されたオブジェクトプロパティのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="49dc6-155">省略可能。</span><span class="sxs-lookup"><span data-stu-id="49dc6-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49dc6-156">要求本文</span><span class="sxs-lookup"><span data-stu-id="49dc6-156">Request body</span></span>
<span data-ttu-id="49dc6-157">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="49dc6-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="49dc6-158">応答</span><span class="sxs-lookup"><span data-stu-id="49dc6-158">Response</span></span>

<span data-ttu-id="49dc6-159">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/user.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="49dc6-160">応答には、 `nextLink` url または`deltaLink` url も含まれます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="49dc6-161">URL が`nextLink`返される場合は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="49dc6-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="49dc6-162">これは、セッションで取得するデータのページが他にもあることを示しています。</span><span class="sxs-lookup"><span data-stu-id="49dc6-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="49dc6-163">アプリケーションは、応答に`nextLink` `deltaLink` url が含まれるまで、url を使用して要求を引き続き行います。</span><span class="sxs-lookup"><span data-stu-id="49dc6-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="49dc6-164">応答には、初期デルタクエリ要求と同じプロパティセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="49dc6-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="49dc6-165">これにより、デルタサイクルを開始するときに、オブジェクトの現在の完全な状態を取得できます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="49dc6-166">URL が`deltaLink`返される場合は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="49dc6-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="49dc6-167">これは、返されるリソースの既存の状態に関するデータがないことを示します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="49dc6-168">`deltaLink` URL を保存して使用し、次のラウンドでのリソースの変更について学習します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="49dc6-169">`Prefer:return=minimal`ヘッダーを指定することもできます。これは、が発行`deltaLink`されてから変更されたプロパティのみを応答値に含めることを選択することです。</span><span class="sxs-lookup"><span data-stu-id="49dc6-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="49dc6-170">Default: 初期デルタ要求と同じプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="49dc6-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="49dc6-171">既定では、次の`deltaLink`方法`nextLink`で、を使用して、または初期デルタクエリで選択されたものと同じプロパティを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="49dc6-172">プロパティが変更されている場合、新しい値は応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="49dc6-173">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="49dc6-174">プロパティが変更されていない場合は、古い値が応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="49dc6-175">プロパティが設定されていない場合は、応答には含まれません。</span><span class="sxs-lookup"><span data-stu-id="49dc6-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="49dc6-176">**注:** この動作では、応答を見ることで、プロパティが変更されているかどうかを判断することはできません。</span><span class="sxs-lookup"><span data-stu-id="49dc6-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="49dc6-177">また、次の[2 番目の例](#request-2)に示すように、デルタ応答は、すべてのプロパティ値を含むため、サイズが大きくなる傾向があります。</span><span class="sxs-lookup"><span data-stu-id="49dc6-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="49dc6-178">代替方法: 変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="49dc6-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="49dc6-179">オプションの要求ヘッダーを追加`prefer:return=minimal`する--次のような動作になります。</span><span class="sxs-lookup"><span data-stu-id="49dc6-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="49dc6-180">プロパティが変更されている場合、新しい値は応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="49dc6-181">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="49dc6-182">プロパティが変更されていない場合、プロパティは応答には含まれません。</span><span class="sxs-lookup"><span data-stu-id="49dc6-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="49dc6-183">(既定の動作とは異なります)。</span><span class="sxs-lookup"><span data-stu-id="49dc6-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="49dc6-184">**注:** このヘッダーは、デルタサイクルの`deltaLink`任意の時点で要求に追加できます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="49dc6-185">ヘッダーは、応答に含まれているプロパティのセットにのみ影響し、デルタクエリの実行方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="49dc6-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="49dc6-186">次の[3 つ目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49dc6-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="49dc6-187">例</span><span class="sxs-lookup"><span data-stu-id="49dc6-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="49dc6-188">要求 1</span><span class="sxs-lookup"><span data-stu-id="49dc6-188">Request 1</span></span>

<span data-ttu-id="49dc6-189">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-189">The following is an example of the request.</span></span> <span data-ttu-id="49dc6-190">パラメーターがない`$select`ので、プロパティの既定のセットが追跡されて返されます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="49dc6-191">応答 1</span><span class="sxs-lookup"><span data-stu-id="49dc6-191">Response 1</span></span>

<span data-ttu-id="49dc6-192">次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="49dc6-193">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="49dc6-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49dc6-194">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="49dc6-194">All the properties will be returned from an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="49dc6-195">要求 2</span><span class="sxs-lookup"><span data-stu-id="49dc6-195">Request 2</span></span>

<span data-ttu-id="49dc6-196">次の例は、既定の応答動作を使用して、変更追跡の3つのプロパティを選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="49dc6-196">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="49dc6-197">応答 2</span><span class="sxs-lookup"><span data-stu-id="49dc6-197">Response 2</span></span>

<span data-ttu-id="49dc6-198">次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="49dc6-199">3つすべてのプロパティは応答に含まれていますが、 `deltaLink`取得した後に変更されたプロパティが不明であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="49dc6-199">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="49dc6-200">要求 3</span><span class="sxs-lookup"><span data-stu-id="49dc6-200">Request 3</span></span>

<span data-ttu-id="49dc6-201">次の例は、変更追跡の3つのプロパティを選択する最初の要求を示しています。これには、次のような最低限の応答動作があります。</span><span class="sxs-lookup"><span data-stu-id="49dc6-201">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="49dc6-202">応答 3</span><span class="sxs-lookup"><span data-stu-id="49dc6-202">Response 3</span></span>

<span data-ttu-id="49dc6-203">次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-203">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="49dc6-204">プロパティは含ま`mobilePhone`れていません。つまり、最後のデルタクエリ以降変更されていないことに注意してください。`displayName`と`jobTitle`は、その値が変更されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-204">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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

- <span data-ttu-id="49dc6-205">[デルタクエリを使用して、Microsoft Graph データの変更を追跡](/graph/delta-query-overview)します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-205">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="49dc6-206">[ユーザーに対する増分の変更を取得](/graph/delta-query-users)します。</span><span class="sxs-lookup"><span data-stu-id="49dc6-206">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
