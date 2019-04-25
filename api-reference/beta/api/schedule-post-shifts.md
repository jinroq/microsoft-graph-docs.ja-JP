---
title: shift を作成する
description: 新しい shift キーを作成します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ae7ff2f598373d58b2a01b678dbb70ae8e290b2d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545601"
---
# <a name="create-shift"></a><span data-ttu-id="6a4cf-103">shift を作成する</span><span class="sxs-lookup"><span data-stu-id="6a4cf-103">Create shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a4cf-104">[スケジュール](../resources/schedule.md)に新しい[shift](../resources/shift.md)インスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-104">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a4cf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a4cf-105">Permissions</span></span>

<span data-ttu-id="6a4cf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a4cf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a4cf-108">Permission type</span></span>      | <span data-ttu-id="6a4cf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a4cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a4cf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a4cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6a4cf-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a4cf-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6a4cf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a4cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a4cf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-113">Not supported.</span></span>    |
|<span data-ttu-id="6a4cf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a4cf-114">Application</span></span> | <span data-ttu-id="6a4cf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-115">Not supported.</span></span> |

> <span data-ttu-id="6a4cf-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6a4cf-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a4cf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a4cf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="6a4cf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a4cf-119">Request headers</span></span>

| <span data-ttu-id="6a4cf-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a4cf-120">Header</span></span>       | <span data-ttu-id="6a4cf-121">値</span><span class="sxs-lookup"><span data-stu-id="6a4cf-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6a4cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a4cf-122">Authorization</span></span>  | <span data-ttu-id="6a4cf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6a4cf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a4cf-125">Content-Type</span></span>  | <span data-ttu-id="6a4cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a4cf-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="6a4cf-127">応答</span><span class="sxs-lookup"><span data-stu-id="6a4cf-127">Response</span></span>

<span data-ttu-id="6a4cf-128">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[shift](../resources/shift.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-128">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a4cf-129">例</span><span class="sxs-lookup"><span data-stu-id="6a4cf-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6a4cf-130">要求</span><span class="sxs-lookup"><span data-stu-id="6a4cf-130">Request</span></span>

<span data-ttu-id="6a4cf-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-post-shifts"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts
Content-type: application/json

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```

#### <a name="response"></a><span data-ttu-id="6a4cf-132">応答</span><span class="sxs-lookup"><span data-stu-id="6a4cf-132">Response</span></span>

<span data-ttu-id="6a4cf-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-133">The following is an example of the response.</span></span> 

><span data-ttu-id="6a4cf-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-shifts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
