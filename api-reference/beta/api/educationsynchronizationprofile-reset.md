---
title: EducationSynchronizationProfile の同期をリセットします。
description: テナントで特定の学校のデータの同期プロファイルの同期をリセットします。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 502eb8d7afdc61926a024b7ddfbac5383a146622
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520411"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="2103b-103">EducationSynchronizationProfile の同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="2103b-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2103b-104">テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="2103b-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="2103b-105">**注:** 再起動するのには同期は、この操作が行われます。</span><span class="sxs-lookup"><span data-stu-id="2103b-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="2103b-106">検出されたエラーは削除されます。</span><span class="sxs-lookup"><span data-stu-id="2103b-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="2103b-107">Azure Active Directory (AD の Azure) からのデータは削除されません。</span><span class="sxs-lookup"><span data-stu-id="2103b-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2103b-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2103b-108">Permissions</span></span>
<span data-ttu-id="2103b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2103b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2103b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2103b-111">Permission type</span></span> | <span data-ttu-id="2103b-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2103b-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="2103b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2103b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2103b-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2103b-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="2103b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2103b-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2103b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2103b-116">Not supported.</span></span>|
|<span data-ttu-id="2103b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2103b-117">Application</span></span>|<span data-ttu-id="2103b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2103b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2103b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2103b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="2103b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2103b-120">Request headers</span></span>
| <span data-ttu-id="2103b-121">名前</span><span class="sxs-lookup"><span data-stu-id="2103b-121">Name</span></span>       | <span data-ttu-id="2103b-122">型</span><span class="sxs-lookup"><span data-stu-id="2103b-122">Type</span></span> | <span data-ttu-id="2103b-123">説明</span><span class="sxs-lookup"><span data-stu-id="2103b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2103b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2103b-124">Authorization</span></span>  | <span data-ttu-id="2103b-125">string</span><span class="sxs-lookup"><span data-stu-id="2103b-125">string</span></span>  | <span data-ttu-id="2103b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2103b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2103b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2103b-128">Request body</span></span>
<span data-ttu-id="2103b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2103b-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2103b-130">応答</span><span class="sxs-lookup"><span data-stu-id="2103b-130">Response</span></span>
<span data-ttu-id="2103b-131">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2103b-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2103b-132">例</span><span class="sxs-lookup"><span data-stu-id="2103b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2103b-133">要求</span><span class="sxs-lookup"><span data-stu-id="2103b-133">Request</span></span>
<span data-ttu-id="2103b-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2103b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="2103b-135">応答</span><span class="sxs-lookup"><span data-stu-id="2103b-135">Response</span></span>

<span data-ttu-id="2103b-136">応答の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="2103b-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
