---
title: directReports を一覧表示する　
description: ユーザーの直属の部下を取得します。このユーザーがマネージャーとして割り当てられているユーザーと連絡先を返します。
localization_priority: Normal
ms.openlocfilehash: 9a5a76b98dfd47d9a0d1d4daceeb6a93c4dc5163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863435"
---
# <a name="list-directreports"></a><span data-ttu-id="372e2-104">directReports を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="372e2-104">List directReports</span></span>

> <span data-ttu-id="372e2-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="372e2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="372e2-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="372e2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="372e2-p103">ユーザーの直属の部下を取得します。このユーザーがマネージャーとして割り当てられているユーザーと連絡先を返します。</span><span class="sxs-lookup"><span data-stu-id="372e2-p103">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="372e2-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="372e2-109">Permissions</span></span>
<span data-ttu-id="372e2-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="372e2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="372e2-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="372e2-112">Permission type</span></span>      | <span data-ttu-id="372e2-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="372e2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="372e2-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="372e2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="372e2-115">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="372e2-115">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="372e2-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="372e2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="372e2-117">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="372e2-117">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="372e2-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="372e2-118">Application</span></span> | <span data-ttu-id="372e2-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="372e2-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="372e2-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="372e2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="372e2-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="372e2-121">Optional query parameters</span></span>
<span data-ttu-id="372e2-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="372e2-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="372e2-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="372e2-123">Request headers</span></span>
| <span data-ttu-id="372e2-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="372e2-124">Header</span></span>       | <span data-ttu-id="372e2-125">値</span><span class="sxs-lookup"><span data-stu-id="372e2-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="372e2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="372e2-126">Authorization</span></span>  | <span data-ttu-id="372e2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="372e2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="372e2-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="372e2-129">Content-Type</span></span>   | <span data-ttu-id="372e2-130">application/json</span><span class="sxs-lookup"><span data-stu-id="372e2-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="372e2-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="372e2-131">Request body</span></span>
<span data-ttu-id="372e2-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="372e2-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="372e2-133">応答</span><span class="sxs-lookup"><span data-stu-id="372e2-133">Response</span></span>

<span data-ttu-id="372e2-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="372e2-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="372e2-135">例</span><span class="sxs-lookup"><span data-stu-id="372e2-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="372e2-136">要求</span><span class="sxs-lookup"><span data-stu-id="372e2-136">Request</span></span>
<span data-ttu-id="372e2-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="372e2-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
##### <a name="response"></a><span data-ttu-id="372e2-138">応答</span><span class="sxs-lookup"><span data-stu-id="372e2-138">Response</span></span>
<span data-ttu-id="372e2-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="372e2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
