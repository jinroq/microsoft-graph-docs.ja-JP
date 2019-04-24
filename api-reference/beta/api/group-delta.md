---
title: 'group: delta'
description: グループメンバーシップの変更を含む、新しく作成、更新、または削除されたグループを取得します。グループコレクション全体の完全な読み取りを実行する必要はありません。 詳細については、「デルタクエリの使用」を参照してください。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: c894df643289d3f92ce20ebd36a53456999ab587
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502730"
---
# <a name="group-delta"></a><span data-ttu-id="f4b4f-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="f4b4f-104">group: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4b4f-105">グループメンバーシップの変更を含む、新しく作成、更新、または削除されたグループを取得します。グループコレクション全体の完全な読み取りを実行する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-105">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="f4b4f-106">詳細については、「[デルタクエリの使用](/graph/delta-query-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4b4f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4b4f-107">Permissions</span></span>

<span data-ttu-id="f4b4f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4b4f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4b4f-110">Permission type</span></span>      | <span data-ttu-id="f4b4f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4b4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4b4f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4b4f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f4b4f-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4b4f-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f4b4f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4b4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4b4f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-115">Not supported.</span></span>    |
|<span data-ttu-id="f4b4f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4b4f-116">Application</span></span> | <span data-ttu-id="f4b4f-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4b4f-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4b4f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4b4f-118">HTTP request</span></span>

<span data-ttu-id="f4b4f-119">変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-119">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="f4b4f-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4b4f-120">Query parameters</span></span>

<span data-ttu-id="f4b4f-p104">グループで変更の追跡を実行するときには、1 つまたは複数の **delta** 関数の呼び出しが必要になります。クエリ パラメーター (`$deltatoken` および `$skiptoken` 以外) を使用する場合は、そのパラメーターを最初の **delta** 要求に指定する必要があります。指定されたパラメーターは、Microsoft Graph を使って自動的にエンコードされ、応答の `nextLink` または `deltaLink` URL のトークン部分として指定されます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-p104">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="f4b4f-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="f4b4f-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="f4b4f-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4b4f-126">Query parameter</span></span> | <span data-ttu-id="f4b4f-127">型</span><span class="sxs-lookup"><span data-stu-id="f4b4f-127">Type</span></span>  |<span data-ttu-id="f4b4f-128">説明</span><span class="sxs-lookup"><span data-stu-id="f4b4f-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4b4f-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="f4b4f-129">$deltatoken</span></span> | <span data-ttu-id="f4b4f-130">string</span><span class="sxs-lookup"><span data-stu-id="f4b4f-130">string</span></span> | <span data-ttu-id="f4b4f-p105">同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="f4b4f-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f4b4f-133">$skiptoken</span></span> | <span data-ttu-id="f4b4f-134">string</span><span class="sxs-lookup"><span data-stu-id="f4b4f-134">string</span></span> | <span data-ttu-id="f4b4f-135">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="f4b4f-136">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4b4f-136">OData query parameters</span></span>

