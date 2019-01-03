---
title: 共有リスト
description: ユーザーと共有されているファイルの一覧を返す計算の把握。
author: simonhult
ms.openlocfilehash: 5d8c4632f2ccb48cc83c3467ddfe0c973f390947
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345816"
---
# <a name="list-shared"></a><span data-ttu-id="27e14-103">共有リスト</span><span class="sxs-lookup"><span data-stu-id="27e14-103">List shared</span></span>

> <span data-ttu-id="27e14-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27e14-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27e14-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27e14-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27e14-106">ユーザーと共有されているファイルの一覧を返す計算の把握。</span><span class="sxs-lookup"><span data-stu-id="27e14-106">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="27e14-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="27e14-107">Permissions</span></span>
<span data-ttu-id="27e14-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27e14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27e14-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27e14-110">Permission type</span></span>      | <span data-ttu-id="27e14-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="27e14-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27e14-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27e14-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27e14-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27e14-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="27e14-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27e14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27e14-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27e14-115">Not supported.</span></span>    |
|<span data-ttu-id="27e14-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27e14-116">Application</span></span> | <span data-ttu-id="27e14-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27e14-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27e14-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27e14-118">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="27e14-119">ユーザー id の要求または 'userPrincipalName' のだけがアクセスできるは、ユーザーが、他のユーザーではありません。</span><span class="sxs-lookup"><span data-stu-id="27e14-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27e14-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="27e14-120">Optional query parameters</span></span>
<span data-ttu-id="27e14-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="27e14-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="27e14-122">使用することができます、`$filter`の共有項目をフィルター処理するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="27e14-122">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="27e14-123">などは、型に基づいています。</span><span class="sxs-lookup"><span data-stu-id="27e14-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="27e14-124">使用可能なコンテナーの種類と[resourceVisualization](../resources/insights-resourcevisualization.md)内でフィルターの種類を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27e14-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="27e14-125">特定のユーザーによって共有されているファイルを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="27e14-125">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="27e14-126">指定することなどにより、`lastshared/sharedby/address`プロパティ。</span><span class="sxs-lookup"><span data-stu-id="27e14-126">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="27e14-127">[SharingDetail](../resources/insights-sharingdetail.md)複合型を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27e14-127">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="27e14-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27e14-128">Request headers</span></span>
| <span data-ttu-id="27e14-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27e14-129">Header</span></span>       |  <span data-ttu-id="27e14-130">値</span><span class="sxs-lookup"><span data-stu-id="27e14-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="27e14-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="27e14-131">Authorization</span></span>  | <span data-ttu-id="27e14-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="27e14-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="27e14-134">承諾</span><span class="sxs-lookup"><span data-stu-id="27e14-134">Accept</span></span>  | <span data-ttu-id="27e14-135">application/json</span><span class="sxs-lookup"><span data-stu-id="27e14-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27e14-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="27e14-136">Request body</span></span>
<span data-ttu-id="27e14-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="27e14-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27e14-138">応答</span><span class="sxs-lookup"><span data-stu-id="27e14-138">Response</span></span>

<span data-ttu-id="27e14-139">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[共有](../resources/insights-shared.md)の項目の一覧です。</span><span class="sxs-lookup"><span data-stu-id="27e14-139">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27e14-140">例</span><span class="sxs-lookup"><span data-stu-id="27e14-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="27e14-141">要求</span><span class="sxs-lookup"><span data-stu-id="27e14-141">Request</span></span>

<span data-ttu-id="27e14-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27e14-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="27e14-143">応答</span><span class="sxs-lookup"><span data-stu-id="27e14-143">Response</span></span>

<span data-ttu-id="27e14-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27e14-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="27e14-147">リソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="27e14-147">Expanding resource</span></span>
<span data-ttu-id="27e14-148">共有洞察によって参照されるリソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="27e14-148">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```