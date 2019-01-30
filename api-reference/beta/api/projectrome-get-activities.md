---
title: ユーザー ・ アクティビティを取得します。
description: 特定のユーザーのアクティビティを取得します。 異なり、**最近使用した**OData 機能、履歴のない活動が返されます。 アクセス許可 UserActivity.ReadWrite.CreatedByApp はフィルターを適用余分な応答に、アプリケーションによって作成された活動のみが返されるようにします。 このサーバー側のフィルター処理が発生空のページでユーザーが特に作業中であり、他のアプリケーションが最新の活動を作成します。 アプリケーションのアクティビティを取得するには、改ページ調整**nextLink**プロパティを使用します。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 96830c2698a079018368ce907ca39d4cda0f63fe
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643462"
---
# <a name="get-user-activities"></a><span data-ttu-id="1d5bd-107">ユーザー ・ アクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-107">Get user activities</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d5bd-108">特定のユーザーのアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-108">Get activities for a given user.</span></span> <span data-ttu-id="1d5bd-109">異なり、**最近使用した**OData 機能、履歴のない活動が返されます。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-109">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="1d5bd-110">アクセス許可 UserActivity.ReadWrite.CreatedByApp はフィルターを適用余分な応答に、アプリケーションによって作成された活動のみが返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-110">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="1d5bd-111">このサーバー側のフィルター処理が発生空のページでユーザーが特に作業中であり、他のアプリケーションが最新の活動を作成します。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-111">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="1d5bd-112">アプリケーションのアクティビティを取得するには、改ページ調整**nextLink**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-112">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d5bd-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d5bd-113">Permissions</span></span>

<span data-ttu-id="1d5bd-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d5bd-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d5bd-116">Permission type</span></span>      | <span data-ttu-id="1d5bd-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d5bd-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d5bd-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d5bd-118">Delegated (work or school account)</span></span> | <span data-ttu-id="1d5bd-119">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1d5bd-119">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1d5bd-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d5bd-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d5bd-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1d5bd-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1d5bd-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d5bd-122">Application</span></span> | <span data-ttu-id="1d5bd-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d5bd-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d5bd-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d5bd-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1d5bd-125">Optional query parameters</span></span>

<span data-ttu-id="1d5bd-126">このメソッドは、応答をカスタマイズするためにいくつかの[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-126">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="1d5bd-127">次のクエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-127">The following query parameters are supported:</span></span>

- <span data-ttu-id="1d5bd-128">$ は、 **historyItems**のナビゲーション プロパティを展開します。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-128">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="1d5bd-129">ページ間でのアイテムの最大数を制限する $top。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-129">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="1d5bd-130">**アクティビティ**または**historyItems**、展開されている場合のいずれかの**lastModifiedDateTime**プロパティで $filter。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-130">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="1d5bd-131">次に、URL エンコードがサポートされているクエリの例を示します。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-131">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="1d5bd-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d5bd-132">Request headers</span></span>

|<span data-ttu-id="1d5bd-133">名前</span><span class="sxs-lookup"><span data-stu-id="1d5bd-133">Name</span></span> | <span data-ttu-id="1d5bd-134">型</span><span class="sxs-lookup"><span data-stu-id="1d5bd-134">Type</span></span> | <span data-ttu-id="1d5bd-135">説明</span><span class="sxs-lookup"><span data-stu-id="1d5bd-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1d5bd-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d5bd-136">Authorization</span></span> | <span data-ttu-id="1d5bd-137">string</span><span class="sxs-lookup"><span data-stu-id="1d5bd-137">string</span></span> | <span data-ttu-id="1d5bd-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d5bd-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d5bd-140">Request body</span></span>

<span data-ttu-id="1d5bd-141">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-141">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="1d5bd-142">応答</span><span class="sxs-lookup"><span data-stu-id="1d5bd-142">Response</span></span>

<span data-ttu-id="1d5bd-143">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、アプリケーションのユーザーのアクティビティに応答コード。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-143">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="1d5bd-144">例</span><span class="sxs-lookup"><span data-stu-id="1d5bd-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1d5bd-145">要求</span><span class="sxs-lookup"><span data-stu-id="1d5bd-145">Request</span></span>

<span data-ttu-id="1d5bd-146">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities
```

##### <a name="response"></a><span data-ttu-id="1d5bd-147">応答</span><span class="sxs-lookup"><span data-stu-id="1d5bd-147">Response</span></span>

<span data-ttu-id="1d5bd-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d5bd-148">The following is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-get-activities.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
