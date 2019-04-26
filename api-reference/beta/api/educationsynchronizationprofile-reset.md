---
title: educationSynchronizationProfile の同期をリセットする
description: テナント内の特定の学校データ同期プロファイルの同期をリセットします。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ccf257a2fc479f87d1e0b6d2b6414d0e3431fcb6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322312"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="df300-103">educationSynchronizationProfile の同期をリセットする</span><span class="sxs-lookup"><span data-stu-id="df300-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df300-104">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="df300-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="df300-105">**注:** この操作を行うと、同期が再開されます。</span><span class="sxs-lookup"><span data-stu-id="df300-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="df300-106">発生したエラーは削除されます。</span><span class="sxs-lookup"><span data-stu-id="df300-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="df300-107">azure Active Directory (azure AD) からデータが削除されることはありません。</span><span class="sxs-lookup"><span data-stu-id="df300-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="df300-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="df300-108">Permissions</span></span>
<span data-ttu-id="df300-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df300-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df300-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df300-111">Permission type</span></span> | <span data-ttu-id="df300-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="df300-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="df300-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df300-113">Delegated (work or school account)</span></span> | <span data-ttu-id="df300-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df300-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="df300-115">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="df300-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="df300-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df300-116">Not supported.</span></span>|
|<span data-ttu-id="df300-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df300-117">Application</span></span>|<span data-ttu-id="df300-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df300-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df300-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df300-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="df300-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df300-120">Request headers</span></span>
| <span data-ttu-id="df300-121">名前</span><span class="sxs-lookup"><span data-stu-id="df300-121">Name</span></span>       | <span data-ttu-id="df300-122">型</span><span class="sxs-lookup"><span data-stu-id="df300-122">Type</span></span> | <span data-ttu-id="df300-123">説明</span><span class="sxs-lookup"><span data-stu-id="df300-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="df300-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="df300-124">Authorization</span></span>  | <span data-ttu-id="df300-125">string</span><span class="sxs-lookup"><span data-stu-id="df300-125">string</span></span>  | <span data-ttu-id="df300-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="df300-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df300-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="df300-128">Request body</span></span>
<span data-ttu-id="df300-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="df300-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="df300-130">応答</span><span class="sxs-lookup"><span data-stu-id="df300-130">Response</span></span>
<span data-ttu-id="df300-131">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="df300-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df300-132">例</span><span class="sxs-lookup"><span data-stu-id="df300-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df300-133">要求</span><span class="sxs-lookup"><span data-stu-id="df300-133">Request</span></span>
<span data-ttu-id="df300-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="df300-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="df300-135">応答</span><span class="sxs-lookup"><span data-stu-id="df300-135">Response</span></span>

<span data-ttu-id="df300-136">応答本文はありません。</span><span class="sxs-lookup"><span data-stu-id="df300-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
