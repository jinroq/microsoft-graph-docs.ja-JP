---
title: ユーザーの最近の活動を取得します。
description: " API です。 サービスはの最も最近の historyItems では、クエリを実行し、それらの関連の活動を引き出します。 アクティビティは、 **historyItem**で、最新の**lastModified**に従って並べ替えられます。 これは、なしで**historyItems**が応答に含まれないことを意味します。 UserActivity.ReadWrite.CreatedByApp アクセス許可も適用されます応答に追加のフィルタ リング、アプリケーションによって作成された活動のみが返されるようにします。 このサーバー側のフィルター処理が発生空のページでユーザーが特に作業中であり、他のアプリケーションが最新の活動を作成します。 アプリケーションのアクティビティを取得するには、改ページ調整**nextLink**プロパティを使用します。"
localization_priority: Normal
ms.openlocfilehash: 36df29d2000934da417b473235575f5741078dc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819790"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="ab6ef-109">ユーザーの最近の活動を取得します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-109">Get recent user activities</span></span>

> <span data-ttu-id="ab6ef-110">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-110">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab6ef-111">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-111">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab6ef-112">特定のユーザーの最近の活動を取得します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-112">Get recent activities for a given user.</span></span> <span data-ttu-id="ab6ef-113">この OData の関数では、「最近使用した」の API と同様に動作して含まれているいくつか既定動作があります。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-113">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="ab6ef-114">サービスは、最新の[historyItems](../resources/projectrome-historyitem.md)のクエリを実行し、それらの関連の活動を引き出します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-114">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="ab6ef-115">アクティビティは、 **historyItem**で、最新の**lastModified**に従って並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-115">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="ab6ef-116">これは、なしで**historyItems**が応答に含まれないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-116">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="ab6ef-117">UserActivity.ReadWrite.CreatedByApp アクセス許可も適用されます応答に追加のフィルタ リング、アプリケーションによって作成された活動のみが返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-117">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="ab6ef-118">このサーバー側のフィルター処理が発生空のページでユーザーが特に作業中であり、他のアプリケーションが最新の活動を作成します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-118">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="ab6ef-119">アプリケーションのアクティビティを取得するには、改ページ調整**nextLink**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-119">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab6ef-120">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ab6ef-120">Permissions</span></span>

<span data-ttu-id="ab6ef-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab6ef-123">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab6ef-123">Permission type</span></span>      | <span data-ttu-id="ab6ef-124">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab6ef-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab6ef-125">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab6ef-125">Delegated (work or school account)</span></span> | <span data-ttu-id="ab6ef-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ab6ef-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ab6ef-127">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab6ef-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab6ef-128">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ab6ef-128">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ab6ef-129">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab6ef-129">Application</span></span> | <span data-ttu-id="ab6ef-130">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab6ef-131">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab6ef-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab6ef-132">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ab6ef-132">Optional query parameters</span></span>

<span data-ttu-id="ab6ef-133">このメソッドは、応答をカスタマイズするためにいくつかの[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-133">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="ab6ef-134">次のクエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-134">The following query parameters are supported:</span></span>

- <span data-ttu-id="ab6ef-135">$ は、 **historyItems**のナビゲーション プロパティを展開します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-135">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="ab6ef-136">ページ間でのアイテムの最大数を制限する $top。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-136">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="ab6ef-137">**アクティビティ**または**historyItems**、展開されている場合のいずれかの**lastModifiedDateTime**プロパティで $filter。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-137">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="ab6ef-138">URL エンコーディングを使用してクエリがサポートされているいくつかの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-138">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="ab6ef-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab6ef-139">Request headers</span></span>

|<span data-ttu-id="ab6ef-140">名前</span><span class="sxs-lookup"><span data-stu-id="ab6ef-140">Name</span></span> | <span data-ttu-id="ab6ef-141">種類</span><span class="sxs-lookup"><span data-stu-id="ab6ef-141">Type</span></span> | <span data-ttu-id="ab6ef-142">説明</span><span class="sxs-lookup"><span data-stu-id="ab6ef-142">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="ab6ef-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab6ef-143">Authorization</span></span> | <span data-ttu-id="ab6ef-144">string</span><span class="sxs-lookup"><span data-stu-id="ab6ef-144">string</span></span> | <span data-ttu-id="ab6ef-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab6ef-147">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab6ef-147">Request body</span></span>

<span data-ttu-id="ab6ef-148">要求の本体を指定することはしません。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-148">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="ab6ef-149">応答</span><span class="sxs-lookup"><span data-stu-id="ab6ef-149">Response</span></span>

<span data-ttu-id="ab6ef-150">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、アプリケーションのユーザーの最近の活動を使用して応答コード。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-150">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="ab6ef-151">例</span><span class="sxs-lookup"><span data-stu-id="ab6ef-151">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ab6ef-152">要求</span><span class="sxs-lookup"><span data-stu-id="ab6ef-152">Request</span></span>

<span data-ttu-id="ab6ef-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="ab6ef-154">応答</span><span class="sxs-lookup"><span data-stu-id="ab6ef-154">Response</span></span>

<span data-ttu-id="ab6ef-155">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab6ef-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.activity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": "false",
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
