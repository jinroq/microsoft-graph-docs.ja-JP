---
title: onenoteOperation を取得する
description: '長時間実行される OneNote 操作の状態を取得します。これは、応答で **Operation-Location** ヘッダーを返す操作に適用されます。たとえば、`CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection` です。   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: c869702b856f03bccbbc5101e8e72facd3287738
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932386"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="3b1b0-104">onenoteOperation を取得する</span><span class="sxs-lookup"><span data-stu-id="3b1b0-104">Get onenoteOperation</span></span>

<span data-ttu-id="3b1b0-p102">長時間実行される OneNote 操作の状態を取得します。これは、応答で **Operation-Location** ヘッダーを返す操作に適用されます。たとえば、`CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection` です。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-p102">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="3b1b0-107">`status` プロパティが `completed` または `failed` を返すまで、Operation-Location エンドポイントをポーリングすることができます。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="3b1b0-108">状態が `completed` の場合、`resourceLocation` プロパティにはリソース エンドポイント URI が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="3b1b0-109">状態が `failed` の場合、エラーおよび `@api.diagnostics` プロパティからエラー情報が得られます。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b1b0-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b1b0-110">Permissions</span></span>
<span data-ttu-id="3b1b0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b1b0-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b1b0-113">Permission type</span></span>      | <span data-ttu-id="3b1b0-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b1b0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b1b0-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b1b0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3b1b0-116">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b1b0-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b1b0-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b1b0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b1b0-118">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b1b0-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3b1b0-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b1b0-119">Application</span></span> | <span data-ttu-id="3b1b0-120">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b1b0-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b1b0-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b1b0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b1b0-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3b1b0-122">Optional query parameters</span></span>
<span data-ttu-id="3b1b0-123">なし。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b1b0-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b1b0-124">Request headers</span></span>
| <span data-ttu-id="3b1b0-125">名前</span><span class="sxs-lookup"><span data-stu-id="3b1b0-125">Name</span></span>       | <span data-ttu-id="3b1b0-126">型</span><span class="sxs-lookup"><span data-stu-id="3b1b0-126">Type</span></span> | <span data-ttu-id="3b1b0-127">説明</span><span class="sxs-lookup"><span data-stu-id="3b1b0-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3b1b0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b1b0-128">Authorization</span></span>  | <span data-ttu-id="3b1b0-129">string</span><span class="sxs-lookup"><span data-stu-id="3b1b0-129">string</span></span>  | <span data-ttu-id="3b1b0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b1b0-132">承諾</span><span class="sxs-lookup"><span data-stu-id="3b1b0-132">Accept</span></span> | <span data-ttu-id="3b1b0-133">string</span><span class="sxs-lookup"><span data-stu-id="3b1b0-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3b1b0-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b1b0-134">Request body</span></span>
<span data-ttu-id="3b1b0-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b1b0-136">応答</span><span class="sxs-lookup"><span data-stu-id="3b1b0-136">Response</span></span>

<span data-ttu-id="3b1b0-137">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [onenoteOperation](../resources/onenoteoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b1b0-138">例</span><span class="sxs-lookup"><span data-stu-id="3b1b0-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b1b0-139">要求</span><span class="sxs-lookup"><span data-stu-id="3b1b0-139">Request</span></span>
<span data-ttu-id="3b1b0-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="3b1b0-141">応答</span><span class="sxs-lookup"><span data-stu-id="3b1b0-141">Response</span></span>
<span data-ttu-id="3b1b0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b1b0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
