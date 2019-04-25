---
title: timeoffreasons 理由を一覧表示する
description: スケジュールに含まれる timeoffreasons のリストを取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f91fab2b2a0acdd095b6c46168bd9971b40b667d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545803"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="2545d-103">timeoffreasons 理由を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2545d-103">List timeOffReasons</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="2545d-104">[スケジュール](../resources/schedule.md)に含まれる[timeoffreasons](../resources/timeoffreason.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="2545d-104">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2545d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2545d-105">Permissions</span></span>

<span data-ttu-id="2545d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2545d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2545d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2545d-108">Permission type</span></span>      | <span data-ttu-id="2545d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2545d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2545d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2545d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2545d-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2545d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2545d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2545d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2545d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2545d-113">Not supported.</span></span>    |
|<span data-ttu-id="2545d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2545d-114">Application</span></span> | <span data-ttu-id="2545d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2545d-115">Not supported.</span></span> |

> <span data-ttu-id="2545d-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2545d-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2545d-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="2545d-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2545d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2545d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="2545d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2545d-119">Request headers</span></span>

| <span data-ttu-id="2545d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2545d-120">Header</span></span>       | <span data-ttu-id="2545d-121">値</span><span class="sxs-lookup"><span data-stu-id="2545d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2545d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2545d-122">Authorization</span></span>  | <span data-ttu-id="2545d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2545d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2545d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2545d-125">Content-Type</span></span>  | <span data-ttu-id="2545d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2545d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2545d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2545d-127">Request body</span></span>
<span data-ttu-id="2545d-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2545d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2545d-129">応答</span><span class="sxs-lookup"><span data-stu-id="2545d-129">Response</span></span>

<span data-ttu-id="2545d-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[timeoffreason](../resources/timeoffreason.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2545d-130">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2545d-131">例</span><span class="sxs-lookup"><span data-stu-id="2545d-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2545d-132">要求</span><span class="sxs-lookup"><span data-stu-id="2545d-132">Request</span></span>

<span data-ttu-id="2545d-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2545d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
```

#### <a name="response"></a><span data-ttu-id="2545d-134">応答</span><span class="sxs-lookup"><span data-stu-id="2545d-134">Response</span></span>

<span data-ttu-id="2545d-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2545d-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2545d-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2545d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
      "createdDateTime": "2019-03-12T22:10:38.242Z",
      "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
      "displayName": "Vacation",
      "iconType": "plane",
      "isActive": true,
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of timeOffReason in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-list-timeoffreasons.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
