---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
localization_priority: Normal
ms.openlocfilehash: 1e2efb9835e5e625bdac0385b5011cfe5c8c64b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842050"
---
# <a name="delete-subscription"></a><span data-ttu-id="2463a-103">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="2463a-103">Delete subscription</span></span>

> <span data-ttu-id="2463a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2463a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2463a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2463a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2463a-106">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="2463a-106">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="2463a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2463a-107">Permissions</span></span>

<span data-ttu-id="2463a-p102">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2463a-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2463a-110">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="2463a-110">Resource type / Item</span></span>        | <span data-ttu-id="2463a-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2463a-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="2463a-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="2463a-112">Contacts</span></span>                    | <span data-ttu-id="2463a-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2463a-113">Contacts.Read</span></span>       |
| <span data-ttu-id="2463a-114">スレッド</span><span class="sxs-lookup"><span data-stu-id="2463a-114">Conversations</span></span>               | <span data-ttu-id="2463a-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2463a-115">Group.Read.All</span></span>      |
| <span data-ttu-id="2463a-116">イベント</span><span class="sxs-lookup"><span data-stu-id="2463a-116">Events</span></span>                      | <span data-ttu-id="2463a-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2463a-117">Calendars.Read</span></span>      |
| <span data-ttu-id="2463a-118">メッセージ</span><span class="sxs-lookup"><span data-stu-id="2463a-118">Messages</span></span>                    | <span data-ttu-id="2463a-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2463a-119">Mail.Read</span></span>           |
| <span data-ttu-id="2463a-120">グループ</span><span class="sxs-lookup"><span data-stu-id="2463a-120">Groups</span></span>                      | <span data-ttu-id="2463a-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2463a-121">Group.Read.All</span></span>      |
| <span data-ttu-id="2463a-122">ユーザー</span><span class="sxs-lookup"><span data-stu-id="2463a-122">Users</span></span>                       | <span data-ttu-id="2463a-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2463a-123">User.Read.All</span></span>       |
| <span data-ttu-id="2463a-124">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="2463a-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="2463a-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2463a-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="2463a-126">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="2463a-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="2463a-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2463a-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="2463a-128">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="2463a-128">Security alert</span></span>              | <span data-ttu-id="2463a-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2463a-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="2463a-130">***注:***/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="2463a-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="2463a-131">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2463a-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="2463a-132">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2463a-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2463a-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2463a-133">Request headers</span></span>

| <span data-ttu-id="2463a-134">名前</span><span class="sxs-lookup"><span data-stu-id="2463a-134">Name</span></span>       | <span data-ttu-id="2463a-135">種類</span><span class="sxs-lookup"><span data-stu-id="2463a-135">Type</span></span> | <span data-ttu-id="2463a-136">説明</span><span class="sxs-lookup"><span data-stu-id="2463a-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2463a-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="2463a-137">Authorization</span></span>  | <span data-ttu-id="2463a-138">string</span><span class="sxs-lookup"><span data-stu-id="2463a-138">string</span></span>  | <span data-ttu-id="2463a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2463a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2463a-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="2463a-141">Request body</span></span>

<span data-ttu-id="2463a-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2463a-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2463a-143">応答</span><span class="sxs-lookup"><span data-stu-id="2463a-143">Response</span></span>

<span data-ttu-id="2463a-144">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2463a-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2463a-145">例</span><span class="sxs-lookup"><span data-stu-id="2463a-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2463a-146">要求</span><span class="sxs-lookup"><span data-stu-id="2463a-146">Request</span></span>

<span data-ttu-id="2463a-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2463a-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="2463a-148">応答</span><span class="sxs-lookup"><span data-stu-id="2463a-148">Response</span></span>

<span data-ttu-id="2463a-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2463a-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
