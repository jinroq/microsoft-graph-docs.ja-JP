---
title: サブスクリプションを取得する
description: サブスクリプションのプロパティとリレーションシップを取得します。
ms.openlocfilehash: 62bcb730a5743146113cda30d6dafa022afa4fc1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021663"
---
# <a name="get-subscription"></a><span data-ttu-id="c21e5-103">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="c21e5-103">Get subscription</span></span>

<span data-ttu-id="c21e5-104">サブスクリプションのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="c21e5-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="c21e5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c21e5-105">Permissions</span></span>

<span data-ttu-id="c21e5-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c21e5-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c21e5-108">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="c21e5-108">Resource type / Item</span></span>        | <span data-ttu-id="c21e5-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c21e5-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="c21e5-110">連絡先</span><span class="sxs-lookup"><span data-stu-id="c21e5-110">Contacts</span></span>                    | <span data-ttu-id="c21e5-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c21e5-111">Contacts.Read</span></span>       |
| <span data-ttu-id="c21e5-112">スレッド</span><span class="sxs-lookup"><span data-stu-id="c21e5-112">Conversations</span></span>               | <span data-ttu-id="c21e5-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c21e5-113">Group.Read.All</span></span>      |
| <span data-ttu-id="c21e5-114">イベント</span><span class="sxs-lookup"><span data-stu-id="c21e5-114">Events</span></span>                      | <span data-ttu-id="c21e5-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c21e5-115">Calendars.Read</span></span>      |
| <span data-ttu-id="c21e5-116">メッセージ</span><span class="sxs-lookup"><span data-stu-id="c21e5-116">Messages</span></span>                    | <span data-ttu-id="c21e5-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c21e5-117">Mail.Read</span></span>           |
| <span data-ttu-id="c21e5-118">Groups</span><span class="sxs-lookup"><span data-stu-id="c21e5-118">Groups</span></span>                      | <span data-ttu-id="c21e5-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c21e5-119">Group.Read.All</span></span>      |
| <span data-ttu-id="c21e5-120">Users</span><span class="sxs-lookup"><span data-stu-id="c21e5-120">Users</span></span>                       | <span data-ttu-id="c21e5-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c21e5-121">User.Read.All</span></span>       |
| <span data-ttu-id="c21e5-122">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="c21e5-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="c21e5-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c21e5-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="c21e5-124">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="c21e5-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="c21e5-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c21e5-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="c21e5-126">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="c21e5-126">Security alert</span></span>| <span data-ttu-id="c21e5-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c21e5-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c21e5-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c21e5-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c21e5-129">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c21e5-129">Optional query parameters</span></span>

<span data-ttu-id="c21e5-130">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c21e5-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c21e5-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c21e5-131">Request headers</span></span>

| <span data-ttu-id="c21e5-132">名前</span><span class="sxs-lookup"><span data-stu-id="c21e5-132">Name</span></span>       | <span data-ttu-id="c21e5-133">型</span><span class="sxs-lookup"><span data-stu-id="c21e5-133">Type</span></span> | <span data-ttu-id="c21e5-134">説明</span><span class="sxs-lookup"><span data-stu-id="c21e5-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c21e5-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="c21e5-135">Authorization</span></span>  | <span data-ttu-id="c21e5-136">string</span><span class="sxs-lookup"><span data-stu-id="c21e5-136">string</span></span>  | <span data-ttu-id="c21e5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c21e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c21e5-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="c21e5-139">Request body</span></span>

<span data-ttu-id="c21e5-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c21e5-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c21e5-141">応答</span><span class="sxs-lookup"><span data-stu-id="c21e5-141">Response</span></span>

<span data-ttu-id="c21e5-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c21e5-142">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c21e5-143">例</span><span class="sxs-lookup"><span data-stu-id="c21e5-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c21e5-144">要求</span><span class="sxs-lookup"><span data-stu-id="c21e5-144">Request</span></span>

<span data-ttu-id="c21e5-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c21e5-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="c21e5-146">応答</span><span class="sxs-lookup"><span data-stu-id="c21e5-146">Response</span></span>

<span data-ttu-id="c21e5-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c21e5-147">Here is an example of the response.</span></span>
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