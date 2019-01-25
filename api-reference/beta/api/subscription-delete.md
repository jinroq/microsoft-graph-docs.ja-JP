---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9ca4c772cb6d7de088550a16262275b4c43fb9c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509463"
---
# <a name="delete-subscription"></a><span data-ttu-id="729df-103">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="729df-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="729df-104">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="729df-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="729df-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="729df-105">Permissions</span></span>

<span data-ttu-id="729df-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="729df-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="729df-108">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="729df-108">Resource type / Item</span></span>        | <span data-ttu-id="729df-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="729df-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="729df-110">連絡先</span><span class="sxs-lookup"><span data-stu-id="729df-110">Contacts</span></span>                    | <span data-ttu-id="729df-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="729df-111">Contacts.Read</span></span>       |
| <span data-ttu-id="729df-112">スレッド</span><span class="sxs-lookup"><span data-stu-id="729df-112">Conversations</span></span>               | <span data-ttu-id="729df-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="729df-113">Group.Read.All</span></span>      |
| <span data-ttu-id="729df-114">イベント</span><span class="sxs-lookup"><span data-stu-id="729df-114">Events</span></span>                      | <span data-ttu-id="729df-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="729df-115">Calendars.Read</span></span>      |
| <span data-ttu-id="729df-116">メッセージ</span><span class="sxs-lookup"><span data-stu-id="729df-116">Messages</span></span>                    | <span data-ttu-id="729df-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="729df-117">Mail.Read</span></span>           |
| <span data-ttu-id="729df-118">グループ</span><span class="sxs-lookup"><span data-stu-id="729df-118">Groups</span></span>                      | <span data-ttu-id="729df-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="729df-119">Group.Read.All</span></span>      |
| <span data-ttu-id="729df-120">ユーザー</span><span class="sxs-lookup"><span data-stu-id="729df-120">Users</span></span>                       | <span data-ttu-id="729df-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="729df-121">User.Read.All</span></span>       |
| <span data-ttu-id="729df-122">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="729df-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="729df-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="729df-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="729df-124">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="729df-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="729df-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="729df-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="729df-126">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="729df-126">Security alert</span></span>              | <span data-ttu-id="729df-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="729df-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="729df-128">***注:***/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="729df-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="729df-129">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="729df-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="729df-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="729df-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="729df-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="729df-131">Request headers</span></span>

| <span data-ttu-id="729df-132">名前</span><span class="sxs-lookup"><span data-stu-id="729df-132">Name</span></span>       | <span data-ttu-id="729df-133">型</span><span class="sxs-lookup"><span data-stu-id="729df-133">Type</span></span> | <span data-ttu-id="729df-134">説明</span><span class="sxs-lookup"><span data-stu-id="729df-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="729df-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="729df-135">Authorization</span></span>  | <span data-ttu-id="729df-136">string</span><span class="sxs-lookup"><span data-stu-id="729df-136">string</span></span>  | <span data-ttu-id="729df-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="729df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="729df-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="729df-139">Request body</span></span>

<span data-ttu-id="729df-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="729df-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="729df-141">応答</span><span class="sxs-lookup"><span data-stu-id="729df-141">Response</span></span>

<span data-ttu-id="729df-142">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="729df-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="729df-143">例</span><span class="sxs-lookup"><span data-stu-id="729df-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="729df-144">要求</span><span class="sxs-lookup"><span data-stu-id="729df-144">Request</span></span>

<span data-ttu-id="729df-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="729df-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="729df-146">応答</span><span class="sxs-lookup"><span data-stu-id="729df-146">Response</span></span>

<span data-ttu-id="729df-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="729df-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
