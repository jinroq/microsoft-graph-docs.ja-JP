---
title: リストの使用
description: ユーザーに使用されるファイルの一覧を返す計算の把握。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: e73536d5933d6293539eb00ba8cdc2e85ce5fa93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526103"
---
# <a name="list-used"></a><span data-ttu-id="0a538-103">リストの使用</span><span class="sxs-lookup"><span data-stu-id="0a538-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a538-104">ユーザーに使用されるファイルの一覧を返す計算の把握。</span><span class="sxs-lookup"><span data-stu-id="0a538-104">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a538-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a538-105">Permissions</span></span>
<span data-ttu-id="0a538-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a538-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a538-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a538-108">Permission type</span></span>      | <span data-ttu-id="0a538-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a538-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a538-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a538-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0a538-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a538-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a538-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a538-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a538-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a538-113">Not supported.</span></span>    |
|<span data-ttu-id="0a538-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a538-114">Application</span></span> | <span data-ttu-id="0a538-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a538-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a538-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a538-116">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="0a538-117">'LastModifiedDateTime' で並べ替えられた結果が返されます他のユーザーのドキュメントの使用を要求して、'lastAccessedDateTime' は、'lastModifiedDateTime' に設定されています。</span><span class="sxs-lookup"><span data-stu-id="0a538-117">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a538-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0a538-118">Optional query parameters</span></span>
<span data-ttu-id="0a538-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0a538-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="0a538-120">使用することができます、`$filter`アイテムのフィルターを使用するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="0a538-120">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="0a538-121">などは、型に基づいています。</span><span class="sxs-lookup"><span data-stu-id="0a538-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="0a538-122">コンテナーの種類に基づくか。</span><span class="sxs-lookup"><span data-stu-id="0a538-122">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="0a538-123">使用可能なコンテナーの種類と[resourceVisualization](../resources/insights-resourcevisualization.md)内でフィルターの種類を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a538-123">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="0a538-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a538-124">Request headers</span></span>
| <span data-ttu-id="0a538-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a538-125">Header</span></span>       |  <span data-ttu-id="0a538-126">値</span><span class="sxs-lookup"><span data-stu-id="0a538-126">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="0a538-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a538-127">Authorization</span></span>  | <span data-ttu-id="0a538-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a538-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="0a538-130">承諾</span><span class="sxs-lookup"><span data-stu-id="0a538-130">Accept</span></span>  | <span data-ttu-id="0a538-131">application/json</span><span class="sxs-lookup"><span data-stu-id="0a538-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a538-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a538-132">Request body</span></span>
<span data-ttu-id="0a538-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a538-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a538-134">応答</span><span class="sxs-lookup"><span data-stu-id="0a538-134">Response</span></span>

<span data-ttu-id="0a538-135">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体で[使用する](../resources/insights-used.md)項目の一覧です。</span><span class="sxs-lookup"><span data-stu-id="0a538-135">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a538-136">例</span><span class="sxs-lookup"><span data-stu-id="0a538-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0a538-137">要求</span><span class="sxs-lookup"><span data-stu-id="0a538-137">Request</span></span>

<span data-ttu-id="0a538-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a538-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="0a538-139">応答</span><span class="sxs-lookup"><span data-stu-id="0a538-139">Response</span></span>

<span data-ttu-id="0a538-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a538-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

### <a name="expanding-resource"></a><span data-ttu-id="0a538-143">リソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="0a538-143">Expanding resource</span></span>
<span data-ttu-id="0a538-144">使用の洞察によって参照されるリソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="0a538-144">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
