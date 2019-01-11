---
title: 'directoryRole: デルタ'
description: Get を新しく作成するには、更新、または全体のリソースのコレクションのすべての読み取りを実行することがなくディレクトリの役割を削除します。 詳細については、デルタのクエリを使用するを参照してください。
localization_priority: Normal
ms.openlocfilehash: a46bcfd5c345763e7ab3d64ec780721f7052fbdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846467"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="7ad2b-104">directoryRole: デルタ</span><span class="sxs-lookup"><span data-stu-id="7ad2b-104">directoryRole: delta</span></span>

<span data-ttu-id="7ad2b-105">Get を新しく作成するには、更新、または全体のリソースのコレクションのすべての読み取りを実行することがなくディレクトリの役割を削除します。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-105">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="7ad2b-106">詳細については、[デルタのクエリを使用する](/graph/delta-query-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ad2b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7ad2b-107">Permissions</span></span>

<span data-ttu-id="7ad2b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ad2b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ad2b-110">Permission type</span></span>      | <span data-ttu-id="7ad2b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ad2b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ad2b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ad2b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ad2b-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ad2b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ad2b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ad2b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ad2b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-115">Not supported.</span></span>    |
|<span data-ttu-id="7ad2b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ad2b-116">Application</span></span> | <span data-ttu-id="7ad2b-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ad2b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ad2b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ad2b-118">HTTP request</span></span>

<span data-ttu-id="7ad2b-119">変更の追跡を開始するには、 [directoryRole](../resources/directoryrole.md)リソースで**デルタ**関数を含む要求を行います。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-119">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="7ad2b-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ad2b-120">Query parameters</span></span>

<span data-ttu-id="7ad2b-121">変更を追跡する一連の 1 つまたは複数の**delta**関数の呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="7ad2b-122">任意のクエリ パラメーターを使用する場合 (以外の`$deltatoken`と`$skiptoken`)、**デルタ**の初期要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="7ad2b-123">Microsoft Graph が自動的に任意指定のパラメーターをエンコードのトークンの部分に、`nextLink`または`deltaLink`の応答で提供される URL です。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="7ad2b-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="7ad2b-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="7ad2b-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ad2b-126">Query parameter</span></span>      | <span data-ttu-id="7ad2b-127">種類</span><span class="sxs-lookup"><span data-stu-id="7ad2b-127">Type</span></span>   |<span data-ttu-id="7ad2b-128">説明</span><span class="sxs-lookup"><span data-stu-id="7ad2b-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ad2b-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="7ad2b-129">$deltatoken</span></span> | <span data-ttu-id="7ad2b-130">文字列</span><span class="sxs-lookup"><span data-stu-id="7ad2b-130">string</span></span> | <span data-ttu-id="7ad2b-131">返される[トークンの状態](/graph/delta-query-overview)、`deltaLink`の変更の追跡には、そのラウンドの完了を示す前の**デルタ**関数呼び出し、同じリソースを収集するための URL です。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="7ad2b-132">保存し、全体を適用する`deltaLink`コレクションの変更履歴の次のラウンドの最初の要求にこのトークンを含む URL です。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="7ad2b-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="7ad2b-133">$skiptoken</span></span> | <span data-ttu-id="7ad2b-134">文字列</span><span class="sxs-lookup"><span data-stu-id="7ad2b-134">string</span></span> | <span data-ttu-id="7ad2b-135">返される[トークンの状態](/graph/delta-query-overview)、`nextLink`で同じリソースのコレクションを追跡するにさらに変更が加えられたことを示す前の**デルタ**関数の呼び出しの URL です。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="7ad2b-136">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ad2b-136">OData query parameters</span></span>

<span data-ttu-id="7ad2b-137">このメソッドは、応答をカスタマイズするため、OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-137">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="7ad2b-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="7ad2b-140">サポートが制限されて`$filter`。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-140">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="7ad2b-141">サポートされる唯一の`$filter`の id で特定のリソースに対する変更を追跡するための式が:`$filter=id+eq+{value}`または`$filter=id+eq+{value1}+or+id+eq+{value2}`。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="7ad2b-142">URL の最大長を指定することができます id の数が制限されます。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-142">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ad2b-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ad2b-143">Request headers</span></span>

| <span data-ttu-id="7ad2b-144">名前</span><span class="sxs-lookup"><span data-stu-id="7ad2b-144">Name</span></span>       | <span data-ttu-id="7ad2b-145">説明</span><span class="sxs-lookup"><span data-stu-id="7ad2b-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7ad2b-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ad2b-146">Authorization</span></span>  | <span data-ttu-id="7ad2b-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="7ad2b-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="7ad2b-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ad2b-148">Content-Type</span></span>  | <span data-ttu-id="7ad2b-149">application/json</span><span class="sxs-lookup"><span data-stu-id="7ad2b-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ad2b-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ad2b-150">Request body</span></span>

<span data-ttu-id="7ad2b-151">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="7ad2b-152">応答</span><span class="sxs-lookup"><span data-stu-id="7ad2b-152">Response</span></span>

<span data-ttu-id="7ad2b-153">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[directoryRole](../resources/directoryrole.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-153">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="7ad2b-154">応答にも含まれています、`nextLink`の URL、または`deltaLink`URL です。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="7ad2b-155">場合、`nextLink`の URL が返されますが、セッション内で取得するデータのページを追加します。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="7ad2b-156">アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="7ad2b-157">場合、`deltaLink`の URL が返される、返されるリソースの既存の状態に関する多くのデータはありません。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="7ad2b-158">保存`deltaLink`の URL、将来的に、リソースへの変更の詳細については、次の**デルタ ・** 呼び出しに適用するとします。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-158">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="7ad2b-159">例</span><span class="sxs-lookup"><span data-stu-id="7ad2b-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7ad2b-160">要求</span><span class="sxs-lookup"><span data-stu-id="7ad2b-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="7ad2b-161">応答</span><span class="sxs-lookup"><span data-stu-id="7ad2b-161">Response</span></span>

<span data-ttu-id="7ad2b-p111">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

### <a name="see-also"></a><span data-ttu-id="7ad2b-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ad2b-164">See also</span></span>

- <span data-ttu-id="7ad2b-165">詳細については[Microsoft のグラフのデータの変更を追跡するためにデルタのクエリを使用します。](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="7ad2b-165">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview) for more details</span></span>
- <span data-ttu-id="7ad2b-166">要求の例については、「[ユーザーに対する増分の変更の取得](/graph/delta-query-users)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7ad2b-166">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
