---
title: サブスクリプションを取得する
description: サブスクリプションのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 0feb4ffd49099eabb92e5519b25233100f2acbe5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846838"
---
# <a name="get-subscription"></a><span data-ttu-id="adbf1-103">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="adbf1-103">Get subscription</span></span>

> <span data-ttu-id="adbf1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="adbf1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adbf1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adbf1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="adbf1-106">サブスクリプションのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="adbf1-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="adbf1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="adbf1-107">Permissions</span></span>

<span data-ttu-id="adbf1-p102">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="adbf1-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adbf1-110">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="adbf1-110">Resource type / Item</span></span>        | <span data-ttu-id="adbf1-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="adbf1-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="adbf1-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="adbf1-112">Contacts</span></span>                    | <span data-ttu-id="adbf1-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="adbf1-113">Contacts.Read</span></span>       |
| <span data-ttu-id="adbf1-114">スレッド</span><span class="sxs-lookup"><span data-stu-id="adbf1-114">Conversations</span></span>               | <span data-ttu-id="adbf1-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="adbf1-115">Group.Read.All</span></span>      |
| <span data-ttu-id="adbf1-116">イベント</span><span class="sxs-lookup"><span data-stu-id="adbf1-116">Events</span></span>                      | <span data-ttu-id="adbf1-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="adbf1-117">Calendars.Read</span></span>      |
| <span data-ttu-id="adbf1-118">メッセージ</span><span class="sxs-lookup"><span data-stu-id="adbf1-118">Messages</span></span>                    | <span data-ttu-id="adbf1-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="adbf1-119">Mail.Read</span></span>           |
| <span data-ttu-id="adbf1-120">グループ</span><span class="sxs-lookup"><span data-stu-id="adbf1-120">Groups</span></span>                      | <span data-ttu-id="adbf1-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="adbf1-121">Group.Read.All</span></span>      |
| <span data-ttu-id="adbf1-122">ユーザー</span><span class="sxs-lookup"><span data-stu-id="adbf1-122">Users</span></span>                       | <span data-ttu-id="adbf1-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="adbf1-123">User.Read.All</span></span>       |
| <span data-ttu-id="adbf1-124">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="adbf1-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="adbf1-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="adbf1-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="adbf1-126">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="adbf1-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="adbf1-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbf1-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="adbf1-128">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="adbf1-128">Security alert</span></span>              | <span data-ttu-id="adbf1-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbf1-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="adbf1-130">***注:***/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="adbf1-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="adbf1-131">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adbf1-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="adbf1-132">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="adbf1-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adbf1-133">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="adbf1-133">Optional query parameters</span></span>

<span data-ttu-id="adbf1-134">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="adbf1-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="adbf1-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="adbf1-135">Request headers</span></span>

| <span data-ttu-id="adbf1-136">名前</span><span class="sxs-lookup"><span data-stu-id="adbf1-136">Name</span></span>       | <span data-ttu-id="adbf1-137">種類</span><span class="sxs-lookup"><span data-stu-id="adbf1-137">Type</span></span> | <span data-ttu-id="adbf1-138">説明</span><span class="sxs-lookup"><span data-stu-id="adbf1-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="adbf1-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="adbf1-139">Authorization</span></span>  | <span data-ttu-id="adbf1-140">string</span><span class="sxs-lookup"><span data-stu-id="adbf1-140">string</span></span>  | <span data-ttu-id="adbf1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="adbf1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adbf1-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="adbf1-143">Request body</span></span>

<span data-ttu-id="adbf1-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="adbf1-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adbf1-145">応答</span><span class="sxs-lookup"><span data-stu-id="adbf1-145">Response</span></span>

<span data-ttu-id="adbf1-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="adbf1-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adbf1-147">例</span><span class="sxs-lookup"><span data-stu-id="adbf1-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="adbf1-148">要求</span><span class="sxs-lookup"><span data-stu-id="adbf1-148">Request</span></span>

<span data-ttu-id="adbf1-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="adbf1-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="adbf1-150">応答</span><span class="sxs-lookup"><span data-stu-id="adbf1-150">Response</span></span>

<span data-ttu-id="adbf1-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="adbf1-151">Here is an example of the response.</span></span>
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
