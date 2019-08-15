---
title: EducationSynchronizationProfile での同期の再開
description: テナント内の特定の学校データ同期プロファイルの同期を再開します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 538f4fd48f4a692ab0be2f9e22e49607116d2a1f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415968"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="cf36a-103">EducationSynchronizationProfile での同期の再開</span><span class="sxs-lookup"><span data-stu-id="cf36a-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf36a-104">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="cf36a-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf36a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cf36a-105">Permissions</span></span>
<span data-ttu-id="cf36a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf36a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf36a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf36a-108">Permission type</span></span> | <span data-ttu-id="cf36a-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cf36a-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="cf36a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf36a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf36a-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf36a-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="cf36a-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="cf36a-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cf36a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf36a-113">Not supported.</span></span>|
|<span data-ttu-id="cf36a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf36a-114">Application</span></span>|<span data-ttu-id="cf36a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf36a-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf36a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf36a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="cf36a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf36a-117">Request headers</span></span>
| <span data-ttu-id="cf36a-118">名前</span><span class="sxs-lookup"><span data-stu-id="cf36a-118">Name</span></span>       | <span data-ttu-id="cf36a-119">型</span><span class="sxs-lookup"><span data-stu-id="cf36a-119">Type</span></span> | <span data-ttu-id="cf36a-120">説明</span><span class="sxs-lookup"><span data-stu-id="cf36a-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cf36a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf36a-121">Authorization</span></span>  | <span data-ttu-id="cf36a-122">string</span><span class="sxs-lookup"><span data-stu-id="cf36a-122">string</span></span>  | <span data-ttu-id="cf36a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cf36a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf36a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf36a-125">Request body</span></span>
<span data-ttu-id="cf36a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cf36a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cf36a-127">応答</span><span class="sxs-lookup"><span data-stu-id="cf36a-127">Response</span></span>
<span data-ttu-id="cf36a-128">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="cf36a-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cf36a-129">例</span><span class="sxs-lookup"><span data-stu-id="cf36a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf36a-130">要求</span><span class="sxs-lookup"><span data-stu-id="cf36a-130">Request</span></span>
<span data-ttu-id="cf36a-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf36a-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cf36a-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cf36a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cf36a-133">C#</span><span class="sxs-lookup"><span data-stu-id="cf36a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-resume-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf36a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf36a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-resume-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cf36a-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="cf36a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-resume-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cf36a-136">応答</span><span class="sxs-lookup"><span data-stu-id="cf36a-136">Response</span></span>

<span data-ttu-id="cf36a-137">応答本文はありません。</span><span class="sxs-lookup"><span data-stu-id="cf36a-137">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
HTTP/1.1 200 OK
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
