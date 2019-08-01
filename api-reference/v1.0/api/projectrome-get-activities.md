---
title: ユーザーアクティビティを取得する
description: 特定のユーザーのアクティビティを取得します。 **最近**の OData 関数とは異なり、履歴のないアクティビティは返されます。 アクセス許可 UserActivity は、アプリケーションによって作成されたアクティビティのみが返されるように、応答に特別なフィルター処理を適用します。 このサーバー側のフィルタリングは、ユーザーが特にアクティブで、その他のアプリケーションがより新しいアクティビティを作成した場合に、空のページになる可能性があります。 アプリケーションのアクティビティを取得するには、 **Nextlink**プロパティを使用して改ページにします。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: 1a3dad16f96f8b16618a1916bcccf6cf67eb95ff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975887"
---
# <a name="get-user-activities"></a><span data-ttu-id="234c8-107">ユーザーアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="234c8-107">Get user activities</span></span>

<span data-ttu-id="234c8-108">特定のユーザーのアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="234c8-108">Get activities for a given user.</span></span> <span data-ttu-id="234c8-109">**最近**の OData 関数とは異なり、履歴のないアクティビティは返されます。</span><span class="sxs-lookup"><span data-stu-id="234c8-109">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="234c8-110">アクセス許可 UserActivity は、アプリケーションによって作成されたアクティビティのみが返されるように、応答に特別なフィルター処理を適用します。</span><span class="sxs-lookup"><span data-stu-id="234c8-110">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="234c8-111">このサーバー側のフィルタリングは、ユーザーが特にアクティブで、その他のアプリケーションがより新しいアクティビティを作成した場合に、空のページになる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="234c8-111">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="234c8-112">アプリケーションのアクティビティを取得するには、 **Nextlink**プロパティを使用して改ページにします。</span><span class="sxs-lookup"><span data-stu-id="234c8-112">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="234c8-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="234c8-113">Permissions</span></span>

<span data-ttu-id="234c8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="234c8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="234c8-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="234c8-116">Permission type</span></span>      | <span data-ttu-id="234c8-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="234c8-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="234c8-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="234c8-118">Delegated (work or school account)</span></span> | <span data-ttu-id="234c8-119">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="234c8-119">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="234c8-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="234c8-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="234c8-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="234c8-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="234c8-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="234c8-122">Application</span></span> | <span data-ttu-id="234c8-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="234c8-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="234c8-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="234c8-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="234c8-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="234c8-125">Optional query parameters</span></span>

<span data-ttu-id="234c8-126">このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="234c8-126">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="234c8-127">次のクエリパラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="234c8-127">The following query parameters are supported:</span></span>

- <span data-ttu-id="234c8-128">**履歴項目**ナビゲーションプロパティの $expand。</span><span class="sxs-lookup"><span data-stu-id="234c8-128">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="234c8-129">ページ間でのアイテムの最大数を制限する $top。</span><span class="sxs-lookup"><span data-stu-id="234c8-129">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="234c8-130">**lastModifiedDateTime**プロパティを使用して、アクティビティまたは**履歴アイテム**(展開されている場合) のどちらかを $filter します。</span><span class="sxs-lookup"><span data-stu-id="234c8-130">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="234c8-131">次に、URL エンコードを使用してサポートされているクエリの例をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="234c8-131">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="234c8-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="234c8-132">Request headers</span></span>

|<span data-ttu-id="234c8-133">名前</span><span class="sxs-lookup"><span data-stu-id="234c8-133">Name</span></span> | <span data-ttu-id="234c8-134">型</span><span class="sxs-lookup"><span data-stu-id="234c8-134">Type</span></span> | <span data-ttu-id="234c8-135">説明</span><span class="sxs-lookup"><span data-stu-id="234c8-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="234c8-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="234c8-136">Authorization</span></span> | <span data-ttu-id="234c8-137">string</span><span class="sxs-lookup"><span data-stu-id="234c8-137">string</span></span> | <span data-ttu-id="234c8-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="234c8-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="234c8-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="234c8-140">Request body</span></span>

<span data-ttu-id="234c8-141">要求本文がありません。</span><span class="sxs-lookup"><span data-stu-id="234c8-141">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="234c8-142">応答</span><span class="sxs-lookup"><span data-stu-id="234c8-142">Response</span></span>

<span data-ttu-id="234c8-143">成功した場合、このメソッド`200 OK`はアプリケーションに対するユーザーのアクティビティと共に応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="234c8-143">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="234c8-144">例</span><span class="sxs-lookup"><span data-stu-id="234c8-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="234c8-145">要求</span><span class="sxs-lookup"><span data-stu-id="234c8-145">Request</span></span>

<span data-ttu-id="234c8-146">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="234c8-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="234c8-147">応答</span><span class="sxs-lookup"><span data-stu-id="234c8-147">Response</span></span>

<span data-ttu-id="234c8-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="234c8-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
