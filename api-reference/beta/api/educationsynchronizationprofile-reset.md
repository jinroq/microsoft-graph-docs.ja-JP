---
title: EducationSynchronizationProfile の同期をリセットします。
description: テナントで特定の学校のデータの同期プロファイルの同期をリセットします。
ms.openlocfilehash: 4be91b7d6229148c51dc8fb1279a9078fb5cad7b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071049"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="6223c-103">EducationSynchronizationProfile の同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="6223c-103">Reset sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="6223c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6223c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6223c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6223c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6223c-106">テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="6223c-106">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="6223c-107">**注:** 再起動するのには同期は、この操作が行われます。</span><span class="sxs-lookup"><span data-stu-id="6223c-107">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="6223c-108">検出されたエラーは削除されます。</span><span class="sxs-lookup"><span data-stu-id="6223c-108">Any errors encountered will be deleted.</span></span> <span data-ttu-id="6223c-109">Azure Active Directory (AD の Azure) からのデータは削除されません。</span><span class="sxs-lookup"><span data-stu-id="6223c-109">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="6223c-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6223c-110">Permissions</span></span>
<span data-ttu-id="6223c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6223c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6223c-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6223c-113">Permission type</span></span> | <span data-ttu-id="6223c-114">Permissions</span><span class="sxs-lookup"><span data-stu-id="6223c-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="6223c-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6223c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6223c-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6223c-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="6223c-117">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="6223c-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6223c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6223c-118">Not supported.</span></span>|
|<span data-ttu-id="6223c-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6223c-119">Application</span></span>|<span data-ttu-id="6223c-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6223c-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6223c-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6223c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="6223c-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6223c-122">Request headers</span></span>
| <span data-ttu-id="6223c-123">名前</span><span class="sxs-lookup"><span data-stu-id="6223c-123">Name</span></span>       | <span data-ttu-id="6223c-124">型</span><span class="sxs-lookup"><span data-stu-id="6223c-124">Type</span></span> | <span data-ttu-id="6223c-125">説明</span><span class="sxs-lookup"><span data-stu-id="6223c-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6223c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6223c-126">Authorization</span></span>  | <span data-ttu-id="6223c-127">string</span><span class="sxs-lookup"><span data-stu-id="6223c-127">string</span></span>  | <span data-ttu-id="6223c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6223c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6223c-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="6223c-130">Request body</span></span>
<span data-ttu-id="6223c-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6223c-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6223c-132">応答</span><span class="sxs-lookup"><span data-stu-id="6223c-132">Response</span></span>
<span data-ttu-id="6223c-133">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6223c-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6223c-134">例</span><span class="sxs-lookup"><span data-stu-id="6223c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6223c-135">要求</span><span class="sxs-lookup"><span data-stu-id="6223c-135">Request</span></span>
<span data-ttu-id="6223c-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6223c-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="6223c-137">応答</span><span class="sxs-lookup"><span data-stu-id="6223c-137">Response</span></span>

<span data-ttu-id="6223c-138">応答の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="6223c-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```