---
title: 'directoryobject: delta'
description: 単一のデルタクエリで、次の種類の新規作成、更新、または削除されたディレクトリオブジェクトを取得します。ユーザー、グループ、組織の連絡先。 詳細については、「変更履歴」を参照してください。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9dd3c835070581314b1620c0012237c9beca5b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326075"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="a5ea2-104">directoryobject: delta</span><span class="sxs-lookup"><span data-stu-id="a5ea2-104">directoryObject: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5ea2-105">単一のデルタクエリで、次の種類の新規作成、更新、または削除されたディレクトリオブジェクトを取得します。[ユーザー](../resources/user.md)、[グループ](../resources/group.md)、[組織の連絡先](../resources/orgcontact.md)。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-105">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="a5ea2-106">詳細については、「[変更履歴](/graph/delta-query-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5ea2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5ea2-107">Permissions</span></span>

<span data-ttu-id="a5ea2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5ea2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5ea2-110">Permission type</span></span>      | <span data-ttu-id="a5ea2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5ea2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5ea2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5ea2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5ea2-113">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5ea2-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="a5ea2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5ea2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5ea2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-115">Not supported.</span></span>  |
|<span data-ttu-id="a5ea2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5ea2-116">Application</span></span> | <span data-ttu-id="a5ea2-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5ea2-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5ea2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5ea2-118">HTTP request</span></span>

<span data-ttu-id="a5ea2-119">変更の追跡を開始するには、directoryobjects リソースにデルタ関数を含む要求を行います。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-119">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a5ea2-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5ea2-120">Query parameters</span></span>

