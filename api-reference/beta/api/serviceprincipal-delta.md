---
title: 'servicePrincipal: delta'
description: リソースコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたサービスプリンシパルを取得します。 詳細については、「デルタクエリの使用」を参照してください。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5f9c6a7da170acd33e09231eb482e594b33e3824
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364083"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="83c10-104">servicePrincipal: delta</span><span class="sxs-lookup"><span data-stu-id="83c10-104">servicePrincipal: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83c10-105">リソースコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたサービスプリンシパルを取得します。</span><span class="sxs-lookup"><span data-stu-id="83c10-105">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="83c10-106">詳細については、「[デルタクエリの使用](/graph/delta-query-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83c10-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="83c10-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83c10-107">Permissions</span></span>

<span data-ttu-id="83c10-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83c10-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83c10-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83c10-110">Permission type</span></span>      | <span data-ttu-id="83c10-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83c10-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83c10-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83c10-112">Delegated (work or school account)</span></span> | <span data-ttu-id="83c10-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83c10-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83c10-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83c10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83c10-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83c10-115">Not supported.</span></span>    |
|<span data-ttu-id="83c10-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83c10-116">Application</span></span> | <span data-ttu-id="83c10-117">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="83c10-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83c10-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83c10-118">HTTP request</span></span>

<span data-ttu-id="83c10-119">変更の追跡を開始するには、servicePrincipal リソースにデルタ関数を含む要求を行います。</span><span class="sxs-lookup"><span data-stu-id="83c10-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="83c10-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="83c10-120">Query parameters</span></span>

<span data-ttu-id="83c10-121">変更の追跡では、1回以上の**デルタ**関数呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="83c10-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="83c10-122">任意のクエリ パラメーター (`$deltatoken` と`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83c10-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="83c10-123">Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。</span><span class="sxs-lookup"><span data-stu-id="83c10-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="83c10-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="83c10-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="83c10-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="83c10-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="83c10-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="83c10-126">Query parameter</span></span>      | <span data-ttu-id="83c10-127">種類</span><span class="sxs-lookup"><span data-stu-id="83c10-127">Type</span></span>   |<span data-ttu-id="83c10-128">説明</span><span class="sxs-lookup"><span data-stu-id="83c10-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="83c10-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="83c10-129">$deltatoken</span></span> | <span data-ttu-id="83c10-130">string</span><span class="sxs-lookup"><span data-stu-id="83c10-130">string</span></span> | <span data-ttu-id="83c10-131">同じリソースコレクションに対する前`deltaLink`の**デルタ**関数呼び出しの URL で返された[状態トークン](/graph/delta-query-overview)。変更追跡のラウンドが終了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="83c10-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="83c10-132">そのコレクションの次の`deltaLink`ラウンドの変更追跡の最初の要求で、このトークンを含む URL 全体を保存して適用します。</span><span class="sxs-lookup"><span data-stu-id="83c10-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="83c10-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="83c10-133">$skiptoken</span></span> | <span data-ttu-id="83c10-134">string</span><span class="sxs-lookup"><span data-stu-id="83c10-134">string</span></span> | <span data-ttu-id="83c10-135">前の**デルタ**関数呼び出しの`nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じリソースコレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="83c10-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="83c10-136">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="83c10-136">Optional query parameters</span></span>

<span data-ttu-id="83c10-137">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="83c10-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="83c10-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="83c10-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="83c10-140">`$filter` に対するサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="83c10-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="83c10-141">サポートされ`$filter`ている唯一の式は、id: `$filter=id+eq+{value}`または`$filter=id+eq+{value1}+or+id+eq+{value2}`を使用して特定のリソースの変更を追跡することです。</span><span class="sxs-lookup"><span data-stu-id="83c10-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="83c10-142">指定できる id の数は、URL の最大の長さによって制限されます。</span><span class="sxs-lookup"><span data-stu-id="83c10-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="83c10-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83c10-143">Request headers</span></span>
| <span data-ttu-id="83c10-144">名前</span><span class="sxs-lookup"><span data-stu-id="83c10-144">Name</span></span>       | <span data-ttu-id="83c10-145">説明</span><span class="sxs-lookup"><span data-stu-id="83c10-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="83c10-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="83c10-146">Authorization</span></span>  | <span data-ttu-id="83c10-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="83c10-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="83c10-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83c10-148">Content-Type</span></span>  | <span data-ttu-id="83c10-149">application/json</span><span class="sxs-lookup"><span data-stu-id="83c10-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="83c10-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="83c10-150">Request body</span></span>
<span data-ttu-id="83c10-151">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83c10-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="83c10-152">応答</span><span class="sxs-lookup"><span data-stu-id="83c10-152">Response</span></span>

<span data-ttu-id="83c10-153">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[serviceprincipal](../resources/serviceprincipal.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="83c10-153">If successful, this method returns `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="83c10-154">応答には、nextLink URL または deltaLink URL も含まれます。</span><span class="sxs-lookup"><span data-stu-id="83c10-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="83c10-155">URL が返される場合は、セッションに取得するデータの追加ページがあります。`nextLink`</span><span class="sxs-lookup"><span data-stu-id="83c10-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="83c10-156">アプリケーションは`deltaLink` URL が応答に含まれるまで`nextLink` URLを使用して要求を続けます。</span><span class="sxs-lookup"><span data-stu-id="83c10-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="83c10-157">URL が返される場合、返されるリソースの既存の状態に関するデータはありません。</span><span class="sxs-lookup"><span data-stu-id="83c10-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="83c10-158">今後のリソースの`deltaLink`変更点については、URL を永続化して使用してください。</span><span class="sxs-lookup"><span data-stu-id="83c10-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="83c10-159">参照先:</span><span class="sxs-lookup"><span data-stu-id="83c10-159">See:</span></span></br>
- <span data-ttu-id="83c10-160">詳細については、「[デルタ クエリの使用](/graph/delta-query-overview)」をご覧ください</span><span class="sxs-lookup"><span data-stu-id="83c10-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="83c10-161">要求の例については、「[ユーザーに対する増分の変更の取得](/graph/delta-query-users)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="83c10-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="83c10-162">例</span><span class="sxs-lookup"><span data-stu-id="83c10-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83c10-163">要求</span><span class="sxs-lookup"><span data-stu-id="83c10-163">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="83c10-164">プロトコル</span><span class="sxs-lookup"><span data-stu-id="83c10-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="83c10-165">C#</span><span class="sxs-lookup"><span data-stu-id="83c10-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83c10-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83c10-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83c10-167">目的-C</span><span class="sxs-lookup"><span data-stu-id="83c10-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="83c10-168">Java</span><span class="sxs-lookup"><span data-stu-id="83c10-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="83c10-169">応答</span><span class="sxs-lookup"><span data-stu-id="83c10-169">Response</span></span>
<span data-ttu-id="83c10-p111">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83c10-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.nextLink":"https://graph.microsoft.com/beta/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
     {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
