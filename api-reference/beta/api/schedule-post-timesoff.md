---
title: timeoff の作成
description: 新しい休暇を作成します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: df954be9d07797e663b205af6d4dc1ef5dfb20ff
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657505"
---
# <a name="create-timeoff"></a><span data-ttu-id="53565-103">timeoff の作成</span><span class="sxs-lookup"><span data-stu-id="53565-103">Create timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53565-104">[スケジュール](../resources/schedule.md)に新しい[timeoff](../resources/timeoff.md)インスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="53565-104">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="53565-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53565-105">Permissions</span></span>

<span data-ttu-id="53565-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53565-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53565-108">Permission type</span></span>      | <span data-ttu-id="53565-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53565-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53565-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53565-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53565-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53565-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="53565-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53565-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53565-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53565-113">Not supported.</span></span>    |
|<span data-ttu-id="53565-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53565-114">Application</span></span> | <span data-ttu-id="53565-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53565-115">Not supported.</span></span> |

> <span data-ttu-id="53565-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="53565-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="53565-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="53565-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="53565-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53565-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="53565-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53565-119">Request headers</span></span>

| <span data-ttu-id="53565-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53565-120">Header</span></span>       | <span data-ttu-id="53565-121">値</span><span class="sxs-lookup"><span data-stu-id="53565-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53565-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53565-122">Authorization</span></span>  | <span data-ttu-id="53565-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="53565-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="53565-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53565-125">Content-Type</span></span>  | <span data-ttu-id="53565-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53565-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="53565-127">応答</span><span class="sxs-lookup"><span data-stu-id="53565-127">Response</span></span>

<span data-ttu-id="53565-128">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[timeoff](../resources/timeoff.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53565-128">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53565-129">例</span><span class="sxs-lookup"><span data-stu-id="53565-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="53565-130">要求</span><span class="sxs-lookup"><span data-stu-id="53565-130">Request</span></span>

<span data-ttu-id="53565-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="53565-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-post"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff
Content-type: application/json

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

#### <a name="response"></a><span data-ttu-id="53565-132">応答</span><span class="sxs-lookup"><span data-stu-id="53565-132">Response</span></span>

<span data-ttu-id="53565-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="53565-133">The following is an example of the response.</span></span> 

><span data-ttu-id="53565-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="53565-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "schedule-post-timesoff"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-timesoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
