---
title: イベントを一覧表示する
description: イベント オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c02318a8c7a8c7a8ffc7562d4a807fa06fae47a6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525382"
---
# <a name="list-events"></a><span data-ttu-id="7ebc1-103">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7ebc1-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ebc1-104">[イベント](../resources/event.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ebc1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7ebc1-105">Permissions</span></span>
<span data-ttu-id="7ebc1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ebc1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ebc1-108">Permission type</span></span>      | <span data-ttu-id="7ebc1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ebc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ebc1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ebc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ebc1-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ebc1-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ebc1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ebc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ebc1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-113">Not supported.</span></span>    |
|<span data-ttu-id="7ebc1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ebc1-114">Application</span></span> | <span data-ttu-id="7ebc1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ebc1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ebc1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ebc1-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ebc1-117">Optional query parameters</span></span>
<span data-ttu-id="7ebc1-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ebc1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ebc1-119">Request headers</span></span>
| <span data-ttu-id="7ebc1-120">名前</span><span class="sxs-lookup"><span data-stu-id="7ebc1-120">Name</span></span>       | <span data-ttu-id="7ebc1-121">型</span><span class="sxs-lookup"><span data-stu-id="7ebc1-121">Type</span></span> | <span data-ttu-id="7ebc1-122">説明</span><span class="sxs-lookup"><span data-stu-id="7ebc1-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="7ebc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ebc1-123">Authorization</span></span>  | <span data-ttu-id="7ebc1-124">string</span><span class="sxs-lookup"><span data-stu-id="7ebc1-124">string</span></span> | <span data-ttu-id="7ebc1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ebc1-127">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7ebc1-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="7ebc1-128">string</span><span class="sxs-lookup"><span data-stu-id="7ebc1-128">string</span></span> | <span data-ttu-id="7ebc1-129">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="7ebc1-130">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="7ebc1-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-131">Optional.</span></span> |
| <span data-ttu-id="7ebc1-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="7ebc1-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="7ebc1-133">string</span><span class="sxs-lookup"><span data-stu-id="7ebc1-133">string</span></span> | <span data-ttu-id="7ebc1-134">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="7ebc1-135">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-135">Values can be "text" or "html".</span></span> <span data-ttu-id="7ebc1-136">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="7ebc1-137">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="7ebc1-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ebc1-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ebc1-139">Request body</span></span>
<span data-ttu-id="7ebc1-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ebc1-141">応答</span><span class="sxs-lookup"><span data-stu-id="7ebc1-141">Response</span></span>
<span data-ttu-id="7ebc1-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ebc1-143">例</span><span class="sxs-lookup"><span data-stu-id="7ebc1-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7ebc1-144">要求</span><span class="sxs-lookup"><span data-stu-id="7ebc1-144">Request</span></span>
<span data-ttu-id="7ebc1-145">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="7ebc1-146">応答</span><span class="sxs-lookup"><span data-stu-id="7ebc1-146">Response</span></span>
<span data-ttu-id="7ebc1-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-147">The following is an example of the response.</span></span>
><span data-ttu-id="7ebc1-148">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ebc1-149">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7ebc1-149">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
