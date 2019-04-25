---
title: 'serviceprincipal: delta'
description: リソースコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたサービスプリンシパルを取得します。 詳細については、「デルタクエリの使用」を参照してください。
localization_priority: Normal
ms.openlocfilehash: ed0cf279d1d076e324d24e1774734e9aa14a6b34
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545496"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="89ec2-104">serviceprincipal: delta</span><span class="sxs-lookup"><span data-stu-id="89ec2-104">servicePrincipal: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89ec2-105">リソースコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたサービスプリンシパルを取得します。</span><span class="sxs-lookup"><span data-stu-id="89ec2-105">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="89ec2-106">詳細については、「[デルタクエリの使用](/graph/delta-query-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89ec2-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="89ec2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89ec2-107">Permissions</span></span>

<span data-ttu-id="89ec2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89ec2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="89ec2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89ec2-110">Permission type</span></span>      | <span data-ttu-id="89ec2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89ec2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89ec2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89ec2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89ec2-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="89ec2-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="89ec2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89ec2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89ec2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89ec2-115">Not supported.</span></span>    |
|<span data-ttu-id="89ec2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89ec2-116">Application</span></span> | <span data-ttu-id="89ec2-117">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="89ec2-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89ec2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89ec2-118">HTTP request</span></span>

<span data-ttu-id="89ec2-119">変更の追跡を開始するには、serviceprincipal リソースにデルタ関数を含む要求を行います。</span><span class="sxs-lookup"><span data-stu-id="89ec2-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="89ec2-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="89ec2-120">Query parameters</span></span>

<span data-ttu-id="89ec2-121">変更の追跡では、1回以上の**デルタ**関数呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="89ec2-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="89ec2-122">クエリパラメーター ( `$deltatoken`および`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="89ec2-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="89ec2-123">Microsoft Graph は、指定されたパラメーターを、 `nextLink`応答で指定`deltaLink`されたまたは URL のトークン部分に自動的にエンコードします。</span><span class="sxs-lookup"><span data-stu-id="89ec2-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="89ec2-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="89ec2-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="89ec2-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="89ec2-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="89ec2-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="89ec2-126">Query parameter</span></span>      | <span data-ttu-id="89ec2-127">型</span><span class="sxs-lookup"><span data-stu-id="89ec2-127">Type</span></span>   |<span data-ttu-id="89ec2-128">説明</span><span class="sxs-lookup"><span data-stu-id="89ec2-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89ec2-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="89ec2-129">$deltatoken</span></span> | <span data-ttu-id="89ec2-130">string</span><span class="sxs-lookup"><span data-stu-id="89ec2-130">string</span></span> | <span data-ttu-id="89ec2-131">同じリソースコレクションに対する前`deltaLink`の**デルタ**関数呼び出しの URL で返された[状態トークン](/graph/delta-query-overview)。変更追跡のラウンドが終了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="89ec2-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="89ec2-132">そのコレクションの次の`deltaLink`ラウンドの変更追跡の最初の要求で、このトークンを含む URL 全体を保存して適用します。</span><span class="sxs-lookup"><span data-stu-id="89ec2-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="89ec2-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="89ec2-133">$skiptoken</span></span> | <span data-ttu-id="89ec2-134">string</span><span class="sxs-lookup"><span data-stu-id="89ec2-134">string</span></span> | <span data-ttu-id="89ec2-135">前の**デルタ**関数呼び出しの`nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じリソースコレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="89ec2-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="89ec2-136">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="89ec2-136">Optional query parameters</span></span>

<span data-ttu-id="89ec2-137">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="89ec2-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="89ec2-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="89ec2-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="89ec2-140">次のサポートに`$filter`制限があります。</span><span class="sxs-lookup"><span data-stu-id="89ec2-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="89ec2-141">サポートされ`$filter`ている唯一の式は、id: `$filter=id+eq+{value}`または`$filter=id+eq+{value1}+or+id+eq+{value2}`を使用して特定のリソースの変更を追跡することです。</span><span class="sxs-lookup"><span data-stu-id="89ec2-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="89ec2-142">指定できる id の数は、URL の最大の長さによって制限されます。</span><span class="sxs-lookup"><span data-stu-id="89ec2-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="89ec2-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89ec2-143">Request headers</span></span>
| <span data-ttu-id="89ec2-144">名前</span><span class="sxs-lookup"><span data-stu-id="89ec2-144">Name</span></span>       | <span data-ttu-id="89ec2-145">説明</span><span class="sxs-lookup"><span data-stu-id="89ec2-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89ec2-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="89ec2-146">Authorization</span></span>  | <span data-ttu-id="89ec2-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="89ec2-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="89ec2-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89ec2-148">Content-Type</span></span>  | <span data-ttu-id="89ec2-149">application/json</span><span class="sxs-lookup"><span data-stu-id="89ec2-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="89ec2-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="89ec2-150">Request body</span></span>
<span data-ttu-id="89ec2-151">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="89ec2-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="89ec2-152">応答</span><span class="sxs-lookup"><span data-stu-id="89ec2-152">Response</span></span>

<span data-ttu-id="89ec2-153">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[serviceprincipal](../resources/serviceprincipal.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89ec2-153">If successful, this method returns `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="89ec2-154">応答には、nextlink url または deltaLink url も含まれます。</span><span class="sxs-lookup"><span data-stu-id="89ec2-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="89ec2-155">URL が返される場合は、セッションに取得するデータの追加ページがあります。`nextLink`</span><span class="sxs-lookup"><span data-stu-id="89ec2-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="89ec2-156">アプリケーションは、応答に`nextLink` `deltaLink` url が含まれるまで、url を使用して要求を引き続き行います。</span><span class="sxs-lookup"><span data-stu-id="89ec2-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="89ec2-157">URL が返される場合、返されるリソースの既存の状態に関するデータはありません。</span><span class="sxs-lookup"><span data-stu-id="89ec2-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="89ec2-158">今後のリソースの`deltaLink`変更点については、URL を永続化して使用してください。</span><span class="sxs-lookup"><span data-stu-id="89ec2-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="89ec2-159">参照先:</span><span class="sxs-lookup"><span data-stu-id="89ec2-159">See:</span></span></br>
- <span data-ttu-id="89ec2-160">詳細については、「[デルタ クエリの使用](/graph/delta-query-overview)」をご覧ください</span><span class="sxs-lookup"><span data-stu-id="89ec2-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="89ec2-161">要求の例については、「[ユーザーに対する増分の変更の取得](/graph/delta-query-users)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="89ec2-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="89ec2-162">例</span><span class="sxs-lookup"><span data-stu-id="89ec2-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89ec2-163">要求</span><span class="sxs-lookup"><span data-stu-id="89ec2-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```

##### <a name="response"></a><span data-ttu-id="89ec2-164">応答</span><span class="sxs-lookup"><span data-stu-id="89ec2-164">Response</span></span>
<span data-ttu-id="89ec2-p111">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="89ec2-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/serviceprincipal-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
