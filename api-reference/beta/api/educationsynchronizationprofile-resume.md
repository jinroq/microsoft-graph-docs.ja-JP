---
title: educationSynchronizationProfile での同期の再開
description: テナント内の特定の学校データ同期プロファイルの同期を再開します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8fd56ec1d825104cb442f9184c1735e34b557fce
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324960"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="70786-103">educationSynchronizationProfile での同期の再開</span><span class="sxs-lookup"><span data-stu-id="70786-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70786-104">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="70786-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="70786-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="70786-105">Permissions</span></span>
<span data-ttu-id="70786-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70786-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70786-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="70786-108">Permission type</span></span> | <span data-ttu-id="70786-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="70786-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="70786-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="70786-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70786-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70786-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="70786-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="70786-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="70786-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70786-113">Not supported.</span></span>|
|<span data-ttu-id="70786-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="70786-114">Application</span></span>|<span data-ttu-id="70786-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70786-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70786-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70786-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="70786-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70786-117">Request headers</span></span>
| <span data-ttu-id="70786-118">名前</span><span class="sxs-lookup"><span data-stu-id="70786-118">Name</span></span>       | <span data-ttu-id="70786-119">型</span><span class="sxs-lookup"><span data-stu-id="70786-119">Type</span></span> | <span data-ttu-id="70786-120">説明</span><span class="sxs-lookup"><span data-stu-id="70786-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70786-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70786-121">Authorization</span></span>  | <span data-ttu-id="70786-122">string</span><span class="sxs-lookup"><span data-stu-id="70786-122">string</span></span>  | <span data-ttu-id="70786-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="70786-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70786-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="70786-125">Request body</span></span>
<span data-ttu-id="70786-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="70786-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="70786-127">応答</span><span class="sxs-lookup"><span data-stu-id="70786-127">Response</span></span>
<span data-ttu-id="70786-128">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="70786-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="70786-129">例</span><span class="sxs-lookup"><span data-stu-id="70786-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70786-130">要求</span><span class="sxs-lookup"><span data-stu-id="70786-130">Request</span></span>
<span data-ttu-id="70786-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="70786-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="70786-132">応答</span><span class="sxs-lookup"><span data-stu-id="70786-132">Response</span></span>

<span data-ttu-id="70786-133">応答本文はありません。</span><span class="sxs-lookup"><span data-stu-id="70786-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
