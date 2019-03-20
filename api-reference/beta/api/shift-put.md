---
title: shift を置換する
description: 既存の稼働時間帯を置き換えます。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d8614739757e3962e671440a9a893b9b06d6761f
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657848"
---
# <a name="replace-shift"></a><span data-ttu-id="b14fc-103">shift を置換する</span><span class="sxs-lookup"><span data-stu-id="b14fc-103">Replace shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b14fc-104">既存の[稼働時間帯](../resources/shift.md)を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="b14fc-104">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="b14fc-105">指定した[シフト](../resources/shift.md)が存在しない場合、 `404 Not found`このメソッドはを返します。</span><span class="sxs-lookup"><span data-stu-id="b14fc-105">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b14fc-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b14fc-106">Permissions</span></span>

<span data-ttu-id="b14fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b14fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b14fc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b14fc-109">Permission type</span></span>      | <span data-ttu-id="b14fc-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b14fc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b14fc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b14fc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b14fc-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b14fc-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b14fc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b14fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b14fc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b14fc-114">Not supported.</span></span>    |
|<span data-ttu-id="b14fc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b14fc-115">Application</span></span> | <span data-ttu-id="b14fc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b14fc-116">Not supported.</span></span> |

> <span data-ttu-id="b14fc-117">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b14fc-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b14fc-118">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b14fc-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b14fc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b14fc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="b14fc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b14fc-120">Request headers</span></span>

| <span data-ttu-id="b14fc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b14fc-121">Header</span></span>       | <span data-ttu-id="b14fc-122">値</span><span class="sxs-lookup"><span data-stu-id="b14fc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b14fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b14fc-123">Authorization</span></span>  | <span data-ttu-id="b14fc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b14fc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b14fc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b14fc-126">Content-Type</span></span>  | <span data-ttu-id="b14fc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b14fc-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b14fc-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b14fc-128">Request body</span></span>

<span data-ttu-id="b14fc-129">要求本文で、 [shift](../resources/shift.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b14fc-129">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b14fc-130">応答</span><span class="sxs-lookup"><span data-stu-id="b14fc-130">Response</span></span>

<span data-ttu-id="b14fc-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[shift](../resources/shift.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b14fc-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b14fc-132">例</span><span class="sxs-lookup"><span data-stu-id="b14fc-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b14fc-133">要求</span><span class="sxs-lookup"><span data-stu-id="b14fc-133">Request</span></span>

<span data-ttu-id="b14fc-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b14fc-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
Content-type: application/json
Prefer: return=representation

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

#### <a name="response"></a><span data-ttu-id="b14fc-135">応答</span><span class="sxs-lookup"><span data-stu-id="b14fc-135">Response</span></span>

<span data-ttu-id="b14fc-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b14fc-136">The following is an example of the response.</span></span> 

><span data-ttu-id="b14fc-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b14fc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "string",
  "userId": "string",
  "schedulingGroupId": "string",
  "sharedShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "draftShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "createdDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedBy": {
    "user": {
      "id": "string",
      "displayName": "string"
    },
    "application": {
      "id": "string",
      "displayName": "string"
    },
    "device": {
      "id": "string",
      "displayName": "string"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/shift-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->