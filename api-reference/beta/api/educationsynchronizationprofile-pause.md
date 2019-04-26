---
title: educationSynchronizationProfile 上で同期を一時停止する
description: テナント内の特定の学校データ同期プロファイルの同期を一時停止します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e903ff08c6bb2e3a3bd56a20ca526a0b1ff42909
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324382"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="a3357-103">educationSynchronizationProfile 上で同期を一時停止する</span><span class="sxs-lookup"><span data-stu-id="a3357-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3357-104">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の同期を一時停止します。</span><span class="sxs-lookup"><span data-stu-id="a3357-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3357-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3357-105">Permissions</span></span>
<span data-ttu-id="a3357-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3357-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3357-108">Permission type</span></span> | <span data-ttu-id="a3357-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3357-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="a3357-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3357-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3357-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3357-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="a3357-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="a3357-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a3357-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3357-113">Not supported.</span></span>|
|<span data-ttu-id="a3357-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3357-114">Application</span></span>|<span data-ttu-id="a3357-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3357-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3357-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3357-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="a3357-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3357-117">Request headers</span></span>
| <span data-ttu-id="a3357-118">名前</span><span class="sxs-lookup"><span data-stu-id="a3357-118">Name</span></span>       | <span data-ttu-id="a3357-119">型</span><span class="sxs-lookup"><span data-stu-id="a3357-119">Type</span></span> | <span data-ttu-id="a3357-120">説明</span><span class="sxs-lookup"><span data-stu-id="a3357-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a3357-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3357-121">Authorization</span></span>  | <span data-ttu-id="a3357-122">string</span><span class="sxs-lookup"><span data-stu-id="a3357-122">string</span></span>  | <span data-ttu-id="a3357-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a3357-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3357-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3357-125">Request body</span></span>
<span data-ttu-id="a3357-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3357-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a3357-127">応答</span><span class="sxs-lookup"><span data-stu-id="a3357-127">Response</span></span>
<span data-ttu-id="a3357-128">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a3357-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a3357-129">例</span><span class="sxs-lookup"><span data-stu-id="a3357-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3357-130">要求</span><span class="sxs-lookup"><span data-stu-id="a3357-130">Request</span></span>
<span data-ttu-id="a3357-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3357-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="a3357-132">応答</span><span class="sxs-lookup"><span data-stu-id="a3357-132">Response</span></span>

<span data-ttu-id="a3357-133">応答本文はありません。</span><span class="sxs-lookup"><span data-stu-id="a3357-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
