---
title: ユーザー ・ アクティビティを取得します。
description: 特定のユーザーのアクティビティを取得します。 異なり、**最近使用した**OData 機能、履歴のない活動が返されます。 アクセス許可 UserActivity.ReadWrite.CreatedByApp はフィルターを適用余分な応答に、アプリケーションによって作成された活動のみが返されるようにします。 このサーバー側のフィルター処理が発生空のページでユーザーが特に作業中であり、他のアプリケーションが最新の活動を作成します。 アプリケーションのアクティビティを取得するには、改ページ調整**nextLink**プロパティを使用します。
localization_priority: Normal
ms.openlocfilehash: 8106d1c2cb740033fd81a21068aba5a15fd1b1b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809374"
---
# <a name="get-user-activities"></a><span data-ttu-id="71cd6-107">ユーザー ・ アクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="71cd6-107">Get user activities</span></span>

> <span data-ttu-id="71cd6-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="71cd6-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71cd6-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71cd6-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71cd6-110">特定のユーザーのアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="71cd6-110">Get activities for a given user.</span></span> <span data-ttu-id="71cd6-111">異なり、**最近使用した**OData 機能、履歴のない活動が返されます。</span><span class="sxs-lookup"><span data-stu-id="71cd6-111">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="71cd6-112">アクセス許可 UserActivity.ReadWrite.CreatedByApp はフィルターを適用余分な応答に、アプリケーションによって作成された活動のみが返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="71cd6-112">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="71cd6-113">このサーバー側のフィルター処理が発生空のページでユーザーが特に作業中であり、他のアプリケーションが最新の活動を作成します。</span><span class="sxs-lookup"><span data-stu-id="71cd6-113">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="71cd6-114">アプリケーションのアクティビティを取得するには、改ページ調整**nextLink**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="71cd6-114">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="71cd6-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="71cd6-115">Permissions</span></span>

<span data-ttu-id="71cd6-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71cd6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71cd6-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71cd6-118">Permission type</span></span>      | <span data-ttu-id="71cd6-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="71cd6-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71cd6-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71cd6-120">Delegated (work or school account)</span></span> | <span data-ttu-id="71cd6-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="71cd6-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="71cd6-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71cd6-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71cd6-123">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="71cd6-123">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="71cd6-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71cd6-124">Application</span></span> | <span data-ttu-id="71cd6-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71cd6-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71cd6-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71cd6-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71cd6-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="71cd6-127">Optional query parameters</span></span>

<span data-ttu-id="71cd6-128">このメソッドは、応答をカスタマイズするためにいくつかの[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="71cd6-128">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="71cd6-129">次のクエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="71cd6-129">The following query parameters are supported:</span></span>

- <span data-ttu-id="71cd6-130">$ は、 **historyItems**のナビゲーション プロパティを展開します。</span><span class="sxs-lookup"><span data-stu-id="71cd6-130">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="71cd6-131">ページ間でのアイテムの最大数を制限する $top。</span><span class="sxs-lookup"><span data-stu-id="71cd6-131">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="71cd6-132">**アクティビティ**または**historyItems**、展開されている場合のいずれかの**lastModifiedDateTime**プロパティで $filter。</span><span class="sxs-lookup"><span data-stu-id="71cd6-132">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="71cd6-133">次に、URL エンコードがサポートされているクエリの例を示します。</span><span class="sxs-lookup"><span data-stu-id="71cd6-133">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="71cd6-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71cd6-134">Request headers</span></span>

|<span data-ttu-id="71cd6-135">名前</span><span class="sxs-lookup"><span data-stu-id="71cd6-135">Name</span></span> | <span data-ttu-id="71cd6-136">種類</span><span class="sxs-lookup"><span data-stu-id="71cd6-136">Type</span></span> | <span data-ttu-id="71cd6-137">説明</span><span class="sxs-lookup"><span data-stu-id="71cd6-137">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="71cd6-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="71cd6-138">Authorization</span></span> | <span data-ttu-id="71cd6-139">string</span><span class="sxs-lookup"><span data-stu-id="71cd6-139">string</span></span> | <span data-ttu-id="71cd6-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="71cd6-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71cd6-142">要求本文</span><span class="sxs-lookup"><span data-stu-id="71cd6-142">Request body</span></span>

<span data-ttu-id="71cd6-143">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="71cd6-143">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="71cd6-144">応答</span><span class="sxs-lookup"><span data-stu-id="71cd6-144">Response</span></span>

<span data-ttu-id="71cd6-145">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、アプリケーションのユーザーのアクティビティに応答コード。</span><span class="sxs-lookup"><span data-stu-id="71cd6-145">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="71cd6-146">例</span><span class="sxs-lookup"><span data-stu-id="71cd6-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71cd6-147">要求</span><span class="sxs-lookup"><span data-stu-id="71cd6-147">Request</span></span>

<span data-ttu-id="71cd6-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="71cd6-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities
```

##### <a name="response"></a><span data-ttu-id="71cd6-149">応答</span><span class="sxs-lookup"><span data-stu-id="71cd6-149">Response</span></span>

<span data-ttu-id="71cd6-150">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="71cd6-150">The following is an example of the response.</span></span>

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
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
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
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