<span data-ttu-id="f4b4f-137">このメソッドは、応答をカスタマイズするためのオプションの OData クエリパラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-137">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="f4b4f-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="f4b4f-140">を使用`$expand=members`して、メンバーシップの変更を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-140">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="f4b4f-141">次のサポートに`$filter`制限があります。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-141">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="f4b4f-142">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-142">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="f4b4f-143">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-143">You can filter multiple objects.</span></span> <span data-ttu-id="f4b4f-144">たとえば、`https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-144">For example, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="f4b4f-145">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-145">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4b4f-146">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4b4f-146">Request headers</span></span>

| <span data-ttu-id="f4b4f-147">名前</span><span class="sxs-lookup"><span data-stu-id="f4b4f-147">Name</span></span>       | <span data-ttu-id="f4b4f-148">説明</span><span class="sxs-lookup"><span data-stu-id="f4b4f-148">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4b4f-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4b4f-149">Authorization</span></span>  | <span data-ttu-id="f4b4f-150">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="f4b4f-150">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="f4b4f-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4b4f-151">Content-Type</span></span>  | <span data-ttu-id="f4b4f-152">application/json</span><span class="sxs-lookup"><span data-stu-id="f4b4f-152">application/json</span></span> |
| <span data-ttu-id="f4b4f-153">Prefer</span><span class="sxs-lookup"><span data-stu-id="f4b4f-153">Prefer</span></span> | <span data-ttu-id="f4b4f-154">戻り値 = 最小</span><span class="sxs-lookup"><span data-stu-id="f4b4f-154">return=minimal</span></span> <br><br><span data-ttu-id="f4b4f-155">を`deltaLink`使用する要求でこのヘッダーを指定すると、最後のラウンド以降に変更されたオブジェクトプロパティのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-155">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="f4b4f-156">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-156">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4b4f-157">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4b4f-157">Request body</span></span>

<span data-ttu-id="f4b4f-158">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-158">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="f4b4f-159">応答</span><span class="sxs-lookup"><span data-stu-id="f4b4f-159">Response</span></span>

<span data-ttu-id="f4b4f-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-160">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="f4b4f-161">応答には、 `nextLink` url または`deltaLink` url のいずれかの状態トークンも含まれます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-161">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="f4b4f-162">URL が`nextLink`返される場合は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-162">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="f4b4f-163">これは、セッションで取得するデータのページが他にもあることを示しています。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-163">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="f4b4f-164">アプリケーションは、応答に`nextLink` `deltaLink` url が含まれるまで、url を使用して要求を引き続き行います。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-164">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="f4b4f-165">応答には、初期デルタクエリ要求と同じプロパティセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-165">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="f4b4f-166">これにより、デルタサイクルを開始するときに、オブジェクトの現在の完全な状態を取得できます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-166">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="f4b4f-167">URL が`deltaLink`返される場合は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-167">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="f4b4f-168">これは、返されるリソースの既存の状態に関するデータがないことを示します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-168">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="f4b4f-169">`deltaLink` URL を保存して使用し、次のラウンドでのリソースの変更について学習します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-169">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="f4b4f-170">`Prefer:return=minimal`ヘッダーを指定することもできます。これは、が発行`deltaLink`されてから変更されたプロパティのみを応答値に含めることを選択することです。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-170">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="f4b4f-171">Default: 初期デルタ要求と同じプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="f4b4f-171">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="f4b4f-172">既定では、次の`deltaLink`方法`nextLink`で、を使用して、または初期デルタクエリで選択されたものと同じプロパティを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-172">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="f4b4f-173">プロパティが変更されている場合、新しい値は応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-173">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="f4b4f-174">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-174">This includes properties being set to null value.</span></span>
- <span data-ttu-id="f4b4f-175">プロパティが変更されていない場合は、古い値が応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-175">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="f4b4f-176">プロパティが設定されていない場合は、応答には含まれません。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-176">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="f4b4f-177">**注:** この動作では、応答を見ることで、プロパティが変更されているかどうかを判断することはできません。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-177">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="f4b4f-178">また、次の[2 番目の例](#request-2)に示すように、デルタ応答は、すべてのプロパティ値を含むため、サイズが大きくなる傾向があります。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-178">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="f4b4f-179">代替方法: 変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="f4b4f-179">Alternative: return only the changed properties</span></span>

<span data-ttu-id="f4b4f-180">オプションの要求ヘッダーを追加`prefer:return=minimal`する--次のような動作になります。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-180">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="f4b4f-181">プロパティが変更されている場合、新しい値は応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-181">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="f4b4f-182">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-182">This includes properties being set to null value.</span></span>
- <span data-ttu-id="f4b4f-183">プロパティが変更されていない場合、プロパティは応答には含まれません。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-183">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="f4b4f-184">(既定の動作とは異なります)。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-184">(Different from the default behavior.)</span></span>

> <span data-ttu-id="f4b4f-185">**注:** このヘッダーは、デルタサイクルの`deltaLink`任意の時点で要求に追加できます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-185">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="f4b4f-186">ヘッダーは、応答に含まれているプロパティのセットにのみ影響し、デルタクエリの実行方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-186">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="f4b4f-187">次の[3 つ目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-187">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="f4b4f-188">例</span><span class="sxs-lookup"><span data-stu-id="f4b4f-188">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="f4b4f-189">要求 1</span><span class="sxs-lookup"><span data-stu-id="f4b4f-189">Request 1</span></span>

<span data-ttu-id="f4b4f-190">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-190">The following is an example of the request.</span></span> <span data-ttu-id="f4b4f-191">パラメーターがない`$select`ので、プロパティの既定のセットが追跡されて返されます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-191">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="f4b4f-192">応答 1</span><span class="sxs-lookup"><span data-stu-id="f4b4f-192">Response 1</span></span>

<span data-ttu-id="f4b4f-193">次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-193">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="f4b4f-194">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-194">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f4b4f-195">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-195">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="f4b4f-196">グループ内の member オブジェクトの id を含む*メンバー @ delta*プロパティが存在することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-196">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="f4b4f-197">要求 2</span><span class="sxs-lookup"><span data-stu-id="f4b4f-197">Request 2</span></span>

<span data-ttu-id="f4b4f-198">次の例は、既定の応答動作を使用して、変更追跡の3つのプロパティを選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-198">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="f4b4f-199">応答 2</span><span class="sxs-lookup"><span data-stu-id="f4b4f-199">Response 2</span></span>

<span data-ttu-id="f4b4f-200">次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="f4b4f-201">3つすべてのプロパティは応答に含まれていますが、 `deltaLink`取得した後に変更されたプロパティが不明であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-201">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="f4b4f-202">要求 3</span><span class="sxs-lookup"><span data-stu-id="f4b4f-202">Request 3</span></span>

<span data-ttu-id="f4b4f-203">次の例は、変更追跡の3つのプロパティを選択する最初の要求を示しています。これには、次のような最低限の応答動作があります。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-203">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="f4b4f-204">応答 3</span><span class="sxs-lookup"><span data-stu-id="f4b4f-204">Response 3</span></span>

<span data-ttu-id="f4b4f-205">次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-205">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="f4b4f-206">プロパティは含ま`mailNickname`れていません。つまり、最後のデルタクエリ以降変更されていないことに注意してください。`displayName`と`description`は、その値が変更されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-206">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="f4b4f-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4b4f-207">See also</span></span>

- <span data-ttu-id="f4b4f-208">[デルタクエリを使用して、Microsoft Graph データの変更を追跡](/graph/delta-query-overview)します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-208">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="f4b4f-209">[グループに対する増分の変更を取得](/graph/delta-query-groups)します。</span><span class="sxs-lookup"><span data-stu-id="f4b4f-209">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

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
    "Error: /api-reference/beta/api/group-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
