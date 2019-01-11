---
title: EducationSynchronizationProfile の同期をリセットします。
description: テナントで特定の学校のデータの同期プロファイルの同期をリセットします。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 54352d29280d671aaddc152307d8669f64c11bdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808541"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="73888-103">EducationSynchronizationProfile の同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="73888-103">Reset sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="73888-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="73888-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73888-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73888-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73888-106">テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="73888-106">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="73888-107">**注:** 再起動するのには同期は、この操作が行われます。</span><span class="sxs-lookup"><span data-stu-id="73888-107">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="73888-108">検出されたエラーは削除されます。</span><span class="sxs-lookup"><span data-stu-id="73888-108">Any errors encountered will be deleted.</span></span> <span data-ttu-id="73888-109">Azure Active Directory (AD の Azure) からのデータは削除されません。</span><span class="sxs-lookup"><span data-stu-id="73888-109">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="73888-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73888-110">Permissions</span></span>
<span data-ttu-id="73888-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73888-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73888-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73888-113">Permission type</span></span> | <span data-ttu-id="73888-114">Permissions</span><span class="sxs-lookup"><span data-stu-id="73888-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="73888-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73888-115">Delegated (work or school account)</span></span> | <span data-ttu-id="73888-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73888-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="73888-117">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="73888-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="73888-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73888-118">Not supported.</span></span>|
|<span data-ttu-id="73888-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73888-119">Application</span></span>|<span data-ttu-id="73888-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73888-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73888-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73888-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="73888-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73888-122">Request headers</span></span>
| <span data-ttu-id="73888-123">名前</span><span class="sxs-lookup"><span data-stu-id="73888-123">Name</span></span>       | <span data-ttu-id="73888-124">種類</span><span class="sxs-lookup"><span data-stu-id="73888-124">Type</span></span> | <span data-ttu-id="73888-125">説明</span><span class="sxs-lookup"><span data-stu-id="73888-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73888-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="73888-126">Authorization</span></span>  | <span data-ttu-id="73888-127">string</span><span class="sxs-lookup"><span data-stu-id="73888-127">string</span></span>  | <span data-ttu-id="73888-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73888-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73888-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="73888-130">Request body</span></span>
<span data-ttu-id="73888-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73888-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="73888-132">応答</span><span class="sxs-lookup"><span data-stu-id="73888-132">Response</span></span>
<span data-ttu-id="73888-133">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="73888-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="73888-134">例</span><span class="sxs-lookup"><span data-stu-id="73888-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73888-135">要求</span><span class="sxs-lookup"><span data-stu-id="73888-135">Request</span></span>
<span data-ttu-id="73888-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="73888-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="73888-137">応答</span><span class="sxs-lookup"><span data-stu-id="73888-137">Response</span></span>

<span data-ttu-id="73888-138">応答の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="73888-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
