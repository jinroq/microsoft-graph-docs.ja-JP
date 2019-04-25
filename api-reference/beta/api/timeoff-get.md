---
title: timeoff を取得する
description: ID で timeoff を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8408fc1c83668b5f3bc6f6086b97915854b7d255
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536905"
---
# <a name="get-timeoff"></a><span data-ttu-id="76c85-103">timeoff を取得する</span><span class="sxs-lookup"><span data-stu-id="76c85-103">Get timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76c85-104">[timeoff](../resources/timeoff.md)オブジェクトのプロパティと関係を ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="76c85-104">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="76c85-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="76c85-105">Permissions</span></span>

<span data-ttu-id="76c85-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76c85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76c85-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76c85-108">Permission type</span></span>      | <span data-ttu-id="76c85-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="76c85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76c85-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76c85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76c85-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76c85-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="76c85-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76c85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76c85-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76c85-113">Not supported.</span></span>    |
|<span data-ttu-id="76c85-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76c85-114">Application</span></span> | <span data-ttu-id="76c85-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76c85-115">Not supported.</span></span> |

> <span data-ttu-id="76c85-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="76c85-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="76c85-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="76c85-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="76c85-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76c85-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="76c85-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76c85-119">Request headers</span></span>

| <span data-ttu-id="76c85-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76c85-120">Header</span></span>       | <span data-ttu-id="76c85-121">値</span><span class="sxs-lookup"><span data-stu-id="76c85-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="76c85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76c85-122">Authorization</span></span>  | <span data-ttu-id="76c85-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="76c85-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="76c85-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76c85-125">Content-Type</span></span>  | <span data-ttu-id="76c85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76c85-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76c85-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="76c85-127">Request body</span></span>
<span data-ttu-id="76c85-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="76c85-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76c85-129">応答</span><span class="sxs-lookup"><span data-stu-id="76c85-129">Response</span></span>

<span data-ttu-id="76c85-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[timeoff](../resources/timeoff.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="76c85-130">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76c85-131">例</span><span class="sxs-lookup"><span data-stu-id="76c85-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="76c85-132">要求</span><span class="sxs-lookup"><span data-stu-id="76c85-132">Request</span></span>

<span data-ttu-id="76c85-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76c85-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="76c85-134">応答</span><span class="sxs-lookup"><span data-stu-id="76c85-134">Response</span></span>

<span data-ttu-id="76c85-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76c85-135">The following is an example of the response.</span></span> 

><span data-ttu-id="76c85-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="76c85-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Get a timeOff by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
