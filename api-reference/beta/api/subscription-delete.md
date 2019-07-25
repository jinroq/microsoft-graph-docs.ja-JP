---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: cb76dca373d6d175ad68c38cedb8b00573d69816
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869510"
---
# <a name="delete-subscription"></a><span data-ttu-id="6690e-103">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="6690e-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6690e-104">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="6690e-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="6690e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6690e-105">Permissions</span></span>

<span data-ttu-id="6690e-106">要求されたリソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、以下の表で指定されているアクセス許可がこの API を呼び出すため必要な最小限の特権となります。</span><span class="sxs-lookup"><span data-stu-id="6690e-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6690e-107">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6690e-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6690e-108">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="6690e-108">Supported resource</span></span> | <span data-ttu-id="6690e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6690e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6690e-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6690e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6690e-111">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6690e-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6690e-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="6690e-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6690e-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6690e-113">Contacts.Read</span></span> | <span data-ttu-id="6690e-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6690e-114">Contacts.Read</span></span> | <span data-ttu-id="6690e-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6690e-115">Contacts.Read</span></span> |
|<span data-ttu-id="6690e-116">[driveItem](../resources/driveitem.md) (ユーザーの個人用 OneDrive)</span><span class="sxs-lookup"><span data-stu-id="6690e-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6690e-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="6690e-117">Not supported</span></span> | <span data-ttu-id="6690e-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6690e-118">Files.ReadWrite</span></span> | <span data-ttu-id="6690e-119">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="6690e-119">Not supported</span></span> |
|<span data-ttu-id="6690e-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="6690e-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6690e-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6690e-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="6690e-122">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="6690e-122">Not supported</span></span> | <span data-ttu-id="6690e-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6690e-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6690e-124">イベント</span><span class="sxs-lookup"><span data-stu-id="6690e-124">event</span></span>](../resources/event.md) | <span data-ttu-id="6690e-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6690e-125">Calendars.Read</span></span> | <span data-ttu-id="6690e-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6690e-126">Calendars.Read</span></span> | <span data-ttu-id="6690e-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6690e-127">Calendars.Read</span></span> |
|[<span data-ttu-id="6690e-128">グループ</span><span class="sxs-lookup"><span data-stu-id="6690e-128">group</span></span>](../resources/group.md) | <span data-ttu-id="6690e-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6690e-129">Group.Read.All</span></span> | <span data-ttu-id="6690e-130">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6690e-130">Not supported</span></span> | <span data-ttu-id="6690e-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6690e-131">Group.Read.All</span></span> |
|[<span data-ttu-id="6690e-132">グループ会話</span><span class="sxs-lookup"><span data-stu-id="6690e-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6690e-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6690e-133">Group.Read.All</span></span> | <span data-ttu-id="6690e-134">非サポート</span><span class="sxs-lookup"><span data-stu-id="6690e-134">Not supported</span></span> | <span data-ttu-id="6690e-135">非サポート</span><span class="sxs-lookup"><span data-stu-id="6690e-135">Not supported</span></span> |
|[<span data-ttu-id="6690e-136">メッセージ</span><span class="sxs-lookup"><span data-stu-id="6690e-136">message</span></span>](../resources/message.md) | <span data-ttu-id="6690e-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6690e-137">Mail.Read</span></span> | <span data-ttu-id="6690e-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6690e-138">Mail.Read</span></span> | <span data-ttu-id="6690e-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6690e-139">Mail.Read</span></span> |
|[<span data-ttu-id="6690e-140">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="6690e-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6690e-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6690e-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6690e-142">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6690e-142">Not supported</span></span> | <span data-ttu-id="6690e-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6690e-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6690e-144">ユーザー</span><span class="sxs-lookup"><span data-stu-id="6690e-144">user</span></span>](../resources/user.md) | <span data-ttu-id="6690e-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6690e-145">User.Read.All</span></span> | <span data-ttu-id="6690e-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6690e-146">User.Read.All</span></span> | <span data-ttu-id="6690e-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6690e-147">User.Read.All</span></span> |

> <span data-ttu-id="6690e-148">**注:** OneDrive と Outlook のアイテムのサブスクリプションについては、追加の制限があります。</span><span class="sxs-lookup"><span data-stu-id="6690e-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="6690e-149">この制限は、サブスクリプションの作成および管理 (サブスクリプションの取得、更新、削除) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="6690e-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="6690e-150">個人用 OneDrive では、そのドライブのルート フォルダーまたは任意のサブフォルダーにサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="6690e-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6690e-151">OneDrive for Business の場合、サブスクライブできるのはルート フォルダーだけです。</span><span class="sxs-lookup"><span data-stu-id="6690e-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6690e-152">サブスクライブしたフォルダー、または階層内の任意のファイル、フォルダー、あるいは他の driveItem オブジェクトの要求された種類の変更について通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="6690e-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="6690e-153">**ドライブ**、または個々のファイルなどのフォルダーではない **driveItem** インスタンスをサブスクライブすることはできません。</span><span class="sxs-lookup"><span data-stu-id="6690e-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="6690e-154">Outlook における委任されたアクセス許可では、サインインしているユーザーのメールボックス内のフォルダーにあるアイテムのみをサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="6690e-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6690e-155">つまり、委任されたアクセス許可 Calendars.Read を使用して、別のユーザーのメールボックス内のイベントをサブスクライブすることなどはできません。</span><span class="sxs-lookup"><span data-stu-id="6690e-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6690e-156">_共有または委任_フォルダーの Outlook 連絡先、イベント、メッセージの変更通知をサブスクライブするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="6690e-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6690e-157">対応するアプリケーション アクセス許可を使用して、テナントの_任意_のユーザーのフォルダーまたはメールボックス内にあるアイテムの変更をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="6690e-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6690e-158">Outlook 共有アクセス許可 (Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared、および対応する読み取り/書き込み) は使用しないでください。それらは、共有フォルダーまたは委任フォルダーにあるアイテムの変更通知のサブスクライブをサポート**していない**からです。</span><span class="sxs-lookup"><span data-stu-id="6690e-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="6690e-159">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6690e-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6690e-160">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6690e-160">Request headers</span></span>

| <span data-ttu-id="6690e-161">名前</span><span class="sxs-lookup"><span data-stu-id="6690e-161">Name</span></span>       | <span data-ttu-id="6690e-162">型</span><span class="sxs-lookup"><span data-stu-id="6690e-162">Type</span></span> | <span data-ttu-id="6690e-163">説明</span><span class="sxs-lookup"><span data-stu-id="6690e-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6690e-164">Authorization</span><span class="sxs-lookup"><span data-stu-id="6690e-164">Authorization</span></span>  | <span data-ttu-id="6690e-165">string</span><span class="sxs-lookup"><span data-stu-id="6690e-165">string</span></span>  | <span data-ttu-id="6690e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6690e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6690e-168">要求本文</span><span class="sxs-lookup"><span data-stu-id="6690e-168">Request body</span></span>

<span data-ttu-id="6690e-169">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6690e-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6690e-170">応答</span><span class="sxs-lookup"><span data-stu-id="6690e-170">Response</span></span>

<span data-ttu-id="6690e-171">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6690e-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6690e-172">例</span><span class="sxs-lookup"><span data-stu-id="6690e-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6690e-173">要求</span><span class="sxs-lookup"><span data-stu-id="6690e-173">Request</span></span>

<span data-ttu-id="6690e-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6690e-174">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6690e-175">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6690e-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6690e-176">C#</span><span class="sxs-lookup"><span data-stu-id="6690e-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6690e-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="6690e-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6690e-178">目的-C</span><span class="sxs-lookup"><span data-stu-id="6690e-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6690e-179">Java</span><span class="sxs-lookup"><span data-stu-id="6690e-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6690e-180">応答</span><span class="sxs-lookup"><span data-stu-id="6690e-180">Response</span></span>

<span data-ttu-id="6690e-181">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6690e-181">Here is an example of the response.</span></span>
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
  ]
}
-->
