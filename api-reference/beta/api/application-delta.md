---
title: 'アプリケーション: デルタ'
description: Get を新しく作成するには、更新、または全体のリソースのコレクションのすべての読み取りを実行しなくてもアプリケーションを削除します。 詳細については、デルタのクエリを使用するを参照してください。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 13b6f7809cf47edcc9de8c9ddfb052645b15f25a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517072"
---
# <a name="application-delta"></a><span data-ttu-id="148f9-104">アプリケーション: デルタ</span><span class="sxs-lookup"><span data-stu-id="148f9-104">application: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="148f9-105">Get を新しく作成するには、更新、または全体のリソースのコレクションのすべての読み取りを実行しなくてもアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="148f9-105">Get newly created, updated, or deleted applications without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="148f9-106">詳細については、[デルタのクエリを使用する](/graph/delta-query-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="148f9-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="148f9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="148f9-107">Permissions</span></span>

<span data-ttu-id="148f9-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="148f9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="148f9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="148f9-110">Permission type</span></span>      | <span data-ttu-id="148f9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="148f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="148f9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="148f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="148f9-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="148f9-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="148f9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="148f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="148f9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="148f9-115">Not supported.</span></span>    |
|<span data-ttu-id="148f9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="148f9-116">Application</span></span> | <span data-ttu-id="148f9-117">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="148f9-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="148f9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="148f9-118">HTTP request</span></span>

<span data-ttu-id="148f9-119">変更の追跡を開始するには、アプリケーション リソースにデルタ関数を含む要求を行います。</span><span class="sxs-lookup"><span data-stu-id="148f9-119">To begin tracking changes, you make a request including the delta function on the application resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a><span data-ttu-id="148f9-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="148f9-120">Query parameters</span></span>

<span data-ttu-id="148f9-121">変更を追跡する一連の 1 つまたは複数の**delta**関数の呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="148f9-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="148f9-122">任意のクエリ パラメーターを使用する場合 (以外の`$deltatoken`と`$skiptoken`)、**デルタ**の初期要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="148f9-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="148f9-123">Microsoft Graph が自動的に任意指定のパラメーターをエンコードのトークンの部分に、`nextLink`または`deltaLink`の応答で提供される URL です。</span><span class="sxs-lookup"><span data-stu-id="148f9-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="148f9-124">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="148f9-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="148f9-125">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="148f9-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="148f9-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="148f9-126">Query parameter</span></span>      | <span data-ttu-id="148f9-127">種類</span><span class="sxs-lookup"><span data-stu-id="148f9-127">Type</span></span>   |<span data-ttu-id="148f9-128">説明</span><span class="sxs-lookup"><span data-stu-id="148f9-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="148f9-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="148f9-129">$deltatoken</span></span> | <span data-ttu-id="148f9-130">string</span><span class="sxs-lookup"><span data-stu-id="148f9-130">string</span></span> | <span data-ttu-id="148f9-131">返される[トークンの状態](/graph/delta-query-overview)、`deltaLink`の変更の追跡には、そのラウンドの完了を示す前の**デルタ**関数呼び出し、同じリソースを収集するための URL です。</span><span class="sxs-lookup"><span data-stu-id="148f9-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="148f9-132">保存し、全体を適用する`deltaLink`コレクションの変更履歴の次のラウンドの最初の要求にこのトークンを含む URL です。</span><span class="sxs-lookup"><span data-stu-id="148f9-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="148f9-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="148f9-133">$skiptoken</span></span> | <span data-ttu-id="148f9-134">string</span><span class="sxs-lookup"><span data-stu-id="148f9-134">string</span></span> | <span data-ttu-id="148f9-135">返される[トークンの状態](/graph/delta-query-overview)、`nextLink`で同じリソースのコレクションを追跡するにさらに変更が加えられたことを示す前の**デルタ**関数の呼び出しの URL です。</span><span class="sxs-lookup"><span data-stu-id="148f9-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="148f9-136">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="148f9-136">Optional query parameters</span></span>

<span data-ttu-id="148f9-137">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="148f9-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="148f9-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="148f9-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="148f9-140">サポートが制限されて`$filter`。</span><span class="sxs-lookup"><span data-stu-id="148f9-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="148f9-141">サポートされる唯一の`$filter`の id で特定のリソースに対する変更を追跡するための式が:`$filter=id+eq+{value}`または`$filter=id+eq+{value1}+or+id+eq+{value2}`。</span><span class="sxs-lookup"><span data-stu-id="148f9-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="148f9-142">URL の最大長を指定することができます id の数が制限されます。</span><span class="sxs-lookup"><span data-stu-id="148f9-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="148f9-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="148f9-143">Request headers</span></span>
| <span data-ttu-id="148f9-144">名前</span><span class="sxs-lookup"><span data-stu-id="148f9-144">Name</span></span>       | <span data-ttu-id="148f9-145">説明</span><span class="sxs-lookup"><span data-stu-id="148f9-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="148f9-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="148f9-146">Authorization</span></span>  | <span data-ttu-id="148f9-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="148f9-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="148f9-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="148f9-148">Content-Type</span></span>  | <span data-ttu-id="148f9-149">application/json</span><span class="sxs-lookup"><span data-stu-id="148f9-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="148f9-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="148f9-150">Request body</span></span>
<span data-ttu-id="148f9-151">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="148f9-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="148f9-152">応答</span><span class="sxs-lookup"><span data-stu-id="148f9-152">Response</span></span>

<span data-ttu-id="148f9-153">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[アプリケーション](../resources/application.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="148f9-153">If successful, this method returns `200 OK` response code and [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="148f9-154">応答には、nextLink URL または deltaLink の URL も含まれています。</span><span class="sxs-lookup"><span data-stu-id="148f9-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="148f9-155">場合、`nextLink`の URL が返されますが、セッション内で取得するデータのページを追加します。</span><span class="sxs-lookup"><span data-stu-id="148f9-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="148f9-156">アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="148f9-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="148f9-157">場合、`deltaLink`の URL が返される、返されるリソースの既存の状態に関する多くのデータはありません。</span><span class="sxs-lookup"><span data-stu-id="148f9-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="148f9-158">永続化し、使用して、 `deltaLink` 、将来的にリソースへの変更に関する説明への URL です。</span><span class="sxs-lookup"><span data-stu-id="148f9-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="148f9-159">参照先:</span><span class="sxs-lookup"><span data-stu-id="148f9-159">See:</span></span></br>
- <span data-ttu-id="148f9-160">詳細については、「[デルタ クエリの使用](/graph/delta-query-overview)」をご覧ください</span><span class="sxs-lookup"><span data-stu-id="148f9-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="148f9-161">要求の例については、「[ユーザーに対する増分の変更の取得](/graph/delta-query-users)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="148f9-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="148f9-162">例</span><span class="sxs-lookup"><span data-stu-id="148f9-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="148f9-163">要求</span><span class="sxs-lookup"><span data-stu-id="148f9-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```http
GET https://graph.microsoft.com/beta/applications/delta
```

##### <a name="response"></a><span data-ttu-id="148f9-164">応答</span><span class="sxs-lookup"><span data-stu-id="148f9-164">Response</span></span>
<span data-ttu-id="148f9-p111">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="148f9-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
