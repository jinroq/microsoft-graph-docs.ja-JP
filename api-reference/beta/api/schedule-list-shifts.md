---
title: シフトの一覧表示
description: スケジュール内のシフトの一覧を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1250ac0d05636d83602412c912bff604938a317a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545493"
---
# <a name="list-shifts"></a><span data-ttu-id="0a0b0-103">シフトの一覧表示</span><span class="sxs-lookup"><span data-stu-id="0a0b0-103">List shifts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="0a0b0-104">[スケジュール](../resources/schedule.md)に含まれる[シフト](../resources/shift.md)インスタンスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-104">Get the list of [shift](../resources/shift.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a0b0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a0b0-105">Permissions</span></span>

<span data-ttu-id="0a0b0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a0b0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a0b0-108">Permission type</span></span>      | <span data-ttu-id="0a0b0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a0b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a0b0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a0b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0a0b0-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a0b0-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a0b0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a0b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a0b0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-113">Not supported.</span></span>    |
|<span data-ttu-id="0a0b0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a0b0-114">Application</span></span> | <span data-ttu-id="0a0b0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-115">Not supported.</span></span> |

> <span data-ttu-id="0a0b0-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0a0b0-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0a0b0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a0b0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a0b0-119">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0a0b0-119">Optional query parameters</span></span>
<span data-ttu-id="0a0b0-120">このメソッドは、応答をカスタマイズするための $filter [OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-120">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a0b0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a0b0-121">Request headers</span></span>

| <span data-ttu-id="0a0b0-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a0b0-122">Header</span></span>       | <span data-ttu-id="0a0b0-123">値</span><span class="sxs-lookup"><span data-stu-id="0a0b0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a0b0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a0b0-124">Authorization</span></span>  | <span data-ttu-id="0a0b0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a0b0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a0b0-127">Content-Type</span></span>  | <span data-ttu-id="0a0b0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0a0b0-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a0b0-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a0b0-129">Request body</span></span>
<span data-ttu-id="0a0b0-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a0b0-131">応答</span><span class="sxs-lookup"><span data-stu-id="0a0b0-131">Response</span></span>

<span data-ttu-id="0a0b0-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[shift](../resources/shift.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-132">If successful, this method returns a `200 OK` response code and a collection of [shift](../resources/shift.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a0b0-133">例</span><span class="sxs-lookup"><span data-stu-id="0a0b0-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0a0b0-134">要求</span><span class="sxs-lookup"><span data-stu-id="0a0b0-134">Request</span></span>

<span data-ttu-id="0a0b0-135">次に示すのは、共有バージョンを持つすべての**shift**オブジェクトを取得する要求の例です。2019年3月11日から18月11日までの下書きバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-135">The following is an example of a request that gets all **shift** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-list-shifts"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts?$filter=sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z
```

#### <a name="response"></a><span data-ttu-id="0a0b0-136">応答</span><span class="sxs-lookup"><span data-stu-id="0a0b0-136">Response</span></span>

<span data-ttu-id="0a0b0-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-137">The following is an example of the response.</span></span> 

><span data-ttu-id="0a0b0-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0a0b0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of shifts in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-list-shifts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
