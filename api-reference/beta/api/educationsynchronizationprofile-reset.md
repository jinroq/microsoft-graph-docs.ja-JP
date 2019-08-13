---
title: EducationSynchronizationProfile の同期をリセットする
description: テナント内の特定の学校データ同期プロファイルの同期をリセットします。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 39eb45fca9f4952f8fa557af40c08a037f7fb678
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323830"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="06701-103">EducationSynchronizationProfile の同期をリセットする</span><span class="sxs-lookup"><span data-stu-id="06701-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06701-104">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="06701-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="06701-105">**注:** この操作を行うと、同期が再開されます。</span><span class="sxs-lookup"><span data-stu-id="06701-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="06701-106">発生したエラーは削除されます。</span><span class="sxs-lookup"><span data-stu-id="06701-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="06701-107">Azure Active Directory (Azure AD) からデータが削除されることはありません。</span><span class="sxs-lookup"><span data-stu-id="06701-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="06701-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="06701-108">Permissions</span></span>
<span data-ttu-id="06701-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06701-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06701-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06701-111">Permission type</span></span> | <span data-ttu-id="06701-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="06701-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="06701-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06701-113">Delegated (work or school account)</span></span> | <span data-ttu-id="06701-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06701-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="06701-115">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="06701-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="06701-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06701-116">Not supported.</span></span>|
|<span data-ttu-id="06701-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06701-117">Application</span></span>|<span data-ttu-id="06701-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06701-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06701-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06701-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="06701-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06701-120">Request headers</span></span>
| <span data-ttu-id="06701-121">名前</span><span class="sxs-lookup"><span data-stu-id="06701-121">Name</span></span>       | <span data-ttu-id="06701-122">型</span><span class="sxs-lookup"><span data-stu-id="06701-122">Type</span></span> | <span data-ttu-id="06701-123">説明</span><span class="sxs-lookup"><span data-stu-id="06701-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06701-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="06701-124">Authorization</span></span>  | <span data-ttu-id="06701-125">string</span><span class="sxs-lookup"><span data-stu-id="06701-125">string</span></span>  | <span data-ttu-id="06701-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="06701-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06701-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="06701-128">Request body</span></span>
<span data-ttu-id="06701-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="06701-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="06701-130">応答</span><span class="sxs-lookup"><span data-stu-id="06701-130">Response</span></span>
<span data-ttu-id="06701-131">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="06701-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="06701-132">例</span><span class="sxs-lookup"><span data-stu-id="06701-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06701-133">要求</span><span class="sxs-lookup"><span data-stu-id="06701-133">Request</span></span>
<span data-ttu-id="06701-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06701-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="06701-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="06701-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06701-136">C#</span><span class="sxs-lookup"><span data-stu-id="06701-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06701-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06701-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06701-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="06701-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="06701-139">Java</span><span class="sxs-lookup"><span data-stu-id="06701-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-reset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="06701-140">応答</span><span class="sxs-lookup"><span data-stu-id="06701-140">Response</span></span>

<span data-ttu-id="06701-141">応答本文はありません。</span><span class="sxs-lookup"><span data-stu-id="06701-141">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
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
