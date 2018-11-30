---
title: onenoteOperation を取得する
description: '長時間実行される OneNote 操作の状態を取得します。これは、応答で **Operation-Location** ヘッダーを返す操作に適用されます。たとえば、`CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection` です。   '
ms.openlocfilehash: abd11846cce1eab5e51ffc966d754a8a47f005bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072483"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="f5eb8-104">onenoteOperation を取得する</span><span class="sxs-lookup"><span data-stu-id="f5eb8-104">Get onenoteOperation</span></span>

> <span data-ttu-id="f5eb8-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5eb8-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5eb8-p103">長時間実行される OneNote 操作の状態を取得します。これは、応答で **Operation-Location** ヘッダーを返す操作に適用されます。たとえば、`CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection` です。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-p103">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="f5eb8-109">`status` プロパティが `completed` または `failed` を返すまで、Operation-Location エンドポイントをポーリングすることができます。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-109">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="f5eb8-110">状態が `completed` の場合、`resourceLocation` プロパティにはリソース エンドポイント URI が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-110">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="f5eb8-111">状態が `failed` の場合、エラーおよび `@api.diagnostics` プロパティからエラー情報が得られます。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-111">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5eb8-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f5eb8-112">Permissions</span></span>
<span data-ttu-id="f5eb8-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5eb8-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5eb8-115">Permission type</span></span>      | <span data-ttu-id="f5eb8-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5eb8-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5eb8-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5eb8-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f5eb8-118">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5eb8-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f5eb8-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5eb8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5eb8-120">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5eb8-120">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f5eb8-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5eb8-121">Application</span></span> | <span data-ttu-id="f5eb8-122">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5eb8-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5eb8-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5eb8-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5eb8-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f5eb8-124">Optional query parameters</span></span>
<span data-ttu-id="f5eb8-125">なし。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-125">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5eb8-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5eb8-126">Request headers</span></span>
| <span data-ttu-id="f5eb8-127">名前</span><span class="sxs-lookup"><span data-stu-id="f5eb8-127">Name</span></span>       | <span data-ttu-id="f5eb8-128">型</span><span class="sxs-lookup"><span data-stu-id="f5eb8-128">Type</span></span> | <span data-ttu-id="f5eb8-129">説明</span><span class="sxs-lookup"><span data-stu-id="f5eb8-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5eb8-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5eb8-130">Authorization</span></span>  | <span data-ttu-id="f5eb8-131">string</span><span class="sxs-lookup"><span data-stu-id="f5eb8-131">string</span></span>  | <span data-ttu-id="f5eb8-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5eb8-134">承諾</span><span class="sxs-lookup"><span data-stu-id="f5eb8-134">Accept</span></span> | <span data-ttu-id="f5eb8-135">string</span><span class="sxs-lookup"><span data-stu-id="f5eb8-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f5eb8-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5eb8-136">Request body</span></span>
<span data-ttu-id="f5eb8-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5eb8-138">応答</span><span class="sxs-lookup"><span data-stu-id="f5eb8-138">Response</span></span>

<span data-ttu-id="f5eb8-139">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [onenoteOperation](../resources/onenoteoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-139">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5eb8-140">例</span><span class="sxs-lookup"><span data-stu-id="f5eb8-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5eb8-141">要求</span><span class="sxs-lookup"><span data-stu-id="f5eb8-141">Request</span></span>
<span data-ttu-id="f5eb8-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="f5eb8-143">応答</span><span class="sxs-lookup"><span data-stu-id="f5eb8-143">Response</span></span>
<span data-ttu-id="f5eb8-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f5eb8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
