---
title: 'directoryObject: デルタ'
description: 'Get を新規作成、更新、または、次の種類のディレクトリ オブジェクトを削除: ユーザー、グループ、および 1 つのデルタのクエリで、組織の連絡先です。 詳細については変更の履歴を参照してください。'
ms.openlocfilehash: 98674a141c0567defb06da7b1ccd95a209aaa4f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068350"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="5961d-104">directoryObject: デルタ</span><span class="sxs-lookup"><span data-stu-id="5961d-104">directoryObject: delta</span></span>

> <span data-ttu-id="5961d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5961d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5961d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5961d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5961d-107">Get を新規作成、更新、または、次の種類のディレクトリ オブジェクトを削除:[ユーザー](../resources/user.md)、[グループ](../resources/group.md)および[組織の連絡先](../resources/orgcontact.md)を 1 つのデルタのクエリにします。</span><span class="sxs-lookup"><span data-stu-id="5961d-107">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="5961d-108">詳細については、[変更履歴の記録](/graph/delta-query-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5961d-108">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="5961d-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5961d-109">Permissions</span></span>

<span data-ttu-id="5961d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5961d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5961d-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5961d-112">Permission type</span></span>      | <span data-ttu-id="5961d-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5961d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5961d-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5961d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5961d-115">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5961d-115">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="5961d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5961d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5961d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5961d-117">Not supported.</span></span>  |
|<span data-ttu-id="5961d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5961d-118">Application</span></span> | <span data-ttu-id="5961d-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5961d-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5961d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5961d-120">HTTP request</span></span>

<span data-ttu-id="5961d-121">変更の追跡を開始するには、directoryObjects リソースでデルタ関数を含む要求を行います。</span><span class="sxs-lookup"><span data-stu-id="5961d-121">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="5961d-122">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5961d-122">Query parameters</span></span>

<span data-ttu-id="5961d-123">変更を追跡する一連の 1 つまたは複数の**delta**関数の呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="5961d-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="5961d-124">任意のクエリ パラメーターを使用する場合 (以外の`$deltatoken`と`$skiptoken`)、**デルタ**の初期要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5961d-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="5961d-125">Microsoft Graph が自動的に任意指定のパラメーターをエンコードのトークンの部分に、`nextLink`または`deltaLink`の応答で提供される URL です。</span><span class="sxs-lookup"><span data-stu-id="5961d-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="5961d-126">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="5961d-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="5961d-127">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="5961d-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="5961d-128">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5961d-128">Query parameter</span></span> | <span data-ttu-id="5961d-129">種類</span><span class="sxs-lookup"><span data-stu-id="5961d-129">Type</span></span> |<span data-ttu-id="5961d-130">説明</span><span class="sxs-lookup"><span data-stu-id="5961d-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5961d-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="5961d-131">$deltatoken</span></span> | <span data-ttu-id="5961d-132">文字列</span><span class="sxs-lookup"><span data-stu-id="5961d-132">string</span></span> | <span data-ttu-id="5961d-p106">同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="5961d-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="5961d-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="5961d-135">$skiptoken</span></span> | <span data-ttu-id="5961d-136">文字列</span><span class="sxs-lookup"><span data-stu-id="5961d-136">string</span></span> | <span data-ttu-id="5961d-137">前の**デルタ**関数の `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。</span><span class="sxs-lookup"><span data-stu-id="5961d-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="5961d-138">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5961d-138">OData query parameters</span></span>

<span data-ttu-id="5961d-139">このメソッドは、応答をカスタマイズするためのオプションの OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="5961d-139">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="5961d-140">使用することができます`$filter`、特殊な`isOf`directoryObject から派生した型のサブセットをフィルター処理する演算子です。</span><span class="sxs-lookup"><span data-stu-id="5961d-140">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="5961d-141">使用して複数の式を組み合わせることができます、 `or`、1 つのデルタ クエリを複数の種類を追跡できるようにします。</span><span class="sxs-lookup"><span data-stu-id="5961d-141">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="5961d-142">詳細については、 [3 番目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5961d-142">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5961d-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5961d-143">Request headers</span></span>

| <span data-ttu-id="5961d-144">名前</span><span class="sxs-lookup"><span data-stu-id="5961d-144">Name</span></span>       | <span data-ttu-id="5961d-145">説明</span><span class="sxs-lookup"><span data-stu-id="5961d-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5961d-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="5961d-146">Authorization</span></span>  | <span data-ttu-id="5961d-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="5961d-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="5961d-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5961d-148">Content-Type</span></span>  | <span data-ttu-id="5961d-149">application/json</span><span class="sxs-lookup"><span data-stu-id="5961d-149">application/json</span></span> |
| <span data-ttu-id="5961d-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="5961d-150">Prefer</span></span> | <span data-ttu-id="5961d-151">返す最小 =</span><span class="sxs-lookup"><span data-stu-id="5961d-151">return=minimal</span></span> <br><br><span data-ttu-id="5961d-152">このヘッダーを指定する要求を使用すると、`deltaLink`最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="5961d-152">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="5961d-153">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5961d-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5961d-154">要求本文</span><span class="sxs-lookup"><span data-stu-id="5961d-154">Request body</span></span>

<span data-ttu-id="5961d-155">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5961d-155">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="5961d-156">応答</span><span class="sxs-lookup"><span data-stu-id="5961d-156">Response</span></span>

<span data-ttu-id="5961d-157">かどうかは成功すると、このメソッドを返します`200 OK`応答の本体で応答コードと[ユーザー](../resources/directoryobject.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5961d-157">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="5961d-158">応答にも含まれています、`nextLink`の URL、または`deltaLink`URL です。</span><span class="sxs-lookup"><span data-stu-id="5961d-158">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="5961d-159">場合、`nextLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="5961d-159">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="5961d-160">これは、他のページのセッションで取得するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="5961d-160">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="5961d-161">アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="5961d-161">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="5961d-162">応答には、同じ一連最初のデルタ ・ クエリ要求のようにプロパティにはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5961d-162">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="5961d-163">これにより、デルタ ・ サイクルを開始するときに、オブジェクトのすべての現在の状態をキャプチャすることができます。</span><span class="sxs-lookup"><span data-stu-id="5961d-163">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="5961d-164">場合、`deltaLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="5961d-164">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="5961d-165">これは、返されるリソースの既存の状態に関するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="5961d-165">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="5961d-166">保存し、使用して、`deltaLink`について学習するための URL は次のラウンドでリソースを変更します。</span><span class="sxs-lookup"><span data-stu-id="5961d-166">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="5961d-167">指定の選択肢がある場合、`Prefer:return=minimal`時間以降に変更されたプロパティのみの応答の値に追加する、ヘッダー、`deltaLink`が発行されました。</span><span class="sxs-lookup"><span data-stu-id="5961d-167">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="5961d-168">既定値: は、最初のデルタ ・ リクエストと同じプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="5961d-168">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="5961d-169">既定では、要求を使用して、`deltaLink`または`nextLink`次のように最初のデルタ ・ クエリで選択したのと同じプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="5961d-169">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="5961d-170">プロパティが変更された場合は、応答に新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5961d-170">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="5961d-171">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5961d-171">This includes properties being set to null value.</span></span>
- <span data-ttu-id="5961d-172">プロパティが変更されていない場合は、応答に古い値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5961d-172">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="5961d-173">プロパティの場合は、含まれませんの応答ですべての前に設定されています。</span><span class="sxs-lookup"><span data-stu-id="5961d-173">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="5961d-174">**注:** この現象に関して、応答を見ることはできませんプロパティを変更するかどうかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="5961d-174">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="5961d-175">また、デルタの応答をすべてのプロパティ値が含まれているために大きくなる傾向があります。</span><span class="sxs-lookup"><span data-stu-id="5961d-175">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="5961d-176">: 別の方法が変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="5961d-176">Alternative: return only the changed properties</span></span>

<span data-ttu-id="5961d-177">オプションの要求ヘッダーでは - を追加する`prefer:return=minimal`の次の動作の結果します。</span><span class="sxs-lookup"><span data-stu-id="5961d-177">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="5961d-178">プロパティが変更された場合は、応答に新しい値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5961d-178">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="5961d-179">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5961d-179">This includes properties being set to null value.</span></span>
- <span data-ttu-id="5961d-180">プロパティが変更されていない場合は、プロパティが含まれていない応答ですべての。</span><span class="sxs-lookup"><span data-stu-id="5961d-180">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="5961d-181">(既定の動作と異なります)</span><span class="sxs-lookup"><span data-stu-id="5961d-181">(Different from the default behavior.)</span></span>

> <span data-ttu-id="5961d-182">**注:** ヘッダーを追加することができます、`deltaLink`デルタ ・ サイクルの時間内の任意の時点で要求します。</span><span class="sxs-lookup"><span data-stu-id="5961d-182">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="5961d-183">ヘッダーの応答に含まれるプロパティのセットにのみ影響し、デルタ ・ クエリを実行する方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="5961d-183">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="5961d-184">例</span><span class="sxs-lookup"><span data-stu-id="5961d-184">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="5961d-185">要求 1</span><span class="sxs-lookup"><span data-stu-id="5961d-185">Request 1</span></span>

<span data-ttu-id="5961d-186">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5961d-186">The following is an example of the request.</span></span> <span data-ttu-id="5961d-187">ありません`$select`パラメーター、プロパティの既定のセットが追跡され、返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="5961d-187">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a><span data-ttu-id="5961d-188">応答 1</span><span class="sxs-lookup"><span data-stu-id="5961d-188">Response 1</span></span>

<span data-ttu-id="5961d-189">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="5961d-189">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="5961d-190">No`isOf`フィルターが使用されているため、directoryObject から派生したすべての型が返されます。</span><span class="sxs-lookup"><span data-stu-id="5961d-190">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="5961d-p120">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5961d-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
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
      "id": "string (identifier)",
      "jobTitle": "string",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="5961d-193">要求 2</span><span class="sxs-lookup"><span data-stu-id="5961d-193">Request 2</span></span>

<span data-ttu-id="5961d-194">次の使用例は、最小限に抑える別の応答の動作の使用を示しています。</span><span class="sxs-lookup"><span data-stu-id="5961d-194">The next example shows the use of the alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a><span data-ttu-id="5961d-195">応答 2</span><span class="sxs-lookup"><span data-stu-id="5961d-195">Response 2</span></span>

<span data-ttu-id="5961d-196">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="5961d-196">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="5961d-197">実際に変更されたプロパティだけが返されますを注意してください。</span><span class="sxs-lookup"><span data-stu-id="5961d-197">Note only the properties that have actually changed are returned.</span></span>

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
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="5961d-198">要求 3</span><span class="sxs-lookup"><span data-stu-id="5961d-198">Request 3</span></span>

<span data-ttu-id="5961d-199">次の例は、最初の要求を使用して、`isOf`のユーザーとグループのエンティティのみを除外する演算子。</span><span class="sxs-lookup"><span data-stu-id="5961d-199">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a><span data-ttu-id="5961d-200">応答 3</span><span class="sxs-lookup"><span data-stu-id="5961d-200">Response 3</span></span>

<span data-ttu-id="5961d-201">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="5961d-201">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="5961d-202">ユーザーとグループのオブジェクトのみが返されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="5961d-202">Note that only user and group objects are returned:</span></span>

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
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

- <span data-ttu-id="5961d-203">[グラフ データの変更を追跡するためにデルタのクエリを使用します](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="5961d-203">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="5961d-204">[ユーザーの増分の変更を取得](/graph/delta-query-users)します。</span><span class="sxs-lookup"><span data-stu-id="5961d-204">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
