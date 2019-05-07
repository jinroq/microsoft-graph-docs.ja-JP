---
title: 最近のユーザーアクティビティを取得する
description: " トレース. サービスは最新の履歴項目を照会してから、関連するアクティビティを抽出します。 アクティビティは、**履歴アイテム**の最新の**lastModified**に従って並べ替えられます。 これは、**履歴アイテム**のないアクティビティは応答に含まれないことを意味します。 また、アプリケーションによって作成されたアクティビティのみが返されるように、アプリのアクセス許可は、応答に特別なフィルター処理も適用します。 このサーバー側のフィルタリングは、ユーザーが特にアクティブで、その他のアプリケーションがより新しいアクティビティを作成した場合に、空のページになる可能性があります。 アプリケーションのアクティビティを取得するには、 **Nextlink**プロパティを使用して改ページにします。"
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 709723dfb728c169c8b596675dc26308dd60dac5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608393"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="0b07b-109">最近のユーザーアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="0b07b-109">Get recent user activities</span></span>

<span data-ttu-id="0b07b-110">特定のユーザーの最近のアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="0b07b-110">Get recent activities for a given user.</span></span> <span data-ttu-id="0b07b-111">この OData 関数には、"最近使用された" API のように動作するようにするための既定の動作がいくつか含まれています。</span><span class="sxs-lookup"><span data-stu-id="0b07b-111">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="0b07b-112">サービスは最新の[履歴項目](../resources/projectrome-historyitem.md)を照会してから、関連するアクティビティを抽出します。</span><span class="sxs-lookup"><span data-stu-id="0b07b-112">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="0b07b-113">アクティビティは、**履歴アイテム**の最新の**lastModified**に従って並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="0b07b-113">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="0b07b-114">これは、**履歴アイテム**のないアクティビティは応答に含まれないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="0b07b-114">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="0b07b-115">また、アプリケーションによって作成されたアクティビティのみが返されるように、アプリのアクセス許可は、応答に特別なフィルター処理も適用します。</span><span class="sxs-lookup"><span data-stu-id="0b07b-115">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="0b07b-116">このサーバー側のフィルタリングは、ユーザーが特にアクティブで、その他のアプリケーションがより新しいアクティビティを作成した場合に、空のページになる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0b07b-116">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="0b07b-117">アプリケーションのアクティビティを取得するには、 **Nextlink**プロパティを使用して改ページにします。</span><span class="sxs-lookup"><span data-stu-id="0b07b-117">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b07b-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0b07b-118">Permissions</span></span>

<span data-ttu-id="0b07b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b07b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b07b-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b07b-121">Permission type</span></span>      | <span data-ttu-id="0b07b-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b07b-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b07b-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b07b-123">Delegated (work or school account)</span></span> | <span data-ttu-id="0b07b-124">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="0b07b-124">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="0b07b-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b07b-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b07b-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="0b07b-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="0b07b-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b07b-127">Application</span></span> | <span data-ttu-id="0b07b-128">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b07b-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b07b-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b07b-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b07b-130">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0b07b-130">Optional query parameters</span></span>

<span data-ttu-id="0b07b-131">このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0b07b-131">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="0b07b-132">次のクエリパラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0b07b-132">The following query parameters are supported:</span></span>

- <span data-ttu-id="0b07b-133">**履歴項目**ナビゲーションプロパティの $expand。</span><span class="sxs-lookup"><span data-stu-id="0b07b-133">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="0b07b-134">ページ間でのアイテムの最大数を制限する $top。</span><span class="sxs-lookup"><span data-stu-id="0b07b-134">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="0b07b-135">**lastModifiedDateTime**プロパティを使用して、**アクティビティ**または**履歴アイテム**(展開されている場合) のどちらかを $filter します。</span><span class="sxs-lookup"><span data-stu-id="0b07b-135">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="0b07b-136">次に、URL エンコードでサポートされているクエリの例をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="0b07b-136">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="0b07b-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b07b-137">Request headers</span></span>

|<span data-ttu-id="0b07b-138">名前</span><span class="sxs-lookup"><span data-stu-id="0b07b-138">Name</span></span> | <span data-ttu-id="0b07b-139">型</span><span class="sxs-lookup"><span data-stu-id="0b07b-139">Type</span></span> | <span data-ttu-id="0b07b-140">説明</span><span class="sxs-lookup"><span data-stu-id="0b07b-140">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="0b07b-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b07b-141">Authorization</span></span> | <span data-ttu-id="0b07b-142">string</span><span class="sxs-lookup"><span data-stu-id="0b07b-142">string</span></span> | <span data-ttu-id="0b07b-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0b07b-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b07b-145">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b07b-145">Request body</span></span>

<span data-ttu-id="0b07b-146">要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0b07b-146">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="0b07b-147">応答</span><span class="sxs-lookup"><span data-stu-id="0b07b-147">Response</span></span>

<span data-ttu-id="0b07b-148">成功した場合、このメソッド`200 OK`は、アプリケーションのユーザーの最近のアクティビティで応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0b07b-148">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="0b07b-149">例</span><span class="sxs-lookup"><span data-stu-id="0b07b-149">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0b07b-150">要求</span><span class="sxs-lookup"><span data-stu-id="0b07b-150">Request</span></span>

<span data-ttu-id="0b07b-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b07b-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="0b07b-152">応答</span><span class="sxs-lookup"><span data-stu-id="0b07b-152">Response</span></span>

<span data-ttu-id="0b07b-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b07b-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0b07b-154">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="0b07b-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0b07b-155">Visual</span><span class="sxs-lookup"><span data-stu-id="0b07b-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_recent_activities-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b07b-156">Java</span><span class="sxs-lookup"><span data-stu-id="0b07b-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_recent_activities-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/projectrome-get-recent-activities.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/projectrome-get-recent-activities.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members.",

    "Warning: get_recent_activities/container/visualElements/content/$schema:
      Undocumented property '$schema' [String] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/body:
      Undocumented property 'body' [Collection(Object)] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/type:
      Undocumented property 'type' [String] was not expected on resource microsoft.graph.Json."

  ],
  "tocPath": ""
}-->
