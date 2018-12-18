---
title: リストの使用
description: ユーザーに使用されるファイルの一覧を返す計算の把握。
author: simonhult
ms.openlocfilehash: 17f47e4e82d5cb038438b5d164c76371221de11a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342498"
---
# <a name="list-used"></a><span data-ttu-id="d7b0f-103">リストの使用</span><span class="sxs-lookup"><span data-stu-id="d7b0f-103">List used</span></span>

> <span data-ttu-id="d7b0f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7b0f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7b0f-106">ユーザーに使用されるファイルの一覧を返す計算の把握。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-106">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7b0f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7b0f-107">Permissions</span></span>
<span data-ttu-id="d7b0f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7b0f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7b0f-110">Permission type</span></span>      | <span data-ttu-id="d7b0f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7b0f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7b0f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7b0f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7b0f-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7b0f-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7b0f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7b0f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7b0f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-115">Not supported.</span></span>    |
|<span data-ttu-id="d7b0f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7b0f-116">Application</span></span> | <span data-ttu-id="d7b0f-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7b0f-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7b0f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7b0f-118">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="d7b0f-119">'LastModifiedDateTime' で並べ替えられた結果が返されます他のユーザーのドキュメントの使用を要求して、'lastAccessedDateTime' は、'lastModifiedDateTime' に設定されています。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-119">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7b0f-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d7b0f-120">Optional query parameters</span></span>
<span data-ttu-id="d7b0f-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d7b0f-122">使用することができます、`$filter`アイテムのフィルターを使用するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-122">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="d7b0f-123">などは、型に基づいています。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="d7b0f-124">コンテナーの種類に基づくか。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-124">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="d7b0f-125">使用可能なコンテナーの種類と[resourceVisualization](../resources/insights-resourcevisualization.md)内でフィルターの種類を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-125">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="d7b0f-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7b0f-126">Request headers</span></span>
| <span data-ttu-id="d7b0f-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7b0f-127">Header</span></span>       |  <span data-ttu-id="d7b0f-128">値</span><span class="sxs-lookup"><span data-stu-id="d7b0f-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="d7b0f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7b0f-129">Authorization</span></span>  | <span data-ttu-id="d7b0f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d7b0f-132">承諾</span><span class="sxs-lookup"><span data-stu-id="d7b0f-132">Accept</span></span>  | <span data-ttu-id="d7b0f-133">application/json</span><span class="sxs-lookup"><span data-stu-id="d7b0f-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7b0f-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7b0f-134">Request body</span></span>
<span data-ttu-id="d7b0f-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7b0f-136">応答</span><span class="sxs-lookup"><span data-stu-id="d7b0f-136">Response</span></span>

<span data-ttu-id="d7b0f-137">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体で[使用する](../resources/insights-used.md)項目の一覧です。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-137">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7b0f-138">例</span><span class="sxs-lookup"><span data-stu-id="d7b0f-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d7b0f-139">要求</span><span class="sxs-lookup"><span data-stu-id="d7b0f-139">Request</span></span>

<span data-ttu-id="d7b0f-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="d7b0f-141">応答</span><span class="sxs-lookup"><span data-stu-id="d7b0f-141">Response</span></span>

<span data-ttu-id="d7b0f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```

### <a name="expanding-resource"></a><span data-ttu-id="d7b0f-145">リソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-145">Expanding resource</span></span>
<span data-ttu-id="d7b0f-146">使用の洞察によって参照されるリソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="d7b0f-146">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
