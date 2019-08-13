---
title: OnenoteOperation を取得する
description: '長時間実行している OneNote 操作の状態を取得します。 これ`CopyNotebook`は`CopyToNotebook` `CopyToSectionGroup`、、、、などの応答の**操作場所**ヘッダーを返す操作に適用され`and CopyToSection`ます。   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 57e01f2002600272be2666a4259c659872c0a60f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346724"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="180a0-104">OnenoteOperation を取得する</span><span class="sxs-lookup"><span data-stu-id="180a0-104">Get onenoteOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="180a0-105">長時間実行している OneNote 操作の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="180a0-105">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="180a0-106">これ`CopyNotebook`は`CopyToNotebook` `CopyToSectionGroup`、、、、などの応答の**操作場所**ヘッダーを返す操作に適用され`and CopyToSection`ます。</span><span class="sxs-lookup"><span data-stu-id="180a0-106">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="180a0-107">プロパティが`status`または`completed` `failed`を返すまで、操作場所エンドポイントをポーリングできます。</span><span class="sxs-lookup"><span data-stu-id="180a0-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="180a0-108">状態が`completed`の場合、プロパティ`resourceLocation`にはリソースエンドポイント URI が含まれます。</span><span class="sxs-lookup"><span data-stu-id="180a0-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="180a0-109">状態がの場合`failed`、エラーおよび`@api.diagnostics`プロパティからエラー情報が得られます。</span><span class="sxs-lookup"><span data-stu-id="180a0-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="180a0-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="180a0-110">Permissions</span></span>
<span data-ttu-id="180a0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="180a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="180a0-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="180a0-113">Permission type</span></span>      | <span data-ttu-id="180a0-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="180a0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="180a0-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="180a0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="180a0-116">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="180a0-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="180a0-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="180a0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="180a0-118">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="180a0-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="180a0-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="180a0-119">Application</span></span> | <span data-ttu-id="180a0-120">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="180a0-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="180a0-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="180a0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="180a0-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="180a0-122">Optional query parameters</span></span>
<span data-ttu-id="180a0-123">なし。</span><span class="sxs-lookup"><span data-stu-id="180a0-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="180a0-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="180a0-124">Request headers</span></span>
| <span data-ttu-id="180a0-125">名前</span><span class="sxs-lookup"><span data-stu-id="180a0-125">Name</span></span>       | <span data-ttu-id="180a0-126">型</span><span class="sxs-lookup"><span data-stu-id="180a0-126">Type</span></span> | <span data-ttu-id="180a0-127">説明</span><span class="sxs-lookup"><span data-stu-id="180a0-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="180a0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="180a0-128">Authorization</span></span>  | <span data-ttu-id="180a0-129">string</span><span class="sxs-lookup"><span data-stu-id="180a0-129">string</span></span>  | <span data-ttu-id="180a0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="180a0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="180a0-132">承諾</span><span class="sxs-lookup"><span data-stu-id="180a0-132">Accept</span></span> | <span data-ttu-id="180a0-133">string</span><span class="sxs-lookup"><span data-stu-id="180a0-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="180a0-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="180a0-134">Request body</span></span>
<span data-ttu-id="180a0-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="180a0-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="180a0-136">応答</span><span class="sxs-lookup"><span data-stu-id="180a0-136">Response</span></span>

<span data-ttu-id="180a0-137">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onenoteOperation](../resources/onenoteoperation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="180a0-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="180a0-138">例</span><span class="sxs-lookup"><span data-stu-id="180a0-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="180a0-139">要求</span><span class="sxs-lookup"><span data-stu-id="180a0-139">Request</span></span>
<span data-ttu-id="180a0-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="180a0-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="180a0-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="180a0-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="180a0-142">C#</span><span class="sxs-lookup"><span data-stu-id="180a0-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="180a0-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="180a0-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="180a0-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="180a0-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="180a0-145">Java</span><span class="sxs-lookup"><span data-stu-id="180a0-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onenoteoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="180a0-146">応答</span><span class="sxs-lookup"><span data-stu-id="180a0-146">Response</span></span>
<span data-ttu-id="180a0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="180a0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
