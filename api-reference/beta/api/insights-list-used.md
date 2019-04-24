---
title: 使用するリスト
description: ユーザーが使用するファイルの一覧を返す、計算された洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2341e41701a2b7306b9e0f1cb89a6b5df76b55ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32500854"
---
# <a name="list-used"></a><span data-ttu-id="d6454-103">使用するリスト</span><span class="sxs-lookup"><span data-stu-id="d6454-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6454-104">ユーザーが使用するファイルの一覧を返す、計算された洞察。</span><span class="sxs-lookup"><span data-stu-id="d6454-104">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6454-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6454-105">Permissions</span></span>
<span data-ttu-id="d6454-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6454-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6454-108">Permission type</span></span>      | <span data-ttu-id="d6454-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6454-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6454-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6454-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6454-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6454-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6454-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6454-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6454-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6454-113">Not supported.</span></span>    |
|<span data-ttu-id="d6454-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6454-114">Application</span></span> | <span data-ttu-id="d6454-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6454-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6454-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6454-116">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="d6454-117">他のユーザーの使用ドキュメントを要求すると、結果は ' lastModifiedDateTime ' で並べ替えられ、' lastAccessedDateTime ' は ' lastModifiedDateTime ' に設定されます。</span><span class="sxs-lookup"><span data-stu-id="d6454-117">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/{id | userPrincipalName}/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6454-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d6454-118">Optional query parameters</span></span>
<span data-ttu-id="d6454-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d6454-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d6454-120">クエリパラメーターを使用`$filter`して、使用されているアイテムをフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="d6454-120">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="d6454-121">たとえば、Type に基づいています。</span><span class="sxs-lookup"><span data-stu-id="d6454-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="d6454-122">またはコンテナーの種類に基づきます。</span><span class="sxs-lookup"><span data-stu-id="d6454-122">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="d6454-123">利用可能なコンテナーの種類と種類を表示します。これは、 [resourcevisualization](../resources/insights-resourcevisualization.md)でフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="d6454-123">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="d6454-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6454-124">Request headers</span></span>
| <span data-ttu-id="d6454-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6454-125">Header</span></span>       |  <span data-ttu-id="d6454-126">値</span><span class="sxs-lookup"><span data-stu-id="d6454-126">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="d6454-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6454-127">Authorization</span></span>  | <span data-ttu-id="d6454-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d6454-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d6454-130">承諾</span><span class="sxs-lookup"><span data-stu-id="d6454-130">Accept</span></span>  | <span data-ttu-id="d6454-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d6454-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6454-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6454-132">Request body</span></span>
<span data-ttu-id="d6454-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d6454-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6454-134">応答</span><span class="sxs-lookup"><span data-stu-id="d6454-134">Response</span></span>

<span data-ttu-id="d6454-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[使用され](../resources/insights-used.md)ている項目のリストを返します。</span><span class="sxs-lookup"><span data-stu-id="d6454-135">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6454-136">例</span><span class="sxs-lookup"><span data-stu-id="d6454-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d6454-137">要求</span><span class="sxs-lookup"><span data-stu-id="d6454-137">Request</span></span>

<span data-ttu-id="d6454-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6454-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="d6454-139">応答</span><span class="sxs-lookup"><span data-stu-id="d6454-139">Response</span></span>

<span data-ttu-id="d6454-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d6454-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

### <a name="expanding-resource"></a><span data-ttu-id="d6454-143">リソースの展開</span><span class="sxs-lookup"><span data-stu-id="d6454-143">Expanding resource</span></span>
<span data-ttu-id="d6454-144">使用されている洞察で参照されているリソースを展開できます。</span><span class="sxs-lookup"><span data-stu-id="d6454-144">The resource referenced by a used insight can be expanded.</span></span>
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
