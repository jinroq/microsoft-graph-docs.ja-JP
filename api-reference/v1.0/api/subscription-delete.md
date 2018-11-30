---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
ms.openlocfilehash: 249393cef11e2768eec0a6435a8485b51cf6921c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024092"
---
# <a name="delete-subscription"></a><span data-ttu-id="8a230-103">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="8a230-103">Delete subscription</span></span>

<span data-ttu-id="8a230-104">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="8a230-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a230-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a230-105">Permissions</span></span>

<span data-ttu-id="8a230-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a230-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a230-108">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="8a230-108">Resource type / Item</span></span>        | <span data-ttu-id="8a230-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a230-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="8a230-110">連絡先</span><span class="sxs-lookup"><span data-stu-id="8a230-110">Contacts</span></span>                    | <span data-ttu-id="8a230-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8a230-111">Contacts.Read</span></span>       |
| <span data-ttu-id="8a230-112">スレッド</span><span class="sxs-lookup"><span data-stu-id="8a230-112">Conversations</span></span>               | <span data-ttu-id="8a230-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a230-113">Group.Read.All</span></span>      |
| <span data-ttu-id="8a230-114">イベント</span><span class="sxs-lookup"><span data-stu-id="8a230-114">Events</span></span>                      | <span data-ttu-id="8a230-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8a230-115">Calendars.Read</span></span>      |
| <span data-ttu-id="8a230-116">メッセージ</span><span class="sxs-lookup"><span data-stu-id="8a230-116">Messages</span></span>                    | <span data-ttu-id="8a230-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8a230-117">Mail.Read</span></span>           |
| <span data-ttu-id="8a230-118">Groups</span><span class="sxs-lookup"><span data-stu-id="8a230-118">Groups</span></span>                      | <span data-ttu-id="8a230-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a230-119">Group.Read.All</span></span>      |
| <span data-ttu-id="8a230-120">Users</span><span class="sxs-lookup"><span data-stu-id="8a230-120">Users</span></span>                       | <span data-ttu-id="8a230-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a230-121">User.Read.All</span></span>       |
| <span data-ttu-id="8a230-122">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="8a230-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="8a230-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a230-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="8a230-124">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="8a230-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="8a230-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a230-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="8a230-126">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="8a230-126">Security alert</span></span>| <span data-ttu-id="8a230-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a230-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a230-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a230-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8a230-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a230-129">Request headers</span></span>

| <span data-ttu-id="8a230-130">名前</span><span class="sxs-lookup"><span data-stu-id="8a230-130">Name</span></span>       | <span data-ttu-id="8a230-131">型</span><span class="sxs-lookup"><span data-stu-id="8a230-131">Type</span></span> | <span data-ttu-id="8a230-132">説明</span><span class="sxs-lookup"><span data-stu-id="8a230-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8a230-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a230-133">Authorization</span></span>  | <span data-ttu-id="8a230-134">string</span><span class="sxs-lookup"><span data-stu-id="8a230-134">string</span></span>  | <span data-ttu-id="8a230-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a230-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a230-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a230-137">Request body</span></span>

<span data-ttu-id="8a230-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a230-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a230-139">応答</span><span class="sxs-lookup"><span data-stu-id="8a230-139">Response</span></span>

<span data-ttu-id="8a230-140">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8a230-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8a230-141">例</span><span class="sxs-lookup"><span data-stu-id="8a230-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8a230-142">要求</span><span class="sxs-lookup"><span data-stu-id="8a230-142">Request</span></span>

<span data-ttu-id="8a230-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a230-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="8a230-144">応答</span><span class="sxs-lookup"><span data-stu-id="8a230-144">Response</span></span>

<span data-ttu-id="8a230-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8a230-145">Here is an example of the response.</span></span>
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
