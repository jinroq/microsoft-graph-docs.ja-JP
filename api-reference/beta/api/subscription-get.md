---
title: サブスクリプションを取得する
description: サブスクリプションのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c7dd20810cd9fdacec697345d42690f85bc3b8b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522365"
---
# <a name="get-subscription"></a><span data-ttu-id="6345f-103">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="6345f-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6345f-104">サブスクリプションのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="6345f-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="6345f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6345f-105">Permissions</span></span>

<span data-ttu-id="6345f-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6345f-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6345f-108">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="6345f-108">Resource type / Item</span></span>        | <span data-ttu-id="6345f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6345f-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="6345f-110">連絡先</span><span class="sxs-lookup"><span data-stu-id="6345f-110">Contacts</span></span>                    | <span data-ttu-id="6345f-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6345f-111">Contacts.Read</span></span>       |
| <span data-ttu-id="6345f-112">スレッド</span><span class="sxs-lookup"><span data-stu-id="6345f-112">Conversations</span></span>               | <span data-ttu-id="6345f-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6345f-113">Group.Read.All</span></span>      |
| <span data-ttu-id="6345f-114">イベント</span><span class="sxs-lookup"><span data-stu-id="6345f-114">Events</span></span>                      | <span data-ttu-id="6345f-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6345f-115">Calendars.Read</span></span>      |
| <span data-ttu-id="6345f-116">メッセージ</span><span class="sxs-lookup"><span data-stu-id="6345f-116">Messages</span></span>                    | <span data-ttu-id="6345f-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6345f-117">Mail.Read</span></span>           |
| <span data-ttu-id="6345f-118">グループ</span><span class="sxs-lookup"><span data-stu-id="6345f-118">Groups</span></span>                      | <span data-ttu-id="6345f-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6345f-119">Group.Read.All</span></span>      |
| <span data-ttu-id="6345f-120">ユーザー</span><span class="sxs-lookup"><span data-stu-id="6345f-120">Users</span></span>                       | <span data-ttu-id="6345f-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6345f-121">User.Read.All</span></span>       |
| <span data-ttu-id="6345f-122">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="6345f-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="6345f-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6345f-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="6345f-124">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="6345f-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="6345f-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6345f-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="6345f-126">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="6345f-126">Security alert</span></span>              | <span data-ttu-id="6345f-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6345f-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="6345f-128">***注:***/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="6345f-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="6345f-129">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6345f-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="6345f-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6345f-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6345f-131">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6345f-131">Optional query parameters</span></span>

<span data-ttu-id="6345f-132">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6345f-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6345f-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6345f-133">Request headers</span></span>

| <span data-ttu-id="6345f-134">名前</span><span class="sxs-lookup"><span data-stu-id="6345f-134">Name</span></span>       | <span data-ttu-id="6345f-135">型</span><span class="sxs-lookup"><span data-stu-id="6345f-135">Type</span></span> | <span data-ttu-id="6345f-136">説明</span><span class="sxs-lookup"><span data-stu-id="6345f-136">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="6345f-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="6345f-137">Authorization</span></span>  | <span data-ttu-id="6345f-138">string</span><span class="sxs-lookup"><span data-stu-id="6345f-138">string</span></span>  | <span data-ttu-id="6345f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6345f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6345f-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="6345f-141">Request body</span></span>

<span data-ttu-id="6345f-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6345f-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6345f-143">応答</span><span class="sxs-lookup"><span data-stu-id="6345f-143">Response</span></span>

<span data-ttu-id="6345f-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6345f-144">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6345f-145">例</span><span class="sxs-lookup"><span data-stu-id="6345f-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6345f-146">要求</span><span class="sxs-lookup"><span data-stu-id="6345f-146">Request</span></span>

<span data-ttu-id="6345f-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6345f-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="6345f-148">応答</span><span class="sxs-lookup"><span data-stu-id="6345f-148">Response</span></span>

<span data-ttu-id="6345f-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6345f-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
