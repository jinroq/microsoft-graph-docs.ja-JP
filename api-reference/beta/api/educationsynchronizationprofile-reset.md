---
title: EducationSynchronizationProfile の同期をリセットする
description: テナント内の特定の学校データ同期プロファイルの同期をリセットします。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d1bae89181f496bac3fc89b50b76e6f57f1fb8a1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587102"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="a5aa3-103">EducationSynchronizationProfile の同期をリセットする</span><span class="sxs-lookup"><span data-stu-id="a5aa3-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5aa3-104">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="a5aa3-105">**注:** この操作を行うと、同期が再開されます。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="a5aa3-106">発生したエラーは削除されます。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="a5aa3-107">Azure Active Directory (Azure AD) からデータが削除されることはありません。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a5aa3-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5aa3-108">Permissions</span></span>
<span data-ttu-id="a5aa3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5aa3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5aa3-111">Permission type</span></span> | <span data-ttu-id="a5aa3-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5aa3-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="a5aa3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5aa3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a5aa3-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5aa3-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="a5aa3-115">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="a5aa3-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a5aa3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-116">Not supported.</span></span>|
|<span data-ttu-id="a5aa3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5aa3-117">Application</span></span>|<span data-ttu-id="a5aa3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5aa3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5aa3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="a5aa3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5aa3-120">Request headers</span></span>
| <span data-ttu-id="a5aa3-121">名前</span><span class="sxs-lookup"><span data-stu-id="a5aa3-121">Name</span></span>       | <span data-ttu-id="a5aa3-122">型</span><span class="sxs-lookup"><span data-stu-id="a5aa3-122">Type</span></span> | <span data-ttu-id="a5aa3-123">説明</span><span class="sxs-lookup"><span data-stu-id="a5aa3-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5aa3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5aa3-124">Authorization</span></span>  | <span data-ttu-id="a5aa3-125">string</span><span class="sxs-lookup"><span data-stu-id="a5aa3-125">string</span></span>  | <span data-ttu-id="a5aa3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5aa3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5aa3-128">Request body</span></span>
<span data-ttu-id="a5aa3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a5aa3-130">応答</span><span class="sxs-lookup"><span data-stu-id="a5aa3-130">Response</span></span>
<span data-ttu-id="a5aa3-131">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5aa3-132">例</span><span class="sxs-lookup"><span data-stu-id="a5aa3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5aa3-133">要求</span><span class="sxs-lookup"><span data-stu-id="a5aa3-133">Request</span></span>
<span data-ttu-id="a5aa3-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="a5aa3-135">応答</span><span class="sxs-lookup"><span data-stu-id="a5aa3-135">Response</span></span>

<span data-ttu-id="a5aa3-136">応答本文はありません。</span><span class="sxs-lookup"><span data-stu-id="a5aa3-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5aa3-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="a5aa3-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a5aa3-138">Visual</span><span class="sxs-lookup"><span data-stu-id="a5aa3-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_reset-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5aa3-139">Java</span><span class="sxs-lookup"><span data-stu-id="a5aa3-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_reset-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
