---
title: EducationSynchronizationProfile での同期の再開
description: テナント内の特定の学校データ同期プロファイルの同期を再開します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b4abb054763416e65f99da14aaa1e2ea1db1eb15
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587458"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="1bdd2-103">EducationSynchronizationProfile での同期の再開</span><span class="sxs-lookup"><span data-stu-id="1bdd2-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bdd2-104">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="1bdd2-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bdd2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1bdd2-105">Permissions</span></span>
<span data-ttu-id="1bdd2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bdd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1bdd2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1bdd2-108">Permission type</span></span> | <span data-ttu-id="1bdd2-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1bdd2-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="1bdd2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1bdd2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1bdd2-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bdd2-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="1bdd2-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="1bdd2-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1bdd2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bdd2-113">Not supported.</span></span>|
|<span data-ttu-id="1bdd2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1bdd2-114">Application</span></span>|<span data-ttu-id="1bdd2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bdd2-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bdd2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1bdd2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="1bdd2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1bdd2-117">Request headers</span></span>
| <span data-ttu-id="1bdd2-118">名前</span><span class="sxs-lookup"><span data-stu-id="1bdd2-118">Name</span></span>       | <span data-ttu-id="1bdd2-119">型</span><span class="sxs-lookup"><span data-stu-id="1bdd2-119">Type</span></span> | <span data-ttu-id="1bdd2-120">説明</span><span class="sxs-lookup"><span data-stu-id="1bdd2-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1bdd2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bdd2-121">Authorization</span></span>  | <span data-ttu-id="1bdd2-122">string</span><span class="sxs-lookup"><span data-stu-id="1bdd2-122">string</span></span>  | <span data-ttu-id="1bdd2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1bdd2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bdd2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1bdd2-125">Request body</span></span>
<span data-ttu-id="1bdd2-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1bdd2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1bdd2-127">応答</span><span class="sxs-lookup"><span data-stu-id="1bdd2-127">Response</span></span>
<span data-ttu-id="1bdd2-128">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1bdd2-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1bdd2-129">例</span><span class="sxs-lookup"><span data-stu-id="1bdd2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bdd2-130">要求</span><span class="sxs-lookup"><span data-stu-id="1bdd2-130">Request</span></span>
<span data-ttu-id="1bdd2-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1bdd2-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="1bdd2-132">応答</span><span class="sxs-lookup"><span data-stu-id="1bdd2-132">Response</span></span>

<span data-ttu-id="1bdd2-133">応答本文はありません。</span><span class="sxs-lookup"><span data-stu-id="1bdd2-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1bdd2-134">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1bdd2-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1bdd2-135">Visual</span><span class="sxs-lookup"><span data-stu-id="1bdd2-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bdd2-136">Java</span><span class="sxs-lookup"><span data-stu-id="1bdd2-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
