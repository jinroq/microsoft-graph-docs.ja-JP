---
title: EducationSynchronizationProfile 上で同期を一時停止する
description: テナント内の特定の学校データ同期プロファイルの同期を一時停止します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 79f184d0816fa3c9d3e5a9dd58737b8cf0ab657c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415996"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="585f8-103">EducationSynchronizationProfile 上で同期を一時停止する</span><span class="sxs-lookup"><span data-stu-id="585f8-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="585f8-104">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の同期を一時停止します。</span><span class="sxs-lookup"><span data-stu-id="585f8-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="585f8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="585f8-105">Permissions</span></span>
<span data-ttu-id="585f8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="585f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="585f8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="585f8-108">Permission type</span></span> | <span data-ttu-id="585f8-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="585f8-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="585f8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="585f8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="585f8-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="585f8-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="585f8-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="585f8-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="585f8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="585f8-113">Not supported.</span></span>|
|<span data-ttu-id="585f8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="585f8-114">Application</span></span>|<span data-ttu-id="585f8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="585f8-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="585f8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="585f8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="585f8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="585f8-117">Request headers</span></span>
| <span data-ttu-id="585f8-118">名前</span><span class="sxs-lookup"><span data-stu-id="585f8-118">Name</span></span>       | <span data-ttu-id="585f8-119">型</span><span class="sxs-lookup"><span data-stu-id="585f8-119">Type</span></span> | <span data-ttu-id="585f8-120">説明</span><span class="sxs-lookup"><span data-stu-id="585f8-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="585f8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="585f8-121">Authorization</span></span>  | <span data-ttu-id="585f8-122">string</span><span class="sxs-lookup"><span data-stu-id="585f8-122">string</span></span>  | <span data-ttu-id="585f8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="585f8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="585f8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="585f8-125">Request body</span></span>
<span data-ttu-id="585f8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="585f8-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="585f8-127">応答</span><span class="sxs-lookup"><span data-stu-id="585f8-127">Response</span></span>
<span data-ttu-id="585f8-128">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="585f8-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="585f8-129">例</span><span class="sxs-lookup"><span data-stu-id="585f8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="585f8-130">要求</span><span class="sxs-lookup"><span data-stu-id="585f8-130">Request</span></span>
<span data-ttu-id="585f8-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="585f8-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="585f8-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="585f8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="585f8-133">C#</span><span class="sxs-lookup"><span data-stu-id="585f8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="585f8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="585f8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="585f8-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="585f8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="585f8-136">応答</span><span class="sxs-lookup"><span data-stu-id="585f8-136">Response</span></span>

<span data-ttu-id="585f8-137">応答本文はありません。</span><span class="sxs-lookup"><span data-stu-id="585f8-137">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
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
