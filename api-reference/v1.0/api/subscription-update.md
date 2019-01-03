---
title: サブスクリプションを更新する
description: サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。
ms.openlocfilehash: 75b01a72310f9e9d227f4d185d13f6ee7dfdf835
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021304"
---
# <a name="update-subscription"></a><span data-ttu-id="6e770-103">サブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="6e770-103">Update subscription</span></span>

<span data-ttu-id="6e770-104">サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。</span><span class="sxs-lookup"><span data-stu-id="6e770-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="6e770-105">サブスクリプションの有効期限後、時間の長さをリソースの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="6e770-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="6e770-106">通知の欠落を回避するには、するためにアプリケーションの有効期限前に、サブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e770-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="6e770-107">各リソースの種類のサブスクリプションの最大長の[サブスクリプション](../resources/subscription.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e770-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e770-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e770-108">Permissions</span></span>

<span data-ttu-id="6e770-p102">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e770-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e770-111">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="6e770-111">Resource type / Item</span></span>        | <span data-ttu-id="6e770-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e770-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="6e770-113">連絡先</span><span class="sxs-lookup"><span data-stu-id="6e770-113">Contacts</span></span>                    | <span data-ttu-id="6e770-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6e770-114">Contacts.Read</span></span>       |
| <span data-ttu-id="6e770-115">スレッド</span><span class="sxs-lookup"><span data-stu-id="6e770-115">Conversations</span></span>               | <span data-ttu-id="6e770-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e770-116">Group.Read.All</span></span>      |
| <span data-ttu-id="6e770-117">イベント</span><span class="sxs-lookup"><span data-stu-id="6e770-117">Events</span></span>                      | <span data-ttu-id="6e770-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e770-118">Calendars.Read</span></span>      |
| <span data-ttu-id="6e770-119">メッセージ</span><span class="sxs-lookup"><span data-stu-id="6e770-119">Messages</span></span>                    | <span data-ttu-id="6e770-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6e770-120">Mail.Read</span></span>           |
| <span data-ttu-id="6e770-121">Groups</span><span class="sxs-lookup"><span data-stu-id="6e770-121">Groups</span></span>                      | <span data-ttu-id="6e770-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e770-122">Group.Read.All</span></span>      |
| <span data-ttu-id="6e770-123">Users</span><span class="sxs-lookup"><span data-stu-id="6e770-123">Users</span></span>                       | <span data-ttu-id="6e770-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e770-124">User.Read.All</span></span>       |
| <span data-ttu-id="6e770-125">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="6e770-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="6e770-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e770-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="6e770-127">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="6e770-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="6e770-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e770-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="6e770-129">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="6e770-129">Security alert</span></span>| <span data-ttu-id="6e770-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e770-130">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e770-131">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e770-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6e770-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e770-132">Request headers</span></span>

| <span data-ttu-id="6e770-133">名前</span><span class="sxs-lookup"><span data-stu-id="6e770-133">Name</span></span>       | <span data-ttu-id="6e770-134">型</span><span class="sxs-lookup"><span data-stu-id="6e770-134">Type</span></span> | <span data-ttu-id="6e770-135">説明</span><span class="sxs-lookup"><span data-stu-id="6e770-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6e770-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e770-136">Authorization</span></span>  | <span data-ttu-id="6e770-137">string</span><span class="sxs-lookup"><span data-stu-id="6e770-137">string</span></span>  | <span data-ttu-id="6e770-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e770-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6e770-140">応答</span><span class="sxs-lookup"><span data-stu-id="6e770-140">Response</span></span>

<span data-ttu-id="6e770-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6e770-141">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e770-142">例</span><span class="sxs-lookup"><span data-stu-id="6e770-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6e770-143">要求</span><span class="sxs-lookup"><span data-stu-id="6e770-143">Request</span></span>

<span data-ttu-id="6e770-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6e770-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="6e770-145">応答</span><span class="sxs-lookup"><span data-stu-id="6e770-145">Response</span></span>

<span data-ttu-id="6e770-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6e770-146">Here is an example of the response.</span></span>
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
  "clientState":"subscription-identifier",
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