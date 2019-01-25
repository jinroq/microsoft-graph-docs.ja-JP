---
title: EducationSynchronizationProfile の同期を再開します。
description: テナントで特定の学校のデータの同期プロファイルの同期を再開します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 50ffcb4ceab401a3041ecb69baa1de0409be94a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513257"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="300d1-103">EducationSynchronizationProfile の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="300d1-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="300d1-104">テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="300d1-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="300d1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="300d1-105">Permissions</span></span>
<span data-ttu-id="300d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="300d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="300d1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="300d1-108">Permission type</span></span> | <span data-ttu-id="300d1-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="300d1-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="300d1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="300d1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="300d1-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="300d1-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="300d1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="300d1-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="300d1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="300d1-113">Not supported.</span></span>|
|<span data-ttu-id="300d1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="300d1-114">Application</span></span>|<span data-ttu-id="300d1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="300d1-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="300d1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="300d1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="300d1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="300d1-117">Request headers</span></span>
| <span data-ttu-id="300d1-118">名前</span><span class="sxs-lookup"><span data-stu-id="300d1-118">Name</span></span>       | <span data-ttu-id="300d1-119">型</span><span class="sxs-lookup"><span data-stu-id="300d1-119">Type</span></span> | <span data-ttu-id="300d1-120">説明</span><span class="sxs-lookup"><span data-stu-id="300d1-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="300d1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="300d1-121">Authorization</span></span>  | <span data-ttu-id="300d1-122">string</span><span class="sxs-lookup"><span data-stu-id="300d1-122">string</span></span>  | <span data-ttu-id="300d1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="300d1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="300d1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="300d1-125">Request body</span></span>
<span data-ttu-id="300d1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="300d1-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="300d1-127">応答</span><span class="sxs-lookup"><span data-stu-id="300d1-127">Response</span></span>
<span data-ttu-id="300d1-128">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="300d1-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="300d1-129">例</span><span class="sxs-lookup"><span data-stu-id="300d1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="300d1-130">要求</span><span class="sxs-lookup"><span data-stu-id="300d1-130">Request</span></span>
<span data-ttu-id="300d1-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="300d1-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="300d1-132">応答</span><span class="sxs-lookup"><span data-stu-id="300d1-132">Response</span></span>

<span data-ttu-id="300d1-133">応答の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="300d1-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
