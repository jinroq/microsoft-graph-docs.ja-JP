---
title: サブスクリプションを更新する
description: サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 19355ff8acbcdade689b140abca63e8d9885e3fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512781"
---
# <a name="update-subscription"></a><span data-ttu-id="32497-103">サブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="32497-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32497-104">サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。</span><span class="sxs-lookup"><span data-stu-id="32497-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="32497-105">サブスクリプションの有効期限後、時間の長さをリソースの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="32497-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="32497-106">通知の欠落を回避するには、するためにアプリケーションの有効期限前に、サブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="32497-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="32497-107">各リソースの種類のサブスクリプションの最大長の[サブスクリプション](../resources/subscription.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32497-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="32497-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32497-108">Permissions</span></span>

<span data-ttu-id="32497-p102">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32497-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32497-111">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="32497-111">Resource type / Item</span></span>        | <span data-ttu-id="32497-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32497-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="32497-113">連絡先</span><span class="sxs-lookup"><span data-stu-id="32497-113">Contacts</span></span>                    | <span data-ttu-id="32497-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="32497-114">Contacts.Read</span></span>       |
| <span data-ttu-id="32497-115">スレッド</span><span class="sxs-lookup"><span data-stu-id="32497-115">Conversations</span></span>               | <span data-ttu-id="32497-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="32497-116">Group.Read.All</span></span>      |
| <span data-ttu-id="32497-117">イベント</span><span class="sxs-lookup"><span data-stu-id="32497-117">Events</span></span>                      | <span data-ttu-id="32497-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="32497-118">Calendars.Read</span></span>      |
| <span data-ttu-id="32497-119">メッセージ</span><span class="sxs-lookup"><span data-stu-id="32497-119">Messages</span></span>                    | <span data-ttu-id="32497-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="32497-120">Mail.Read</span></span>           |
| <span data-ttu-id="32497-121">グループ</span><span class="sxs-lookup"><span data-stu-id="32497-121">Groups</span></span>                      | <span data-ttu-id="32497-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="32497-122">Group.Read.All</span></span>      |
| <span data-ttu-id="32497-123">ユーザー</span><span class="sxs-lookup"><span data-stu-id="32497-123">Users</span></span>                       | <span data-ttu-id="32497-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="32497-124">User.Read.All</span></span>       |
| <span data-ttu-id="32497-125">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="32497-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="32497-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32497-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="32497-127">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="32497-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="32497-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32497-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="32497-129">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="32497-129">Security alert</span></span>               | <span data-ttu-id="32497-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32497-130">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="32497-131">***注:***/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="32497-131">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="32497-132">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32497-132">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="32497-133">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32497-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="32497-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32497-134">Request headers</span></span>

| <span data-ttu-id="32497-135">名前</span><span class="sxs-lookup"><span data-stu-id="32497-135">Name</span></span>       | <span data-ttu-id="32497-136">型</span><span class="sxs-lookup"><span data-stu-id="32497-136">Type</span></span> | <span data-ttu-id="32497-137">説明</span><span class="sxs-lookup"><span data-stu-id="32497-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="32497-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="32497-138">Authorization</span></span>  | <span data-ttu-id="32497-139">string</span><span class="sxs-lookup"><span data-stu-id="32497-139">string</span></span>  | <span data-ttu-id="32497-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32497-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="32497-142">応答</span><span class="sxs-lookup"><span data-stu-id="32497-142">Response</span></span>

<span data-ttu-id="32497-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="32497-143">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32497-144">例</span><span class="sxs-lookup"><span data-stu-id="32497-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="32497-145">要求</span><span class="sxs-lookup"><span data-stu-id="32497-145">Request</span></span>

<span data-ttu-id="32497-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32497-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="32497-147">応答</span><span class="sxs-lookup"><span data-stu-id="32497-147">Response</span></span>

<span data-ttu-id="32497-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="32497-148">Here is an example of the response.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
