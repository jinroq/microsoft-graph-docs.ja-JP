---
title: EducationSynchronizationProfile を削除する
description: 識別子に基づいて、テナント内の学校データ同期プロファイルを削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a2230d8bc88bfdba6f014c9b78cbdc7f519f075d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416017"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="8bf8f-103">EducationSynchronizationProfile を削除する</span><span class="sxs-lookup"><span data-stu-id="8bf8f-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bf8f-104">識別子に基づいて、テナント内の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bf8f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8bf8f-105">Permissions</span></span>
<span data-ttu-id="8bf8f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bf8f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bf8f-108">Permission type</span></span> | <span data-ttu-id="8bf8f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8bf8f-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="8bf8f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bf8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bf8f-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bf8f-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bf8f-112">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bf8f-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8bf8f-113">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bf8f-113">Request headers</span></span>
| <span data-ttu-id="8bf8f-114">名前</span><span class="sxs-lookup"><span data-stu-id="8bf8f-114">Name</span></span>       | <span data-ttu-id="8bf8f-115">型</span><span class="sxs-lookup"><span data-stu-id="8bf8f-115">Type</span></span> | <span data-ttu-id="8bf8f-116">説明</span><span class="sxs-lookup"><span data-stu-id="8bf8f-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8bf8f-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bf8f-117">Authorization</span></span>  | <span data-ttu-id="8bf8f-118">string</span><span class="sxs-lookup"><span data-stu-id="8bf8f-118">string</span></span>  | <span data-ttu-id="8bf8f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="8bf8f-121">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="8bf8f-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="8bf8f-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-122">Not supported.</span></span>|
|<span data-ttu-id="8bf8f-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bf8f-123">Application</span></span>|<span data-ttu-id="8bf8f-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bf8f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8bf8f-125">Request body</span></span>
<span data-ttu-id="8bf8f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8bf8f-127">応答</span><span class="sxs-lookup"><span data-stu-id="8bf8f-127">Response</span></span>
<span data-ttu-id="8bf8f-128">成功した場合、このメソッド`202 Accepted`は応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bf8f-129">例</span><span class="sxs-lookup"><span data-stu-id="8bf8f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bf8f-130">要求</span><span class="sxs-lookup"><span data-stu-id="8bf8f-130">Request</span></span>
<span data-ttu-id="8bf8f-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8bf8f-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8bf8f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8bf8f-133">C#</span><span class="sxs-lookup"><span data-stu-id="8bf8f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bf8f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bf8f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bf8f-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="8bf8f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8bf8f-136">応答</span><span class="sxs-lookup"><span data-stu-id="8bf8f-136">Response</span></span>
<span data-ttu-id="8bf8f-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
