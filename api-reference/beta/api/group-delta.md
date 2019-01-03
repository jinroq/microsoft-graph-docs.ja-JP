---
title: 'group: delta'
description: Get を新しく作成するには、更新、またはグループ メンバーシップの変更を含むグループ全体のコレクションのすべての読み取りを実行しなくても、グループを削除します。 詳細については、デルタのクエリを使用するを参照してください。
ms.openlocfilehash: 562321ddff9e5c9d2840c1c1178aa8e4f2fd4114
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072769"
---
# <a name="group-delta"></a><span data-ttu-id="dd9c3-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="dd9c3-104">group: delta</span></span>

> <span data-ttu-id="dd9c3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd9c3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd9c3-107">Get を新しく作成するには、更新、またはグループ メンバーシップの変更を含むグループ全体のコレクションのすべての読み取りを実行しなくても、グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-107">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="dd9c3-108">詳細については、[デルタのクエリを使用する](/graph/delta-query-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd9c3-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dd9c3-109">Permissions</span></span>

<span data-ttu-id="dd9c3-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd9c3-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dd9c3-112">Permission type</span></span>      | <span data-ttu-id="dd9c3-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dd9c3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd9c3-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dd9c3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dd9c3-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd9c3-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dd9c3-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dd9c3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd9c3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-117">Not supported.</span></span>    |
|<span data-ttu-id="dd9c3-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dd9c3-118">Application</span></span> | <span data-ttu-id="dd9c3-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd9c3-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd9c3-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dd9c3-120">HTTP request</span></span>

<span data-ttu-id="dd9c3-121">変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-121">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="dd9c3-122">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dd9c3-122">Query parameters</span></span>

<span data-ttu-id="dd9c3-p105">グループで変更の追跡を実行するときには、1 つまたは複数の **delta** 関数の呼び出しが必要になります。クエリ パラメーター (`$deltatoken` および `$skiptoken` 以外) を使用する場合は、そのパラメーターを最初の **delta** 要求に指定する必要があります。指定されたパラメーターは、Microsoft Graph を使って自動的にエンコードされ、応答の `nextLink` または `deltaLink` URL のトークン部分として指定されます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-p105">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="dd9c3-126">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="dd9c3-127">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="dd9c3-128">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dd9c3-128">Query parameter</span></span> | <span data-ttu-id="dd9c3-129">種類</span><span class="sxs-lookup"><span data-stu-id="dd9c3-129">Type</span></span>  |<span data-ttu-id="dd9c3-130">説明</span><span class="sxs-lookup"><span data-stu-id="dd9c3-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd9c3-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="dd9c3-131">$deltatoken</span></span> | <span data-ttu-id="dd9c3-132">文字列</span><span class="sxs-lookup"><span data-stu-id="dd9c3-132">string</span></span> | <span data-ttu-id="dd9c3-p106">同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="dd9c3-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="dd9c3-135">$skiptoken</span></span> | <span data-ttu-id="dd9c3-136">文字列</span><span class="sxs-lookup"><span data-stu-id="dd9c3-136">string</span></span> | <span data-ttu-id="dd9c3-137">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="dd9c3-138">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dd9c3-138">OData query parameters</span></span>

<span data-ttu-id="dd9c3-139">このメソッドは、応答をカスタマイズするためのオプションの OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-139">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="dd9c3-p107">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="dd9c3-142">使用することができます`$expand=members`のメンバーシップの変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-142">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="dd9c3-143">サポートが制限されて`$filter`。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-143">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="dd9c3-144">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-144">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="dd9c3-145">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-145">You can filter multiple objects.</span></span> <span data-ttu-id="dd9c3-146">たとえば、`https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-146">For example, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="dd9c3-147">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-147">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd9c3-148">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd9c3-148">Request headers</span></span>

| <span data-ttu-id="dd9c3-149">名前</span><span class="sxs-lookup"><span data-stu-id="dd9c3-149">Name</span></span>       | <span data-ttu-id="dd9c3-150">説明</span><span class="sxs-lookup"><span data-stu-id="dd9c3-150">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd9c3-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd9c3-151">Authorization</span></span>  | <span data-ttu-id="dd9c3-152">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="dd9c3-152">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="dd9c3-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd9c3-153">Content-Type</span></span>  | <span data-ttu-id="dd9c3-154">application/json</span><span class="sxs-lookup"><span data-stu-id="dd9c3-154">application/json</span></span> |
| <span data-ttu-id="dd9c3-155">Prefer</span><span class="sxs-lookup"><span data-stu-id="dd9c3-155">Prefer</span></span> | <span data-ttu-id="dd9c3-156">返す最小 =</span><span class="sxs-lookup"><span data-stu-id="dd9c3-156">return=minimal</span></span> <br><br><span data-ttu-id="dd9c3-157">このヘッダーを指定する要求を使用すると、`deltaLink`最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-157">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="dd9c3-158">省略可能。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-158">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd9c3-159">要求本文</span><span class="sxs-lookup"><span data-stu-id="dd9c3-159">Request body</span></span>

<span data-ttu-id="dd9c3-160">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-160">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="dd9c3-161">応答</span><span class="sxs-lookup"><span data-stu-id="dd9c3-161">Response</span></span>

