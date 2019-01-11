---
title: サブスクリプションを更新する
description: サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。
localization_priority: Normal
ms.openlocfilehash: 63bcf8f4084053356819601cd6306ad3ff5238c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836121"
---
# <a name="update-subscription"></a><span data-ttu-id="0a032-103">サブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="0a032-103">Update subscription</span></span>

> <span data-ttu-id="0a032-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a032-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a032-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a032-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a032-106">サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。</span><span class="sxs-lookup"><span data-stu-id="0a032-106">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="0a032-107">サブスクリプションの有効期限後、時間の長さをリソースの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="0a032-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="0a032-108">通知の欠落を回避するには、するためにアプリケーションの有効期限前に、サブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a032-108">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="0a032-109">各リソースの種類のサブスクリプションの最大長の[サブスクリプション](../resources/subscription.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a032-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a032-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a032-110">Permissions</span></span>

<span data-ttu-id="0a032-p103">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a032-p103">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a032-113">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="0a032-113">Resource type / Item</span></span>        | <span data-ttu-id="0a032-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a032-114">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="0a032-115">連絡先</span><span class="sxs-lookup"><span data-stu-id="0a032-115">Contacts</span></span>                    | <span data-ttu-id="0a032-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0a032-116">Contacts.Read</span></span>       |
| <span data-ttu-id="0a032-117">スレッド</span><span class="sxs-lookup"><span data-stu-id="0a032-117">Conversations</span></span>               | <span data-ttu-id="0a032-118">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a032-118">Group.Read.All</span></span>      |
| <span data-ttu-id="0a032-119">イベント</span><span class="sxs-lookup"><span data-stu-id="0a032-119">Events</span></span>                      | <span data-ttu-id="0a032-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0a032-120">Calendars.Read</span></span>      |
| <span data-ttu-id="0a032-121">メッセージ</span><span class="sxs-lookup"><span data-stu-id="0a032-121">Messages</span></span>                    | <span data-ttu-id="0a032-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0a032-122">Mail.Read</span></span>           |
| <span data-ttu-id="0a032-123">グループ</span><span class="sxs-lookup"><span data-stu-id="0a032-123">Groups</span></span>                      | <span data-ttu-id="0a032-124">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a032-124">Group.Read.All</span></span>      |
| <span data-ttu-id="0a032-125">ユーザー</span><span class="sxs-lookup"><span data-stu-id="0a032-125">Users</span></span>                       | <span data-ttu-id="0a032-126">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a032-126">User.Read.All</span></span>       |
| <span data-ttu-id="0a032-127">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="0a032-127">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="0a032-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a032-128">Files.ReadWrite</span></span>     |
| <span data-ttu-id="0a032-129">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="0a032-129">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="0a032-130">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a032-130">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="0a032-131">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="0a032-131">Security alert</span></span>               | <span data-ttu-id="0a032-132">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a032-132">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="0a032-133">***注:***/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="0a032-133">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="0a032-134">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a032-134">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="0a032-135">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a032-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0a032-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a032-136">Request headers</span></span>

| <span data-ttu-id="0a032-137">名前</span><span class="sxs-lookup"><span data-stu-id="0a032-137">Name</span></span>       | <span data-ttu-id="0a032-138">種類</span><span class="sxs-lookup"><span data-stu-id="0a032-138">Type</span></span> | <span data-ttu-id="0a032-139">説明</span><span class="sxs-lookup"><span data-stu-id="0a032-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0a032-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a032-140">Authorization</span></span>  | <span data-ttu-id="0a032-141">string</span><span class="sxs-lookup"><span data-stu-id="0a032-141">string</span></span>  | <span data-ttu-id="0a032-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a032-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0a032-144">応答</span><span class="sxs-lookup"><span data-stu-id="0a032-144">Response</span></span>

<span data-ttu-id="0a032-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0a032-145">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a032-146">例</span><span class="sxs-lookup"><span data-stu-id="0a032-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0a032-147">要求</span><span class="sxs-lookup"><span data-stu-id="0a032-147">Request</span></span>

<span data-ttu-id="0a032-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a032-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="0a032-149">応答</span><span class="sxs-lookup"><span data-stu-id="0a032-149">Response</span></span>

<span data-ttu-id="0a032-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0a032-150">Here is an example of the response.</span></span>
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
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
