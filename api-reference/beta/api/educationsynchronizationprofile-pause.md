---
title: EducationSynchronizationProfile の同期を一時停止
description: テナントで特定の学校のデータの同期プロファイルの同期を一時停止します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4979ed19c9a01d6a7ff2d43f7f3755d03b4b070c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950684"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="4c4a9-103">EducationSynchronizationProfile の同期を一時停止</span><span class="sxs-lookup"><span data-stu-id="4c4a9-103">Pause sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="4c4a9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c4a9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c4a9-106">テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の同期を一時停止します。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-106">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c4a9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c4a9-107">Permissions</span></span>
<span data-ttu-id="4c4a9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c4a9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c4a9-110">Permission type</span></span> | <span data-ttu-id="4c4a9-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c4a9-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4c4a9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c4a9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c4a9-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c4a9-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="4c4a9-114">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4c4a9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-115">Not supported.</span></span>|
|<span data-ttu-id="4c4a9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c4a9-116">Application</span></span>|<span data-ttu-id="4c4a9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c4a9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c4a9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="4c4a9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c4a9-119">Request headers</span></span>
| <span data-ttu-id="4c4a9-120">名前</span><span class="sxs-lookup"><span data-stu-id="4c4a9-120">Name</span></span>       | <span data-ttu-id="4c4a9-121">種類</span><span class="sxs-lookup"><span data-stu-id="4c4a9-121">Type</span></span> | <span data-ttu-id="4c4a9-122">説明</span><span class="sxs-lookup"><span data-stu-id="4c4a9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4c4a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c4a9-123">Authorization</span></span>  | <span data-ttu-id="4c4a9-124">string</span><span class="sxs-lookup"><span data-stu-id="4c4a9-124">string</span></span>  | <span data-ttu-id="4c4a9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c4a9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c4a9-127">Request body</span></span>
<span data-ttu-id="4c4a9-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4c4a9-129">応答</span><span class="sxs-lookup"><span data-stu-id="4c4a9-129">Response</span></span>
<span data-ttu-id="4c4a9-130">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4c4a9-131">例</span><span class="sxs-lookup"><span data-stu-id="4c4a9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c4a9-132">要求</span><span class="sxs-lookup"><span data-stu-id="4c4a9-132">Request</span></span>
<span data-ttu-id="4c4a9-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="4c4a9-134">応答</span><span class="sxs-lookup"><span data-stu-id="4c4a9-134">Response</span></span>

<span data-ttu-id="4c4a9-135">応答の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="4c4a9-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