<span data-ttu-id="dd9c3-162">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-162">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="dd9c3-163">応答には、次のいずれかの状態のトークンも含まれています、`nextLink`の URL、または`deltaLink`URL です。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-163">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="dd9c3-164">場合、`nextLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-164">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="dd9c3-165">これは、他のページのセッションで取得するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-165">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="dd9c3-166">アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-166">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="dd9c3-167">応答には、同じ一連最初のデルタ ・ クエリ要求のようにプロパティにはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-167">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="dd9c3-168">これにより、デルタ ・ サイクルを開始するときに、オブジェクトのすべての現在の状態をキャプチャすることができます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-168">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="dd9c3-169">場合、`deltaLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-169">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="dd9c3-170">これは、返されるリソースの既存の状態に関するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-170">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="dd9c3-171">保存し、使用して、`deltaLink`について学習するための URL は次のラウンドでリソースを変更します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-171">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="dd9c3-172">指定の選択肢がある場合、`Prefer:return=minimal`時間以降に変更されたプロパティのみの応答の値に追加する、ヘッダー、`deltaLink`が発行されました。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-172">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="dd9c3-173">既定値: は、最初のデルタ ・ リクエストと同じプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="dd9c3-173">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="dd9c3-174">既定では、要求を使用して、`deltaLink`または`nextLink`次のように最初のデルタ ・ クエリで選択したのと同じプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-174">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="dd9c3-175">プロパティが変更された場合は、応答に新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-175">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="dd9c3-176">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-176">This includes properties being set to null value.</span></span>
- <span data-ttu-id="dd9c3-177">プロパティが変更されていない場合は、応答に古い値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-177">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="dd9c3-178">プロパティの場合は、含まれませんの応答ですべての前に設定されています。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-178">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="dd9c3-179">**注:** この現象に関して、応答を見ることはできませんプロパティを変更するかどうかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-179">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="dd9c3-180">また、デルタの反応をする大規模なすべてのプロパティ値が含まれているため、次の[2 番目の例](#request-2)に示すように傾向があります。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-180">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="dd9c3-181">: 別の方法が変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="dd9c3-181">Alternative: return only the changed properties</span></span>

<span data-ttu-id="dd9c3-182">オプションの要求ヘッダーでは - を追加する`prefer:return=minimal`の次の動作の結果します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-182">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="dd9c3-183">プロパティが変更された場合は、応答に新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-183">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="dd9c3-184">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-184">This includes properties being set to null value.</span></span>
- <span data-ttu-id="dd9c3-185">プロパティが変更されていない場合は、プロパティが含まれていない応答ですべての。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-185">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="dd9c3-186">(既定の動作と異なります)</span><span class="sxs-lookup"><span data-stu-id="dd9c3-186">(Different from the default behavior.)</span></span>

> <span data-ttu-id="dd9c3-187">**注:** ヘッダーを追加することができます、`deltaLink`デルタ ・ サイクルの時間内の任意の時点で要求します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-187">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="dd9c3-188">ヘッダーの応答に含まれるプロパティのセットにのみ影響し、デルタ ・ クエリを実行する方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-188">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="dd9c3-189">次の[3 番目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-189">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="dd9c3-190">例</span><span class="sxs-lookup"><span data-stu-id="dd9c3-190">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="dd9c3-191">要求 1</span><span class="sxs-lookup"><span data-stu-id="dd9c3-191">Request 1</span></span>

<span data-ttu-id="dd9c3-192">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-192">The following is an example of the request.</span></span> <span data-ttu-id="dd9c3-193">ありません`$select`パラメーター、プロパティの既定のセットが追跡され、返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-193">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="dd9c3-194">応答 1</span><span class="sxs-lookup"><span data-stu-id="dd9c3-194">Response 1</span></span>

<span data-ttu-id="dd9c3-195">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-195">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="dd9c3-196">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-196">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dd9c3-197">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-197">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="dd9c3-198">グループ内のメンバー オブジェクトの id が含まれている*members@delta*プロパティが存在することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-198">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="dd9c3-199">要求 2</span><span class="sxs-lookup"><span data-stu-id="dd9c3-199">Request 2</span></span>

<span data-ttu-id="dd9c3-200">次の使用例は、変更の追跡、応答の既定の動作で 3 つのプロパティを選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-200">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="dd9c3-201">応答 2</span><span class="sxs-lookup"><span data-stu-id="dd9c3-201">Response 2</span></span>

<span data-ttu-id="dd9c3-202">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="dd9c3-203">応答ですべての 3 つのプロパティが含まれますし、以降に変更されているどれが不明、`deltaLink`を取得しました。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-203">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="dd9c3-204">要求 3</span><span class="sxs-lookup"><span data-stu-id="dd9c3-204">Request 3</span></span>

<span data-ttu-id="dd9c3-205">次の使用例は、3 つのプロパティの変更履歴の記録を最小限に抑える別の応答の動作を選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-205">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="dd9c3-206">応答 3</span><span class="sxs-lookup"><span data-stu-id="dd9c3-206">Response 3</span></span>

<span data-ttu-id="dd9c3-207">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-207">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="dd9c3-208">なお、`mailNickname`プロパティが含まれていないことを意味するは、前回のデルタ ・ クエリは変更されていません。`displayName`と`description`は、値が変更されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-208">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="dd9c3-209">関連項目</span><span class="sxs-lookup"><span data-stu-id="dd9c3-209">See also</span></span>

- <span data-ttu-id="dd9c3-210">[グラフ データの変更を追跡するためにデルタのクエリを使用します](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-210">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="dd9c3-211">[グループの増分の変更を取得](/graph/delta-query-groups)します。</span><span class="sxs-lookup"><span data-stu-id="dd9c3-211">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->