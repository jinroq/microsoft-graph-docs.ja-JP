---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
localization_priority: Normal
ms.openlocfilehash: a5bd1998df3a7e3a8896fa770c0dbdd72cd59940
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805594"
---
# <a name="delete-subscription"></a><span data-ttu-id="04426-103">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="04426-103">Delete subscription</span></span>

<span data-ttu-id="04426-104">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="04426-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="04426-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04426-105">Permissions</span></span>

<span data-ttu-id="04426-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04426-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04426-108">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="04426-108">Resource type / Item</span></span>        | <span data-ttu-id="04426-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04426-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="04426-110">連絡先</span><span class="sxs-lookup"><span data-stu-id="04426-110">Contacts</span></span>                    | <span data-ttu-id="04426-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="04426-111">Contacts.Read</span></span>       |
| <span data-ttu-id="04426-112">スレッド</span><span class="sxs-lookup"><span data-stu-id="04426-112">Conversations</span></span>               | <span data-ttu-id="04426-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04426-113">Group.Read.All</span></span>      |
| <span data-ttu-id="04426-114">イベント</span><span class="sxs-lookup"><span data-stu-id="04426-114">Events</span></span>                      | <span data-ttu-id="04426-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="04426-115">Calendars.Read</span></span>      |
| <span data-ttu-id="04426-116">メッセージ</span><span class="sxs-lookup"><span data-stu-id="04426-116">Messages</span></span>                    | <span data-ttu-id="04426-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="04426-117">Mail.Read</span></span>           |
| <span data-ttu-id="04426-118">グループ</span><span class="sxs-lookup"><span data-stu-id="04426-118">Groups</span></span>                      | <span data-ttu-id="04426-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04426-119">Group.Read.All</span></span>      |
| <span data-ttu-id="04426-120">ユーザー</span><span class="sxs-lookup"><span data-stu-id="04426-120">Users</span></span>                       | <span data-ttu-id="04426-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="04426-121">User.Read.All</span></span>       |
| <span data-ttu-id="04426-122">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="04426-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="04426-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04426-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="04426-124">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="04426-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="04426-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04426-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="04426-126">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="04426-126">Security alert</span></span>| <span data-ttu-id="04426-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04426-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04426-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04426-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="04426-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04426-129">Request headers</span></span>

| <span data-ttu-id="04426-130">名前</span><span class="sxs-lookup"><span data-stu-id="04426-130">Name</span></span>       | <span data-ttu-id="04426-131">種類</span><span class="sxs-lookup"><span data-stu-id="04426-131">Type</span></span> | <span data-ttu-id="04426-132">説明</span><span class="sxs-lookup"><span data-stu-id="04426-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="04426-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="04426-133">Authorization</span></span>  | <span data-ttu-id="04426-134">string</span><span class="sxs-lookup"><span data-stu-id="04426-134">string</span></span>  | <span data-ttu-id="04426-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04426-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04426-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="04426-137">Request body</span></span>

<span data-ttu-id="04426-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="04426-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04426-139">応答</span><span class="sxs-lookup"><span data-stu-id="04426-139">Response</span></span>

<span data-ttu-id="04426-140">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="04426-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04426-141">例</span><span class="sxs-lookup"><span data-stu-id="04426-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="04426-142">要求</span><span class="sxs-lookup"><span data-stu-id="04426-142">Request</span></span>

<span data-ttu-id="04426-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04426-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="04426-144">応答</span><span class="sxs-lookup"><span data-stu-id="04426-144">Response</span></span>

<span data-ttu-id="04426-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="04426-145">Here is an example of the response.</span></span>
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
