---
title: EducationSynchronizationProfile のステータスを取得します。
description: テナント内には、特定の学校のデータの同期プロファイルの状態を取得します。 応答は、同期のステータスを示します。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: f371d86d188068a90b3a9503adea12fd38ba8e8d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869957"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="7fc84-104">EducationSynchronizationProfile のステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="7fc84-104">Get the status of an educationSynchronizationProfile</span></span>

> <span data-ttu-id="7fc84-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7fc84-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fc84-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fc84-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7fc84-107">テナント内には、特定の学校のデータ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="7fc84-107">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="7fc84-108">応答は、同期のステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="7fc84-108">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fc84-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7fc84-109">Permissions</span></span>
<span data-ttu-id="7fc84-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7fc84-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7fc84-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7fc84-112">Permission type</span></span> | <span data-ttu-id="7fc84-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7fc84-113">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="7fc84-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7fc84-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7fc84-115">EduAdministration.Read、EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fc84-115">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="7fc84-116">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="7fc84-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7fc84-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fc84-117">Not supported.</span></span>|
|<span data-ttu-id="7fc84-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7fc84-118">Application</span></span>| <span data-ttu-id="7fc84-119">EduAdministration.Read.All、EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc84-119">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fc84-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7fc84-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="7fc84-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7fc84-121">Request headers</span></span>
| <span data-ttu-id="7fc84-122">名前</span><span class="sxs-lookup"><span data-stu-id="7fc84-122">Name</span></span>       | <span data-ttu-id="7fc84-123">種類</span><span class="sxs-lookup"><span data-stu-id="7fc84-123">Type</span></span> | <span data-ttu-id="7fc84-124">説明</span><span class="sxs-lookup"><span data-stu-id="7fc84-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7fc84-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fc84-125">Authorization</span></span>  | <span data-ttu-id="7fc84-126">string</span><span class="sxs-lookup"><span data-stu-id="7fc84-126">string</span></span>  | <span data-ttu-id="7fc84-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7fc84-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fc84-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="7fc84-129">Request body</span></span>
<span data-ttu-id="7fc84-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7fc84-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7fc84-131">応答</span><span class="sxs-lookup"><span data-stu-id="7fc84-131">Response</span></span>
<span data-ttu-id="7fc84-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7fc84-132">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fc84-133">例</span><span class="sxs-lookup"><span data-stu-id="7fc84-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fc84-134">要求</span><span class="sxs-lookup"><span data-stu-id="7fc84-134">Request</span></span>
<span data-ttu-id="7fc84-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7fc84-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="7fc84-136">応答</span><span class="sxs-lookup"><span data-stu-id="7fc84-136">Response</span></span>
<span data-ttu-id="7fc84-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7fc84-137">The following is an example of the response.</span></span> 

><span data-ttu-id="7fc84-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7fc84-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```
