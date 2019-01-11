---
title: onenoteOperation を取得する
description: '長時間実行される OneNote 操作の状態を取得します。これは、応答で **Operation-Location** ヘッダーを返す操作に適用されます。たとえば、`CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection` です。   '
localization_priority: Normal
ms.openlocfilehash: b62f83266560f217d9569c6ee7ca39dd53198bb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824767"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="f89ae-104">onenoteOperation を取得する</span><span class="sxs-lookup"><span data-stu-id="f89ae-104">Get onenoteOperation</span></span>

> <span data-ttu-id="f89ae-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f89ae-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f89ae-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f89ae-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f89ae-p103">長時間実行される OneNote 操作の状態を取得します。これは、応答で **Operation-Location** ヘッダーを返す操作に適用されます。たとえば、`CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection` です。</span><span class="sxs-lookup"><span data-stu-id="f89ae-p103">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="f89ae-109">`status` プロパティが `completed` または `failed` を返すまで、Operation-Location エンドポイントをポーリングすることができます。</span><span class="sxs-lookup"><span data-stu-id="f89ae-109">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="f89ae-110">状態が `completed` の場合、`resourceLocation` プロパティにはリソース エンドポイント URI が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f89ae-110">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="f89ae-111">状態が `failed` の場合、エラーおよび `@api.diagnostics` プロパティからエラー情報が得られます。</span><span class="sxs-lookup"><span data-stu-id="f89ae-111">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="f89ae-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f89ae-112">Permissions</span></span>
<span data-ttu-id="f89ae-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f89ae-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f89ae-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f89ae-115">Permission type</span></span>      | <span data-ttu-id="f89ae-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f89ae-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f89ae-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f89ae-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f89ae-118">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f89ae-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f89ae-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f89ae-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f89ae-120">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f89ae-120">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f89ae-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f89ae-121">Application</span></span> | <span data-ttu-id="f89ae-122">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f89ae-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f89ae-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f89ae-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f89ae-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f89ae-124">Optional query parameters</span></span>
<span data-ttu-id="f89ae-125">なし。</span><span class="sxs-lookup"><span data-stu-id="f89ae-125">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f89ae-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f89ae-126">Request headers</span></span>
| <span data-ttu-id="f89ae-127">名前</span><span class="sxs-lookup"><span data-stu-id="f89ae-127">Name</span></span>       | <span data-ttu-id="f89ae-128">種類</span><span class="sxs-lookup"><span data-stu-id="f89ae-128">Type</span></span> | <span data-ttu-id="f89ae-129">説明</span><span class="sxs-lookup"><span data-stu-id="f89ae-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f89ae-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f89ae-130">Authorization</span></span>  | <span data-ttu-id="f89ae-131">string</span><span class="sxs-lookup"><span data-stu-id="f89ae-131">string</span></span>  | <span data-ttu-id="f89ae-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f89ae-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f89ae-134">承諾</span><span class="sxs-lookup"><span data-stu-id="f89ae-134">Accept</span></span> | <span data-ttu-id="f89ae-135">string</span><span class="sxs-lookup"><span data-stu-id="f89ae-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f89ae-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="f89ae-136">Request body</span></span>
<span data-ttu-id="f89ae-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f89ae-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f89ae-138">応答</span><span class="sxs-lookup"><span data-stu-id="f89ae-138">Response</span></span>

<span data-ttu-id="f89ae-139">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [onenoteOperation](../resources/onenoteoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f89ae-139">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f89ae-140">例</span><span class="sxs-lookup"><span data-stu-id="f89ae-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f89ae-141">要求</span><span class="sxs-lookup"><span data-stu-id="f89ae-141">Request</span></span>
<span data-ttu-id="f89ae-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f89ae-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="f89ae-143">応答</span><span class="sxs-lookup"><span data-stu-id="f89ae-143">Response</span></span>
<span data-ttu-id="f89ae-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f89ae-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
