---
title: educationSynchronizationProfile を削除する
description: 識別子に基づいて、テナント内の学校データ同期プロファイルを削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2aaa0d47bcc98c814ad525deb781ac7a7df28d87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457453"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="ce0fb-103">educationSynchronizationProfile を削除する</span><span class="sxs-lookup"><span data-stu-id="ce0fb-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce0fb-104">識別子に基づいて、テナント内の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="ce0fb-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce0fb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce0fb-105">Permissions</span></span>
<span data-ttu-id="ce0fb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce0fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce0fb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce0fb-108">Permission type</span></span> | <span data-ttu-id="ce0fb-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce0fb-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ce0fb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce0fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce0fb-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce0fb-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce0fb-112">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce0fb-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ce0fb-113">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce0fb-113">Request headers</span></span>
| <span data-ttu-id="ce0fb-114">名前</span><span class="sxs-lookup"><span data-stu-id="ce0fb-114">Name</span></span>       | <span data-ttu-id="ce0fb-115">型</span><span class="sxs-lookup"><span data-stu-id="ce0fb-115">Type</span></span> | <span data-ttu-id="ce0fb-116">説明</span><span class="sxs-lookup"><span data-stu-id="ce0fb-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ce0fb-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce0fb-117">Authorization</span></span>  | <span data-ttu-id="ce0fb-118">string</span><span class="sxs-lookup"><span data-stu-id="ce0fb-118">string</span></span>  | <span data-ttu-id="ce0fb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce0fb-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="ce0fb-121">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="ce0fb-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ce0fb-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce0fb-122">Not supported.</span></span>|
|<span data-ttu-id="ce0fb-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce0fb-123">Application</span></span>|<span data-ttu-id="ce0fb-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce0fb-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce0fb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce0fb-125">Request body</span></span>
<span data-ttu-id="ce0fb-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce0fb-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ce0fb-127">応答</span><span class="sxs-lookup"><span data-stu-id="ce0fb-127">Response</span></span>
<span data-ttu-id="ce0fb-128">成功した場合、このメソッド`202 Accepted`は応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="ce0fb-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce0fb-129">例</span><span class="sxs-lookup"><span data-stu-id="ce0fb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce0fb-130">要求</span><span class="sxs-lookup"><span data-stu-id="ce0fb-130">Request</span></span>
<span data-ttu-id="ce0fb-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce0fb-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="ce0fb-132">応答</span><span class="sxs-lookup"><span data-stu-id="ce0fb-132">Response</span></span>
<span data-ttu-id="ce0fb-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ce0fb-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
