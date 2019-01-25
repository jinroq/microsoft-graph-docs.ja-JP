---
title: 共有リスト
description: ユーザーと共有されているファイルの一覧を返す計算の把握。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2eef2a9b306984a8ad05bcf8fefca2458d609ab1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517352"
---
# <a name="list-shared"></a><span data-ttu-id="71090-103">共有リスト</span><span class="sxs-lookup"><span data-stu-id="71090-103">List shared</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71090-104">ユーザーと共有されているファイルの一覧を返す計算の把握。</span><span class="sxs-lookup"><span data-stu-id="71090-104">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="71090-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="71090-105">Permissions</span></span>
<span data-ttu-id="71090-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71090-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71090-108">Permission type</span></span>      | <span data-ttu-id="71090-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="71090-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71090-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71090-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71090-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71090-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="71090-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71090-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71090-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71090-113">Not supported.</span></span>    |
|<span data-ttu-id="71090-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71090-114">Application</span></span> | <span data-ttu-id="71090-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71090-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71090-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71090-116">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="71090-117">ユーザー id の要求または 'userPrincipalName' のだけがアクセスできるは、ユーザーが、他のユーザーではありません。</span><span class="sxs-lookup"><span data-stu-id="71090-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71090-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="71090-118">Optional query parameters</span></span>
<span data-ttu-id="71090-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="71090-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="71090-120">使用することができます、`$filter`の共有項目をフィルター処理するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="71090-120">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="71090-121">などは、型に基づいています。</span><span class="sxs-lookup"><span data-stu-id="71090-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="71090-122">使用可能なコンテナーの種類と[resourceVisualization](../resources/insights-resourcevisualization.md)内でフィルターの種類を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71090-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="71090-123">特定のユーザーによって共有されているファイルを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="71090-123">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="71090-124">指定することなどにより、`lastshared/sharedby/address`プロパティ。</span><span class="sxs-lookup"><span data-stu-id="71090-124">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="71090-125">[SharingDetail](../resources/insights-sharingdetail.md)複合型を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71090-125">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="71090-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71090-126">Request headers</span></span>
| <span data-ttu-id="71090-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71090-127">Header</span></span>       |  <span data-ttu-id="71090-128">値</span><span class="sxs-lookup"><span data-stu-id="71090-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="71090-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="71090-129">Authorization</span></span>  | <span data-ttu-id="71090-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="71090-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="71090-132">承諾</span><span class="sxs-lookup"><span data-stu-id="71090-132">Accept</span></span>  | <span data-ttu-id="71090-133">application/json</span><span class="sxs-lookup"><span data-stu-id="71090-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71090-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="71090-134">Request body</span></span>
<span data-ttu-id="71090-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="71090-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71090-136">応答</span><span class="sxs-lookup"><span data-stu-id="71090-136">Response</span></span>

<span data-ttu-id="71090-137">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[共有](../resources/insights-shared.md)の項目の一覧です。</span><span class="sxs-lookup"><span data-stu-id="71090-137">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71090-138">例</span><span class="sxs-lookup"><span data-stu-id="71090-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71090-139">要求</span><span class="sxs-lookup"><span data-stu-id="71090-139">Request</span></span>

<span data-ttu-id="71090-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71090-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="71090-141">応答</span><span class="sxs-lookup"><span data-stu-id="71090-141">Response</span></span>

<span data-ttu-id="71090-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71090-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="71090-145">リソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="71090-145">Expanding resource</span></span>
<span data-ttu-id="71090-146">共有洞察によって参照されるリソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="71090-146">The resource referenced by a shared insight can be expanded.</span></span>
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
