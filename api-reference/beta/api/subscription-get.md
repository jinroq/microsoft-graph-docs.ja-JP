---
title: サブスクリプションを取得する
description: サブスクリプションのプロパティとリレーションシップを取得します。
ms.openlocfilehash: 5694015fe7e8cbf87b5d62f7ae4af35d1773532b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069664"
---
# <a name="get-subscription"></a><span data-ttu-id="41ea2-103">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="41ea2-103">Get subscription</span></span>

> <span data-ttu-id="41ea2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="41ea2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41ea2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41ea2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41ea2-106">サブスクリプションのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="41ea2-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="41ea2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41ea2-107">Permissions</span></span>

<span data-ttu-id="41ea2-p102">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41ea2-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41ea2-110">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="41ea2-110">Resource type / Item</span></span>        | <span data-ttu-id="41ea2-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41ea2-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="41ea2-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="41ea2-112">Contacts</span></span>                    | <span data-ttu-id="41ea2-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="41ea2-113">Contacts.Read</span></span>       |
| <span data-ttu-id="41ea2-114">スレッド</span><span class="sxs-lookup"><span data-stu-id="41ea2-114">Conversations</span></span>               | <span data-ttu-id="41ea2-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="41ea2-115">Group.Read.All</span></span>      |
| <span data-ttu-id="41ea2-116">イベント</span><span class="sxs-lookup"><span data-stu-id="41ea2-116">Events</span></span>                      | <span data-ttu-id="41ea2-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="41ea2-117">Calendars.Read</span></span>      |
| <span data-ttu-id="41ea2-118">メッセージ</span><span class="sxs-lookup"><span data-stu-id="41ea2-118">Messages</span></span>                    | <span data-ttu-id="41ea2-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="41ea2-119">Mail.Read</span></span>           |
| <span data-ttu-id="41ea2-120">Groups</span><span class="sxs-lookup"><span data-stu-id="41ea2-120">Groups</span></span>                      | <span data-ttu-id="41ea2-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="41ea2-121">Group.Read.All</span></span>      |
| <span data-ttu-id="41ea2-122">Users</span><span class="sxs-lookup"><span data-stu-id="41ea2-122">Users</span></span>                       | <span data-ttu-id="41ea2-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="41ea2-123">User.Read.All</span></span>       |
| <span data-ttu-id="41ea2-124">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="41ea2-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="41ea2-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41ea2-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="41ea2-126">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="41ea2-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="41ea2-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41ea2-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="41ea2-128">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="41ea2-128">Security alert</span></span>              | <span data-ttu-id="41ea2-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41ea2-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="41ea2-130">***注:***/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="41ea2-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="41ea2-131">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41ea2-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="41ea2-132">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41ea2-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41ea2-133">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="41ea2-133">Optional query parameters</span></span>

<span data-ttu-id="41ea2-134">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="41ea2-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41ea2-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41ea2-135">Request headers</span></span>

| <span data-ttu-id="41ea2-136">名前</span><span class="sxs-lookup"><span data-stu-id="41ea2-136">Name</span></span>       | <span data-ttu-id="41ea2-137">型</span><span class="sxs-lookup"><span data-stu-id="41ea2-137">Type</span></span> | <span data-ttu-id="41ea2-138">説明</span><span class="sxs-lookup"><span data-stu-id="41ea2-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="41ea2-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="41ea2-139">Authorization</span></span>  | <span data-ttu-id="41ea2-140">string</span><span class="sxs-lookup"><span data-stu-id="41ea2-140">string</span></span>  | <span data-ttu-id="41ea2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="41ea2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41ea2-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="41ea2-143">Request body</span></span>

<span data-ttu-id="41ea2-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="41ea2-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41ea2-145">応答</span><span class="sxs-lookup"><span data-stu-id="41ea2-145">Response</span></span>

<span data-ttu-id="41ea2-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="41ea2-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41ea2-147">例</span><span class="sxs-lookup"><span data-stu-id="41ea2-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="41ea2-148">要求</span><span class="sxs-lookup"><span data-stu-id="41ea2-148">Request</span></span>

<span data-ttu-id="41ea2-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41ea2-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="41ea2-150">応答</span><span class="sxs-lookup"><span data-stu-id="41ea2-150">Response</span></span>

<span data-ttu-id="41ea2-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="41ea2-151">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