<span data-ttu-id="a5ea2-121">変更の追跡では、1回以上の**デルタ**関数呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="a5ea2-122">クエリパラメーター ( `$deltatoken`および`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="a5ea2-123">Microsoft Graph は、指定されたパラメーターを、 `nextLink`応答で指定`deltaLink`されたまたは URL のトークン部分に自動的にエンコードします。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="a5ea2-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="a5ea2-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="a5ea2-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5ea2-126">Query parameter</span></span> | <span data-ttu-id="a5ea2-127">種類</span><span class="sxs-lookup"><span data-stu-id="a5ea2-127">Type</span></span> |<span data-ttu-id="a5ea2-128">説明</span><span class="sxs-lookup"><span data-stu-id="a5ea2-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5ea2-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a5ea2-129">$deltatoken</span></span> | <span data-ttu-id="a5ea2-130">string</span><span class="sxs-lookup"><span data-stu-id="a5ea2-130">string</span></span> | <span data-ttu-id="a5ea2-p105">同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a5ea2-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a5ea2-133">$skiptoken</span></span> | <span data-ttu-id="a5ea2-134">string</span><span class="sxs-lookup"><span data-stu-id="a5ea2-134">string</span></span> | <span data-ttu-id="a5ea2-135">前の**デルタ**関数の `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="a5ea2-136">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5ea2-136">OData query parameters</span></span>

<span data-ttu-id="a5ea2-137">このメソッドは、応答をカスタマイズするためのオプションの OData クエリパラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="a5ea2-138">特別な`isOf`演算子`$filter`と共にを使用して、directoryobject から派生した型のサブセットをフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-138">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="a5ea2-139">を使用して複数の式`or`を組み合わせることができます。これにより、1つのデルタクエリで複数の種類を追跡できます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-139">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="a5ea2-140">詳細については、 [3 番目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-140">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5ea2-141">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5ea2-141">Request headers</span></span>

| <span data-ttu-id="a5ea2-142">名前</span><span class="sxs-lookup"><span data-stu-id="a5ea2-142">Name</span></span>       | <span data-ttu-id="a5ea2-143">説明</span><span class="sxs-lookup"><span data-stu-id="a5ea2-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a5ea2-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5ea2-144">Authorization</span></span>  | <span data-ttu-id="a5ea2-145">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="a5ea2-145">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="a5ea2-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5ea2-146">Content-Type</span></span>  | <span data-ttu-id="a5ea2-147">application/json</span><span class="sxs-lookup"><span data-stu-id="a5ea2-147">application/json</span></span> |
| <span data-ttu-id="a5ea2-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="a5ea2-148">Prefer</span></span> | <span data-ttu-id="a5ea2-149">戻り値 = 最小</span><span class="sxs-lookup"><span data-stu-id="a5ea2-149">return=minimal</span></span> <br><br><span data-ttu-id="a5ea2-150">を`deltaLink`使用する要求でこのヘッダーを指定すると、最後のラウンド以降に変更されたオブジェクトプロパティのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-150">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="a5ea2-151">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5ea2-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5ea2-152">Request body</span></span>

<span data-ttu-id="a5ea2-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="a5ea2-154">応答</span><span class="sxs-lookup"><span data-stu-id="a5ea2-154">Response</span></span>

<span data-ttu-id="a5ea2-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/directoryobject.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-155">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="a5ea2-156">応答には、 `nextLink` url または`deltaLink` url も含まれます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-156">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="a5ea2-157">URL が`nextLink`返される場合は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-157">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="a5ea2-158">これは、セッションで取得するデータのページが他にもあることを示しています。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-158">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="a5ea2-159">アプリケーションは、応答に`nextLink` `deltaLink` url が含まれるまで、url を使用して要求を引き続き行います。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-159">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="a5ea2-160">応答には、初期デルタクエリ要求と同じプロパティセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-160">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="a5ea2-161">これにより、デルタサイクルを開始するときに、オブジェクトの現在の完全な状態を取得できます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-161">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="a5ea2-162">URL が`deltaLink`返される場合は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-162">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="a5ea2-163">これは、返されるリソースの既存の状態に関するデータがないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-163">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="a5ea2-164">`deltaLink` URL を保存して使用し、次のラウンドでのリソースの変更について学習します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-164">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="a5ea2-165">`Prefer:return=minimal`ヘッダーを指定することもできます。これは、が発行`deltaLink`されてから変更されたプロパティのみを応答値に含めることを選択することです。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-165">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="a5ea2-166">Default: 初期デルタ要求と同じプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="a5ea2-166">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="a5ea2-167">既定では、次の`deltaLink`方法`nextLink`で、を使用して、または初期デルタクエリで選択されたものと同じプロパティを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-167">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="a5ea2-168">プロパティが変更されている場合、新しい値は応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-168">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="a5ea2-169">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-169">This includes properties being set to null value.</span></span>
- <span data-ttu-id="a5ea2-170">プロパティが変更されていない場合は、古い値が応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-170">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="a5ea2-171">プロパティが設定されていない場合は、応答には含まれません。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-171">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="a5ea2-172">**注:** この動作では、応答を見ることで、プロパティが変更されているかどうかを判断することはできません。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-172">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="a5ea2-173">また、デルタ応答は、すべてのプロパティ値を含むため、サイズが大きくなる傾向があります。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-173">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="a5ea2-174">代替方法: 変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="a5ea2-174">Alternative: return only the changed properties</span></span>

<span data-ttu-id="a5ea2-175">オプションの要求ヘッダーを追加`prefer:return=minimal`する--次のような動作になります。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-175">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="a5ea2-176">プロパティが変更されている場合、新しい値は応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-176">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="a5ea2-177">これには、null 値に設定されているプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-177">This includes properties being set to null value.</span></span>
- <span data-ttu-id="a5ea2-178">プロパティが変更されていない場合、プロパティは応答には含まれません。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-178">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="a5ea2-179">(既定の動作とは異なります)。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-179">(Different from the default behavior.)</span></span>

> <span data-ttu-id="a5ea2-180">**注:** このヘッダーは、デルタサイクルの`deltaLink`任意の時点で要求に追加できます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-180">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="a5ea2-181">ヘッダーは、応答に含まれているプロパティのセットにのみ影響し、デルタクエリの実行方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-181">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="a5ea2-182">例</span><span class="sxs-lookup"><span data-stu-id="a5ea2-182">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="a5ea2-183">要求 1</span><span class="sxs-lookup"><span data-stu-id="a5ea2-183">Request 1</span></span>

<span data-ttu-id="a5ea2-184">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-184">The following is an example of the request.</span></span> <span data-ttu-id="a5ea2-185">パラメーターがない`$select`ので、プロパティの既定のセットが追跡されて返されます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-185">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a><span data-ttu-id="a5ea2-186">応答 1</span><span class="sxs-lookup"><span data-stu-id="a5ea2-186">Response 1</span></span>

<span data-ttu-id="a5ea2-187">次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-187">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="a5ea2-188">フィルター `isOf`は使用されていないので、directoryobject から派生したすべての型が返されます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-188">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="a5ea2-189">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-189">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a5ea2-190">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-190">All the properties will be returned from an actual call.</span></span>

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

### <a name="request-2"></a><span data-ttu-id="a5ea2-191">要求 2</span><span class="sxs-lookup"><span data-stu-id="a5ea2-191">Request 2</span></span>

<span data-ttu-id="a5ea2-192">次の例は、代替の最小応答動作の使用法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-192">The next example shows the use of the alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a><span data-ttu-id="a5ea2-193">応答 2</span><span class="sxs-lookup"><span data-stu-id="a5ea2-193">Response 2</span></span>

<span data-ttu-id="a5ea2-194">次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-194">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="a5ea2-195">メモ実際に変更されたプロパティのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-195">Note only the properties that have actually changed are returned.</span></span>

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

### <a name="request-3"></a><span data-ttu-id="a5ea2-196">要求 3</span><span class="sxs-lookup"><span data-stu-id="a5ea2-196">Request 3</span></span>

<span data-ttu-id="a5ea2-197">次の例では、 `isOf`演算子を使用して、ユーザーエンティティとグループエンティティのみを除外する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-197">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a><span data-ttu-id="a5ea2-198">応答 3</span><span class="sxs-lookup"><span data-stu-id="a5ea2-198">Response 3</span></span>

<span data-ttu-id="a5ea2-199">次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-199">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="a5ea2-200">ユーザーオブジェクトとグループオブジェクトのみが返されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-200">Note that only user and group objects are returned:</span></span>

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

- <span data-ttu-id="a5ea2-201">[デルタクエリを使用して、Microsoft Graph データの変更を追跡](/graph/delta-query-overview)します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-201">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="a5ea2-202">[ユーザーに対する増分の変更を取得](/graph/delta-query-users)します。</span><span class="sxs-lookup"><span data-stu-id="a5ea2-202">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
