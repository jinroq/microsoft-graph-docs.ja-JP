---
title: EducationSynchronizationProfile を削除する
description: 識別子に基づいて、テナント内の学校データ同期プロファイルを削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce0d895413a02d2a3ea4b7e84fd25ca8da7dc3e7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860086"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="321b2-103">EducationSynchronizationProfile を削除する</span><span class="sxs-lookup"><span data-stu-id="321b2-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="321b2-104">識別子に基づいて、テナント内の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="321b2-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="321b2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="321b2-105">Permissions</span></span>
<span data-ttu-id="321b2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="321b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="321b2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="321b2-108">Permission type</span></span> | <span data-ttu-id="321b2-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="321b2-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="321b2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="321b2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="321b2-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="321b2-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="321b2-112">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="321b2-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="321b2-113">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="321b2-113">Request headers</span></span>
| <span data-ttu-id="321b2-114">名前</span><span class="sxs-lookup"><span data-stu-id="321b2-114">Name</span></span>       | <span data-ttu-id="321b2-115">型</span><span class="sxs-lookup"><span data-stu-id="321b2-115">Type</span></span> | <span data-ttu-id="321b2-116">説明</span><span class="sxs-lookup"><span data-stu-id="321b2-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="321b2-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="321b2-117">Authorization</span></span>  | <span data-ttu-id="321b2-118">string</span><span class="sxs-lookup"><span data-stu-id="321b2-118">string</span></span>  | <span data-ttu-id="321b2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="321b2-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="321b2-121">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="321b2-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="321b2-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="321b2-122">Not supported.</span></span>|
|<span data-ttu-id="321b2-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="321b2-123">Application</span></span>|<span data-ttu-id="321b2-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="321b2-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="321b2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="321b2-125">Request body</span></span>
<span data-ttu-id="321b2-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="321b2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="321b2-127">応答</span><span class="sxs-lookup"><span data-stu-id="321b2-127">Response</span></span>
<span data-ttu-id="321b2-128">成功した場合、このメソッド`202 Accepted`は応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="321b2-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="321b2-129">例</span><span class="sxs-lookup"><span data-stu-id="321b2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="321b2-130">要求</span><span class="sxs-lookup"><span data-stu-id="321b2-130">Request</span></span>
<span data-ttu-id="321b2-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="321b2-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="321b2-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="321b2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="321b2-133">C#</span><span class="sxs-lookup"><span data-stu-id="321b2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="321b2-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="321b2-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="321b2-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="321b2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="321b2-136">Java</span><span class="sxs-lookup"><span data-stu-id="321b2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="321b2-137">応答</span><span class="sxs-lookup"><span data-stu-id="321b2-137">Response</span></span>
<span data-ttu-id="321b2-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="321b2-138">Here is an example of the response.</span></span>
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
