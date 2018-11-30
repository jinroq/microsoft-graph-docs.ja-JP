---
title: EducationSynchronizationProfile を削除します。
description: 識別子に基づくテナントの学校のデータの同期プロファイルを削除します。
ms.openlocfilehash: 829b723b48eb9a15750bc9d0e00ba50d432e8ab6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071108"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="7afcd-103">EducationSynchronizationProfile を削除します。</span><span class="sxs-lookup"><span data-stu-id="7afcd-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="7afcd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7afcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7afcd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7afcd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7afcd-106">識別子に基づくテナントの学校のデータ[同期プロファイル](../resources/educationsynchronizationprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="7afcd-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="7afcd-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7afcd-107">Permissions</span></span>
<span data-ttu-id="7afcd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7afcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7afcd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7afcd-110">Permission type</span></span> | <span data-ttu-id="7afcd-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="7afcd-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="7afcd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7afcd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7afcd-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7afcd-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7afcd-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7afcd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7afcd-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7afcd-115">Request headers</span></span>
| <span data-ttu-id="7afcd-116">名前</span><span class="sxs-lookup"><span data-stu-id="7afcd-116">Name</span></span>       | <span data-ttu-id="7afcd-117">型</span><span class="sxs-lookup"><span data-stu-id="7afcd-117">Type</span></span> | <span data-ttu-id="7afcd-118">説明</span><span class="sxs-lookup"><span data-stu-id="7afcd-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7afcd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7afcd-119">Authorization</span></span>  | <span data-ttu-id="7afcd-120">string</span><span class="sxs-lookup"><span data-stu-id="7afcd-120">string</span></span>  | <span data-ttu-id="7afcd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7afcd-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="7afcd-123">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="7afcd-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7afcd-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7afcd-124">Not supported.</span></span>|
|<span data-ttu-id="7afcd-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7afcd-125">Application</span></span>|<span data-ttu-id="7afcd-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7afcd-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7afcd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7afcd-127">Request body</span></span>
<span data-ttu-id="7afcd-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7afcd-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7afcd-129">応答</span><span class="sxs-lookup"><span data-stu-id="7afcd-129">Response</span></span>
<span data-ttu-id="7afcd-130">成功した場合、このメソッドは `202 Accepted` 応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="7afcd-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="7afcd-131">例</span><span class="sxs-lookup"><span data-stu-id="7afcd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7afcd-132">要求</span><span class="sxs-lookup"><span data-stu-id="7afcd-132">Request</span></span>
<span data-ttu-id="7afcd-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7afcd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="7afcd-134">応答</span><span class="sxs-lookup"><span data-stu-id="7afcd-134">Response</span></span>
<span data-ttu-id="7afcd-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7afcd-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
