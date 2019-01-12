---
title: EducationSynchronizationProfile の同期を再開します。
description: テナントで特定の学校のデータの同期プロファイルの同期を再開します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0a74d85bd902c21f3af6e8aa506438471f142600
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984669"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="497df-103">EducationSynchronizationProfile の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="497df-103">Resume sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="497df-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="497df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="497df-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="497df-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="497df-106">テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="497df-106">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="497df-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="497df-107">Permissions</span></span>
<span data-ttu-id="497df-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="497df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="497df-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="497df-110">Permission type</span></span> | <span data-ttu-id="497df-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="497df-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="497df-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="497df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="497df-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="497df-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="497df-114">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="497df-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="497df-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="497df-115">Not supported.</span></span>|
|<span data-ttu-id="497df-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="497df-116">Application</span></span>|<span data-ttu-id="497df-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="497df-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="497df-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="497df-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="497df-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="497df-119">Request headers</span></span>
| <span data-ttu-id="497df-120">名前</span><span class="sxs-lookup"><span data-stu-id="497df-120">Name</span></span>       | <span data-ttu-id="497df-121">種類</span><span class="sxs-lookup"><span data-stu-id="497df-121">Type</span></span> | <span data-ttu-id="497df-122">説明</span><span class="sxs-lookup"><span data-stu-id="497df-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="497df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="497df-123">Authorization</span></span>  | <span data-ttu-id="497df-124">string</span><span class="sxs-lookup"><span data-stu-id="497df-124">string</span></span>  | <span data-ttu-id="497df-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="497df-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="497df-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="497df-127">Request body</span></span>
<span data-ttu-id="497df-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="497df-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="497df-129">応答</span><span class="sxs-lookup"><span data-stu-id="497df-129">Response</span></span>
<span data-ttu-id="497df-130">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="497df-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="497df-131">例</span><span class="sxs-lookup"><span data-stu-id="497df-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="497df-132">要求</span><span class="sxs-lookup"><span data-stu-id="497df-132">Request</span></span>
<span data-ttu-id="497df-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="497df-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="497df-134">応答</span><span class="sxs-lookup"><span data-stu-id="497df-134">Response</span></span>

<span data-ttu-id="497df-135">応答の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="497df-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
