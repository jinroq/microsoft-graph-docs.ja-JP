---
title: EducationSynchronizationProfile を削除する
description: 識別子に基づいて、テナント内の学校データ同期プロファイルを削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5f786bf9c36b09aae4a26d3de317d09d1376fb35
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587040"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="397d6-103">EducationSynchronizationProfile を削除する</span><span class="sxs-lookup"><span data-stu-id="397d6-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="397d6-104">識別子に基づいて、テナント内の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="397d6-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="397d6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="397d6-105">Permissions</span></span>
<span data-ttu-id="397d6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="397d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="397d6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="397d6-108">Permission type</span></span> | <span data-ttu-id="397d6-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="397d6-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="397d6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="397d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="397d6-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="397d6-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="397d6-112">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="397d6-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="397d6-113">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="397d6-113">Request headers</span></span>
| <span data-ttu-id="397d6-114">名前</span><span class="sxs-lookup"><span data-stu-id="397d6-114">Name</span></span>       | <span data-ttu-id="397d6-115">型</span><span class="sxs-lookup"><span data-stu-id="397d6-115">Type</span></span> | <span data-ttu-id="397d6-116">説明</span><span class="sxs-lookup"><span data-stu-id="397d6-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="397d6-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="397d6-117">Authorization</span></span>  | <span data-ttu-id="397d6-118">string</span><span class="sxs-lookup"><span data-stu-id="397d6-118">string</span></span>  | <span data-ttu-id="397d6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="397d6-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="397d6-121">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="397d6-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="397d6-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="397d6-122">Not supported.</span></span>|
|<span data-ttu-id="397d6-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="397d6-123">Application</span></span>|<span data-ttu-id="397d6-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="397d6-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="397d6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="397d6-125">Request body</span></span>
<span data-ttu-id="397d6-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="397d6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="397d6-127">応答</span><span class="sxs-lookup"><span data-stu-id="397d6-127">Response</span></span>
<span data-ttu-id="397d6-128">成功した場合、このメソッド`202 Accepted`は応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="397d6-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="397d6-129">例</span><span class="sxs-lookup"><span data-stu-id="397d6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="397d6-130">要求</span><span class="sxs-lookup"><span data-stu-id="397d6-130">Request</span></span>
<span data-ttu-id="397d6-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="397d6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="397d6-132">応答</span><span class="sxs-lookup"><span data-stu-id="397d6-132">Response</span></span>
<span data-ttu-id="397d6-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="397d6-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="397d6-134">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="397d6-134">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="397d6-135">Visual</span><span class="sxs-lookup"><span data-stu-id="397d6-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationProfile-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
