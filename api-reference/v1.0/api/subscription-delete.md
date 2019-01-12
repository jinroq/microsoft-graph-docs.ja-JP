---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: eeed4a7f6981a89a1869257bed339eb6895f25b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932582"
---
# <a name="delete-subscription"></a><span data-ttu-id="fcd58-103">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="fcd58-103">Delete subscription</span></span>

<span data-ttu-id="fcd58-104">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="fcd58-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcd58-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fcd58-105">Permissions</span></span>

<span data-ttu-id="fcd58-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fcd58-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fcd58-108">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="fcd58-108">Resource type / Item</span></span>        | <span data-ttu-id="fcd58-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fcd58-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="fcd58-110">連絡先</span><span class="sxs-lookup"><span data-stu-id="fcd58-110">Contacts</span></span>                    | <span data-ttu-id="fcd58-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fcd58-111">Contacts.Read</span></span>       |
| <span data-ttu-id="fcd58-112">スレッド</span><span class="sxs-lookup"><span data-stu-id="fcd58-112">Conversations</span></span>               | <span data-ttu-id="fcd58-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd58-113">Group.Read.All</span></span>      |
| <span data-ttu-id="fcd58-114">イベント</span><span class="sxs-lookup"><span data-stu-id="fcd58-114">Events</span></span>                      | <span data-ttu-id="fcd58-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fcd58-115">Calendars.Read</span></span>      |
| <span data-ttu-id="fcd58-116">メッセージ</span><span class="sxs-lookup"><span data-stu-id="fcd58-116">Messages</span></span>                    | <span data-ttu-id="fcd58-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fcd58-117">Mail.Read</span></span>           |
| <span data-ttu-id="fcd58-118">グループ</span><span class="sxs-lookup"><span data-stu-id="fcd58-118">Groups</span></span>                      | <span data-ttu-id="fcd58-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd58-119">Group.Read.All</span></span>      |
| <span data-ttu-id="fcd58-120">ユーザー</span><span class="sxs-lookup"><span data-stu-id="fcd58-120">Users</span></span>                       | <span data-ttu-id="fcd58-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd58-121">User.Read.All</span></span>       |
| <span data-ttu-id="fcd58-122">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="fcd58-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="fcd58-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcd58-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="fcd58-124">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="fcd58-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="fcd58-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd58-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="fcd58-126">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="fcd58-126">Security alert</span></span>| <span data-ttu-id="fcd58-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd58-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcd58-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fcd58-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fcd58-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fcd58-129">Request headers</span></span>

| <span data-ttu-id="fcd58-130">名前</span><span class="sxs-lookup"><span data-stu-id="fcd58-130">Name</span></span>       | <span data-ttu-id="fcd58-131">種類</span><span class="sxs-lookup"><span data-stu-id="fcd58-131">Type</span></span> | <span data-ttu-id="fcd58-132">説明</span><span class="sxs-lookup"><span data-stu-id="fcd58-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fcd58-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcd58-133">Authorization</span></span>  | <span data-ttu-id="fcd58-134">string</span><span class="sxs-lookup"><span data-stu-id="fcd58-134">string</span></span>  | <span data-ttu-id="fcd58-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fcd58-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcd58-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="fcd58-137">Request body</span></span>

<span data-ttu-id="fcd58-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fcd58-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcd58-139">応答</span><span class="sxs-lookup"><span data-stu-id="fcd58-139">Response</span></span>

<span data-ttu-id="fcd58-140">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fcd58-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fcd58-141">例</span><span class="sxs-lookup"><span data-stu-id="fcd58-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fcd58-142">要求</span><span class="sxs-lookup"><span data-stu-id="fcd58-142">Request</span></span>

<span data-ttu-id="fcd58-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fcd58-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="fcd58-144">応答</span><span class="sxs-lookup"><span data-stu-id="fcd58-144">Response</span></span>

<span data-ttu-id="fcd58-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fcd58-145">Here is an example of the response.</span></span>
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
