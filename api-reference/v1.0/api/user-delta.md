---
title: 'user: delta'
description: Get を新しく作成するには、更新、または全体のユーザーのコレクションのすべての読み取りを実行することがなくユーザーを削除します。 詳細については変更の履歴を参照してください。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6464e8ad975a5fc996c671df5a01df2988dbf79d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945616"
---
# <a name="user-delta"></a><span data-ttu-id="6f3be-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="6f3be-104">user: delta</span></span>

<span data-ttu-id="6f3be-105">Get を新しく作成するには、更新、または全体のユーザーのコレクションのすべての読み取りを実行することがなくユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="6f3be-106">詳細については、[変更履歴の記録](/graph/delta-query-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f3be-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f3be-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6f3be-107">Permissions</span></span>

<span data-ttu-id="6f3be-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f3be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6f3be-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f3be-110">Permission type</span></span>      | <span data-ttu-id="6f3be-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f3be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f3be-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f3be-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6f3be-113">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f3be-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f3be-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f3be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f3be-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f3be-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="6f3be-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f3be-116">Application</span></span> | <span data-ttu-id="6f3be-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f3be-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f3be-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f3be-118">HTTP request</span></span>

<span data-ttu-id="6f3be-119">変更の追跡を開始するには、ユーザー リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="6f3be-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6f3be-120">Query parameters</span></span>

<span data-ttu-id="6f3be-121">ユーザーの変更の追跡と、一連の 1 つまたは複数の**delta**関数の呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="6f3be-122">任意のクエリ パラメーターを使用する場合 (以外の`$deltatoken`と`$skiptoken`)、**デルタ**の初期要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f3be-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="6f3be-123">Microsoft Graph が自動的に任意指定のパラメーターをエンコードのトークンの部分に、`nextLink`または`deltaLink`の応答で提供される URL です。</span><span class="sxs-lookup"><span data-stu-id="6f3be-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="6f3be-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="6f3be-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="6f3be-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="6f3be-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6f3be-126">Query parameter</span></span>      | <span data-ttu-id="6f3be-127">種類</span><span class="sxs-lookup"><span data-stu-id="6f3be-127">Type</span></span>   |<span data-ttu-id="6f3be-128">説明</span><span class="sxs-lookup"><span data-stu-id="6f3be-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6f3be-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="6f3be-129">$deltatoken</span></span> | <span data-ttu-id="6f3be-130">文字列</span><span class="sxs-lookup"><span data-stu-id="6f3be-130">string</span></span> | <span data-ttu-id="6f3be-p105">同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="6f3be-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="6f3be-133">$skiptoken</span></span> | <span data-ttu-id="6f3be-134">文字列</span><span class="sxs-lookup"><span data-stu-id="6f3be-134">string</span></span> | <span data-ttu-id="6f3be-135">前の**デルタ**関数の `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="6f3be-136">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6f3be-136">OData query parameters</span></span>

<span data-ttu-id="6f3be-137">このメソッドは、応答をカスタマイズするためのオプションの OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="6f3be-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="6f3be-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="6f3be-140">サポートが制限されて`$filter`。</span><span class="sxs-lookup"><span data-stu-id="6f3be-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="6f3be-141">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="6f3be-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="6f3be-142">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-142">You can filter multiple objects.</span></span> <span data-ttu-id="6f3be-143">たとえば、`https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。</span><span class="sxs-lookup"><span data-stu-id="6f3be-143">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="6f3be-144">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="6f3be-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f3be-145">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f3be-145">Request headers</span></span>
| <span data-ttu-id="6f3be-146">名前</span><span class="sxs-lookup"><span data-stu-id="6f3be-146">Name</span></span>       | <span data-ttu-id="6f3be-147">説明</span><span class="sxs-lookup"><span data-stu-id="6f3be-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f3be-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f3be-148">Authorization</span></span>  | <span data-ttu-id="6f3be-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="6f3be-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="6f3be-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f3be-150">Content-Type</span></span>  | <span data-ttu-id="6f3be-151">application/json</span><span class="sxs-lookup"><span data-stu-id="6f3be-151">application/json</span></span> |
| <span data-ttu-id="6f3be-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="6f3be-152">Prefer</span></span> | <span data-ttu-id="6f3be-153">返す最小 =</span><span class="sxs-lookup"><span data-stu-id="6f3be-153">return=minimal</span></span> <br><br><span data-ttu-id="6f3be-154">このヘッダーを指定する要求を使用すると、`deltaLink`最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="6f3be-155">省略可能。</span><span class="sxs-lookup"><span data-stu-id="6f3be-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f3be-156">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f3be-156">Request body</span></span>
<span data-ttu-id="6f3be-157">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6f3be-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="6f3be-158">応答</span><span class="sxs-lookup"><span data-stu-id="6f3be-158">Response</span></span>

<span data-ttu-id="6f3be-159">かどうかは成功すると、このメソッドを返します`200 OK`応答の本体で応答コードと[ユーザー](../resources/user.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6f3be-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="6f3be-160">応答にも含まれています、`nextLink`の URL、または`deltaLink`URL です。</span><span class="sxs-lookup"><span data-stu-id="6f3be-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="6f3be-161">場合、`nextLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="6f3be-162">これは、他のページのセッションで取得するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="6f3be-163">アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f3be-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="6f3be-164">応答には、同じ一連最初のデルタ ・ クエリ要求のようにプロパティにはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f3be-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="6f3be-165">これにより、デルタ ・ サイクルを開始するときに、オブジェクトのすべての現在の状態をキャプチャすることができます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="6f3be-166">場合、`deltaLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="6f3be-167">これは、返されるリソースの既存の状態に関するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="6f3be-168">保存し、使用して、`deltaLink`について学習するための URL は次のラウンドでリソースを変更します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="6f3be-169">指定の選択肢がある場合、`Prefer:return=minimal`時間以降に変更されたプロパティのみの応答の値に追加する、ヘッダー、`deltaLink`が発行されました。</span><span class="sxs-lookup"><span data-stu-id="6f3be-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="6f3be-170">既定値: は、最初のデルタ ・ リクエストと同じプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="6f3be-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="6f3be-171">既定では、要求を使用して、`deltaLink`または`nextLink`次のように最初のデルタ ・ クエリで選択したのと同じプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="6f3be-172">プロパティが変更された場合は、応答に新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="6f3be-173">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="6f3be-174">プロパティが変更されていない場合は、応答に古い値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="6f3be-175">プロパティの場合は、含まれませんの応答ですべての前に設定されています。</span><span class="sxs-lookup"><span data-stu-id="6f3be-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="6f3be-176">**注:** この現象に関して、応答を見ることはできませんプロパティを変更するかどうかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="6f3be-177">また、デルタの反応をする大規模なすべてのプロパティ値が含まれているため、次の[2 番目の例](#request-2)に示すように傾向があります。</span><span class="sxs-lookup"><span data-stu-id="6f3be-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="6f3be-178">: 別の方法が変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="6f3be-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="6f3be-179">オプションの要求ヘッダーでは - を追加する`prefer:return=minimal`の次の動作の結果します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="6f3be-180">プロパティが変更された場合は、応答に新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="6f3be-181">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="6f3be-182">プロパティが変更されていない場合は、プロパティが含まれていない応答ですべての。</span><span class="sxs-lookup"><span data-stu-id="6f3be-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="6f3be-183">(既定の動作と異なります)</span><span class="sxs-lookup"><span data-stu-id="6f3be-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="6f3be-184">**注:** ヘッダーを追加することができます、`deltaLink`デルタ ・ サイクルの時間内の任意の時点で要求します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="6f3be-185">ヘッダーの応答に含まれるプロパティのセットにのみ影響し、デルタ ・ クエリを実行する方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="6f3be-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="6f3be-186">次の[3 番目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f3be-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="6f3be-187">例</span><span class="sxs-lookup"><span data-stu-id="6f3be-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="6f3be-188">要求 1</span><span class="sxs-lookup"><span data-stu-id="6f3be-188">Request 1</span></span>

<span data-ttu-id="6f3be-189">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-189">The following is an example of the request.</span></span> <span data-ttu-id="6f3be-190">ありません`$select`パラメーター、プロパティの既定のセットが追跡され、返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="6f3be-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="6f3be-191">応答 1</span><span class="sxs-lookup"><span data-stu-id="6f3be-191">Response 1</span></span>

<span data-ttu-id="6f3be-192">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="6f3be-p119">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6f3be-p119">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

#### <a name="request-2"></a><span data-ttu-id="6f3be-195">要求 2</span><span class="sxs-lookup"><span data-stu-id="6f3be-195">Request 2</span></span>

<span data-ttu-id="6f3be-196">次の使用例は、変更の追跡、応答の既定の動作で 3 つのプロパティを選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="6f3be-196">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="6f3be-197">応答 2</span><span class="sxs-lookup"><span data-stu-id="6f3be-197">Response 2</span></span>

<span data-ttu-id="6f3be-198">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="6f3be-199">応答ですべての 3 つのプロパティが含まれますし、以降に変更されているどれが不明、`deltaLink`を取得しました。</span><span class="sxs-lookup"><span data-stu-id="6f3be-199">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="6f3be-200">要求 3</span><span class="sxs-lookup"><span data-stu-id="6f3be-200">Request 3</span></span>

<span data-ttu-id="6f3be-201">次の使用例は、3 つのプロパティの変更履歴の記録を最小限に抑える別の応答の動作を選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="6f3be-201">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="6f3be-202">応答 3</span><span class="sxs-lookup"><span data-stu-id="6f3be-202">Response 3</span></span>

<span data-ttu-id="6f3be-203">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-203">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="6f3be-204">なお、`mobilePhone`プロパティが含まれていないことを意味するは、前回のデルタ ・ クエリは変更されていません。`displayName`と`jobTitle`は、値が変更されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-204">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- <span data-ttu-id="6f3be-205">[グラフ データの変更を追跡するためにデルタのクエリを使用します](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="6f3be-205">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="6f3be-206">[ユーザーの増分の変更を取得](/graph/delta-query-users)します。</span><span class="sxs-lookup"><span data-stu-id="6f3be-206">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
