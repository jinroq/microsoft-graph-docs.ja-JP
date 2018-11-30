---
title: 'directoryRole: デルタ'
description: Get を新しく作成するには、更新、または全体のリソースのコレクションのすべての読み取りを実行することがなくディレクトリの役割を削除します。 詳細については、デルタのクエリを使用するを参照してください。
ms.openlocfilehash: b426dd10ead2d1fc34c1d64aa235c343e8e71c3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066691"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="2b84b-104">directoryRole: デルタ</span><span class="sxs-lookup"><span data-stu-id="2b84b-104">directoryRole: delta</span></span>

> <span data-ttu-id="2b84b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b84b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b84b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b84b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b84b-107">Get を新しく作成するには、更新、または全体のリソースのコレクションのすべての読み取りを実行することがなくディレクトリの役割を削除します。</span><span class="sxs-lookup"><span data-stu-id="2b84b-107">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="2b84b-108">詳細については、[デルタのクエリを使用する](/graph/delta-query-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b84b-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b84b-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b84b-109">Permissions</span></span>

<span data-ttu-id="2b84b-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b84b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2b84b-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b84b-112">Permission type</span></span>      | <span data-ttu-id="2b84b-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b84b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b84b-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b84b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2b84b-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b84b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2b84b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b84b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b84b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b84b-117">Not supported.</span></span>    |
|<span data-ttu-id="2b84b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b84b-118">Application</span></span> | <span data-ttu-id="2b84b-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b84b-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b84b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b84b-120">HTTP request</span></span>

<span data-ttu-id="2b84b-121">変更の追跡を開始するには、directoryRole リソースでデルタ関数を含む要求を行います。</span><span class="sxs-lookup"><span data-stu-id="2b84b-121">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

### <a name="query-parameters"></a><span data-ttu-id="2b84b-122">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2b84b-122">Query parameters</span></span>

<span data-ttu-id="2b84b-123">変更を追跡する一連の 1 つまたは複数の**delta**関数の呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="2b84b-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="2b84b-124">任意のクエリ パラメーターを使用する場合 (以外の`$deltatoken`と`$skiptoken`)、**デルタ**の初期要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b84b-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="2b84b-125">Microsoft Graph が自動的に任意指定のパラメーターをエンコードのトークンの部分に、`nextLink`または`deltaLink`の応答で提供される URL です。</span><span class="sxs-lookup"><span data-stu-id="2b84b-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="2b84b-126">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="2b84b-126">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="2b84b-127">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="2b84b-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="2b84b-128">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2b84b-128">Query parameter</span></span>      | <span data-ttu-id="2b84b-129">種類</span><span class="sxs-lookup"><span data-stu-id="2b84b-129">Type</span></span>   |<span data-ttu-id="2b84b-130">説明</span><span class="sxs-lookup"><span data-stu-id="2b84b-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2b84b-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="2b84b-131">$deltatoken</span></span> | <span data-ttu-id="2b84b-132">文字列</span><span class="sxs-lookup"><span data-stu-id="2b84b-132">string</span></span> | <span data-ttu-id="2b84b-133">返される[トークンの状態](/graph/delta-query-overview)、`deltaLink`の変更の追跡には、そのラウンドの完了を示す前の**デルタ**関数呼び出し、同じリソースを収集するための URL です。</span><span class="sxs-lookup"><span data-stu-id="2b84b-133">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="2b84b-134">保存し、全体を適用する`deltaLink`コレクションの変更履歴の次のラウンドの最初の要求にこのトークンを含む URL です。</span><span class="sxs-lookup"><span data-stu-id="2b84b-134">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="2b84b-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="2b84b-135">$skiptoken</span></span> | <span data-ttu-id="2b84b-136">文字列</span><span class="sxs-lookup"><span data-stu-id="2b84b-136">string</span></span> | <span data-ttu-id="2b84b-137">返される[トークンの状態](/graph/delta-query-overview)、`nextLink`で同じリソースのコレクションを追跡するにさらに変更が加えられたことを示す前の**デルタ**関数の呼び出しの URL です。</span><span class="sxs-lookup"><span data-stu-id="2b84b-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="2b84b-138">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2b84b-138">Optional query parameters</span></span>

<span data-ttu-id="2b84b-139">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b84b-139">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="2b84b-p107">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="2b84b-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="2b84b-142">サポートが制限されて`$filter`。</span><span class="sxs-lookup"><span data-stu-id="2b84b-142">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="2b84b-143">サポートされる唯一の`$filter`の id で特定のリソースに対する変更を追跡するための式が:`$filter=id+eq+{value}`または`$filter=id+eq+{value1}+or+id+eq+{value2}`。</span><span class="sxs-lookup"><span data-stu-id="2b84b-143">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="2b84b-144">URL の最大長を指定することができます id の数が制限されます。</span><span class="sxs-lookup"><span data-stu-id="2b84b-144">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="2b84b-145">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b84b-145">Request headers</span></span>
| <span data-ttu-id="2b84b-146">名前</span><span class="sxs-lookup"><span data-stu-id="2b84b-146">Name</span></span>       | <span data-ttu-id="2b84b-147">説明</span><span class="sxs-lookup"><span data-stu-id="2b84b-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2b84b-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b84b-148">Authorization</span></span>  | <span data-ttu-id="2b84b-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="2b84b-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="2b84b-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b84b-150">Content-Type</span></span>  | <span data-ttu-id="2b84b-151">application/json</span><span class="sxs-lookup"><span data-stu-id="2b84b-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b84b-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b84b-152">Request body</span></span>
<span data-ttu-id="2b84b-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2b84b-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="2b84b-154">応答</span><span class="sxs-lookup"><span data-stu-id="2b84b-154">Response</span></span>

<span data-ttu-id="2b84b-155">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[directoryRole](../resources/directoryrole.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2b84b-155">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="2b84b-156">応答には、nextLink URL または deltaLink の URL も含まれています。</span><span class="sxs-lookup"><span data-stu-id="2b84b-156">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="2b84b-157">場合、`nextLink`の URL が返されますが、セッション内で取得するデータのページを追加します。</span><span class="sxs-lookup"><span data-stu-id="2b84b-157">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="2b84b-158">アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="2b84b-158">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="2b84b-159">場合、`deltaLink`の URL が返される、返されるリソースの既存の状態に関する多くのデータはありません。</span><span class="sxs-lookup"><span data-stu-id="2b84b-159">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="2b84b-160">永続化し、使用して、 `deltaLink` 、将来的にリソースへの変更に関する説明への URL です。</span><span class="sxs-lookup"><span data-stu-id="2b84b-160">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="2b84b-161">参照先:</span><span class="sxs-lookup"><span data-stu-id="2b84b-161">See:</span></span></br>
- <span data-ttu-id="2b84b-162">詳細については、「[デルタ クエリの使用](/graph/delta-query-overview)」をご覧ください</span><span class="sxs-lookup"><span data-stu-id="2b84b-162">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="2b84b-163">要求の例については、「[ユーザーに対する増分の変更の取得](/graph/delta-query-users)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2b84b-163">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="2b84b-164">例</span><span class="sxs-lookup"><span data-stu-id="2b84b-164">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b84b-165">要求</span><span class="sxs-lookup"><span data-stu-id="2b84b-165">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="2b84b-166">応答</span><span class="sxs-lookup"><span data-stu-id="2b84b-166">Response</span></span>
<span data-ttu-id="2b84b-p112">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2b84b-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->