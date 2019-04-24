---
title: 共有リスト
description: ユーザーと共有されるファイルの一覧を返す、計算された洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 009d9f65b5403139235e5f9afa932ebbe54ff9d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32500386"
---
# <a name="list-shared"></a><span data-ttu-id="c9345-103">共有リスト</span><span class="sxs-lookup"><span data-stu-id="c9345-103">List shared</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9345-104">ユーザーと共有されるファイルの一覧を返す、計算された洞察。</span><span class="sxs-lookup"><span data-stu-id="c9345-104">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9345-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c9345-105">Permissions</span></span>
<span data-ttu-id="c9345-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9345-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9345-108">Permission type</span></span>      | <span data-ttu-id="c9345-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9345-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9345-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9345-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c9345-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9345-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9345-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9345-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9345-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9345-113">Not supported.</span></span>    |
|<span data-ttu-id="c9345-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9345-114">Application</span></span> | <span data-ttu-id="c9345-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9345-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9345-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9345-116">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="c9345-117">' user id ' または ' userPrincipalName ' を持つ要求は、ユーザーのみがアクセスでき、他のユーザーはアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="c9345-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/{id | userPrincipalName}/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9345-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c9345-118">Optional query parameters</span></span>
<span data-ttu-id="c9345-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c9345-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c9345-120">クエリパラメーターを使用`$filter`して、共有アイテムをフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="c9345-120">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="c9345-121">たとえば、Type に基づいています。</span><span class="sxs-lookup"><span data-stu-id="c9345-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="c9345-122">利用可能なコンテナーの種類と種類を表示します。これは、 [resourcevisualization](../resources/insights-resourcevisualization.md)でフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="c9345-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="c9345-123">特定のユーザーによって共有されているファイルを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="c9345-123">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="c9345-124">たとえば、次のように`lastshared/sharedby/address`プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="c9345-124">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="c9345-125">[sharingdetail](../resources/insights-sharingdetail.md)複合型を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9345-125">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="c9345-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9345-126">Request headers</span></span>
| <span data-ttu-id="c9345-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9345-127">Header</span></span>       |  <span data-ttu-id="c9345-128">値</span><span class="sxs-lookup"><span data-stu-id="c9345-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="c9345-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9345-129">Authorization</span></span>  | <span data-ttu-id="c9345-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c9345-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c9345-132">承諾</span><span class="sxs-lookup"><span data-stu-id="c9345-132">Accept</span></span>  | <span data-ttu-id="c9345-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c9345-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9345-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9345-134">Request body</span></span>
<span data-ttu-id="c9345-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c9345-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9345-136">応答</span><span class="sxs-lookup"><span data-stu-id="c9345-136">Response</span></span>

<span data-ttu-id="c9345-137">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[共有](../resources/insights-shared.md)アイテムのリストを返します。</span><span class="sxs-lookup"><span data-stu-id="c9345-137">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9345-138">例</span><span class="sxs-lookup"><span data-stu-id="c9345-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c9345-139">要求</span><span class="sxs-lookup"><span data-stu-id="c9345-139">Request</span></span>

<span data-ttu-id="c9345-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c9345-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="c9345-141">応答</span><span class="sxs-lookup"><span data-stu-id="c9345-141">Response</span></span>

<span data-ttu-id="c9345-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c9345-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastShared" : { 
                "sharedDateTime" : "sharedDateTime-value",  
                "sharingSubject" : "sharingSubject-value",
                "sharingType" : "sharingType-value", 
                "sharedBy" : { 
                    "displayName" : "displayName-value", 
                    "id": "id-value" 
                }
                "sharingReference" : { 
                    "webUrl" : "webUrl-value",
                    "type: "type-value", 
                    "id": "id-value"
                } 
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
```

### <a name="expanding-resource"></a><span data-ttu-id="c9345-145">リソースの展開</span><span class="sxs-lookup"><span data-stu-id="c9345-145">Expanding resource</span></span>
<span data-ttu-id="c9345-146">共有された洞察で参照されているリソースは展開できます。</span><span class="sxs-lookup"><span data-stu-id="c9345-146">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
