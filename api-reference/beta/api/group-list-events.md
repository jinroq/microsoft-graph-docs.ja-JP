---
title: イベントを一覧表示する
description: イベント オブジェクトのリストを取得します。
author: dkershaw10
ms.openlocfilehash: fdb996f9be5193c5f18e6adb7de0b16938221e58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355546"
---
# <a name="list-events"></a><span data-ttu-id="00e3f-103">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="00e3f-103">List events</span></span>

> <span data-ttu-id="00e3f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="00e3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00e3f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00e3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00e3f-106">[イベント](../resources/event.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="00e3f-106">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="00e3f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00e3f-107">Permissions</span></span>
<span data-ttu-id="00e3f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00e3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00e3f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00e3f-110">Permission type</span></span>      | <span data-ttu-id="00e3f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00e3f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00e3f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00e3f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="00e3f-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e3f-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="00e3f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00e3f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00e3f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00e3f-115">Not supported.</span></span>    |
|<span data-ttu-id="00e3f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00e3f-116">Application</span></span> | <span data-ttu-id="00e3f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00e3f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00e3f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00e3f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00e3f-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="00e3f-119">Optional query parameters</span></span>
<span data-ttu-id="00e3f-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="00e3f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00e3f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00e3f-121">Request headers</span></span>
| <span data-ttu-id="00e3f-122">名前</span><span class="sxs-lookup"><span data-stu-id="00e3f-122">Name</span></span>       | <span data-ttu-id="00e3f-123">種類</span><span class="sxs-lookup"><span data-stu-id="00e3f-123">Type</span></span> | <span data-ttu-id="00e3f-124">説明</span><span class="sxs-lookup"><span data-stu-id="00e3f-124">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="00e3f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="00e3f-125">Authorization</span></span>  | <span data-ttu-id="00e3f-126">string</span><span class="sxs-lookup"><span data-stu-id="00e3f-126">string</span></span> | <span data-ttu-id="00e3f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="00e3f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="00e3f-129">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="00e3f-129">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="00e3f-130">string</span><span class="sxs-lookup"><span data-stu-id="00e3f-130">string</span></span> | <span data-ttu-id="00e3f-131">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="00e3f-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="00e3f-132">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="00e3f-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="00e3f-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="00e3f-133">Optional.</span></span> |
| <span data-ttu-id="00e3f-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="00e3f-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="00e3f-135">string</span><span class="sxs-lookup"><span data-stu-id="00e3f-135">string</span></span> | <span data-ttu-id="00e3f-136">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="00e3f-136">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="00e3f-137">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="00e3f-137">Values can be "text" or "html".</span></span> <span data-ttu-id="00e3f-138">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="00e3f-138">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="00e3f-139">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="00e3f-139">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="00e3f-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="00e3f-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00e3f-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="00e3f-141">Request body</span></span>
<span data-ttu-id="00e3f-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="00e3f-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00e3f-143">応答</span><span class="sxs-lookup"><span data-stu-id="00e3f-143">Response</span></span>
<span data-ttu-id="00e3f-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="00e3f-144">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00e3f-145">例</span><span class="sxs-lookup"><span data-stu-id="00e3f-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="00e3f-146">要求</span><span class="sxs-lookup"><span data-stu-id="00e3f-146">Request</span></span>
<span data-ttu-id="00e3f-147">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00e3f-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="00e3f-148">応答</span><span class="sxs-lookup"><span data-stu-id="00e3f-148">Response</span></span>
<span data-ttu-id="00e3f-149">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00e3f-149">The following is an example of the response.</span></span>
><span data-ttu-id="00e3f-150">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="00e3f-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="00e3f-151">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="00e3f-151">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
