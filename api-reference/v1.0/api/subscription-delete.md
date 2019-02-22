---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 97df6f59d4a8acfacec479e718970feef0c77632
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161433"
---
# <a name="delete-subscription"></a><span data-ttu-id="4526e-103">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="4526e-103">Delete subscription</span></span>

<span data-ttu-id="4526e-104">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="4526e-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="4526e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4526e-105">Permissions</span></span>

<span data-ttu-id="4526e-106">リソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可は、この API を呼び出すために必要な最低限の特権です。</span><span class="sxs-lookup"><span data-stu-id="4526e-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4526e-107">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4526e-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4526e-108">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="4526e-108">Supported resource</span></span> | <span data-ttu-id="4526e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4526e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4526e-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4526e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4526e-111">Application</span><span class="sxs-lookup"><span data-stu-id="4526e-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="4526e-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="4526e-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="4526e-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4526e-113">Contacts.Read</span></span> | <span data-ttu-id="4526e-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4526e-114">Contacts.Read</span></span> | <span data-ttu-id="4526e-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4526e-115">Contacts.Read</span></span> |
|<span data-ttu-id="4526e-116">[ドライブ項目](../resources/driveitem.md)(ユーザーの個人用 OneDrive)</span><span class="sxs-lookup"><span data-stu-id="4526e-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="4526e-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4526e-117">Not supported</span></span> | <span data-ttu-id="4526e-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4526e-118">Files.ReadWrite</span></span> | <span data-ttu-id="4526e-119">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4526e-119">Not supported</span></span> |
|<span data-ttu-id="4526e-120">[ドライブ項目](../resources/driveitem.md)(OneDrive for business)</span><span class="sxs-lookup"><span data-stu-id="4526e-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="4526e-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4526e-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="4526e-122">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4526e-122">Not supported</span></span> | <span data-ttu-id="4526e-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4526e-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="4526e-124">event</span><span class="sxs-lookup"><span data-stu-id="4526e-124">event</span></span>](../resources/event.md) | <span data-ttu-id="4526e-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4526e-125">Calendars.Read</span></span> | <span data-ttu-id="4526e-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4526e-126">Calendars.Read</span></span> | <span data-ttu-id="4526e-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4526e-127">Calendars.Read</span></span> |
|[<span data-ttu-id="4526e-128">group</span><span class="sxs-lookup"><span data-stu-id="4526e-128">group</span></span>](../resources/group.md) | <span data-ttu-id="4526e-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4526e-129">Group.Read.All</span></span> | <span data-ttu-id="4526e-130">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4526e-130">Not supported</span></span> | <span data-ttu-id="4526e-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4526e-131">Group.Read.All</span></span> |
|[<span data-ttu-id="4526e-132">グループ会話</span><span class="sxs-lookup"><span data-stu-id="4526e-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="4526e-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4526e-133">Group.Read.All</span></span> | <span data-ttu-id="4526e-134">使用不可</span><span class="sxs-lookup"><span data-stu-id="4526e-134">Not supported</span></span> | <span data-ttu-id="4526e-135">使用不可</span><span class="sxs-lookup"><span data-stu-id="4526e-135">Not supported</span></span> |
|[<span data-ttu-id="4526e-136">message</span><span class="sxs-lookup"><span data-stu-id="4526e-136">message</span></span>](../resources/message.md) | <span data-ttu-id="4526e-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4526e-137">Mail.Read</span></span> | <span data-ttu-id="4526e-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4526e-138">Mail.Read</span></span> | <span data-ttu-id="4526e-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4526e-139">Mail.Read</span></span> |
|[<span data-ttu-id="4526e-140">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="4526e-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="4526e-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4526e-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="4526e-142">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4526e-142">Not supported</span></span> | <span data-ttu-id="4526e-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4526e-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="4526e-144">user</span><span class="sxs-lookup"><span data-stu-id="4526e-144">user</span></span>](../resources/user.md) | <span data-ttu-id="4526e-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4526e-145">User.Read.All</span></span> | <span data-ttu-id="4526e-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4526e-146">User.Read.All</span></span> | <span data-ttu-id="4526e-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4526e-147">User.Read.All</span></span> |

> <span data-ttu-id="4526e-148">**注:** OneDrive および Outlook アイテムのサブスクリプションには、追加の制限があります。</span><span class="sxs-lookup"><span data-stu-id="4526e-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="4526e-149">この制限は、サブスクリプションの作成と管理 (サブスクリプションの取得、更新、および削除) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="4526e-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="4526e-150">個人用 OneDrive では、ルートフォルダーまたはそのドライブの任意のサブフォルダーを購読できます。</span><span class="sxs-lookup"><span data-stu-id="4526e-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="4526e-151">OneDrive for business では、ルートフォルダーのみをサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="4526e-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="4526e-152">通知は、サブスクライブされたフォルダー、または、階層内の任意のファイル、フォルダー、またはその他のファイル、フォルダー、またはその他のファイル、フォルダー、またはその他のファイル、フォルダー、またはその他の</span><span class="sxs-lookup"><span data-stu-id="4526e-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="4526e-153">個別のファイルなど、フォルダーではない**drive**または**drive アイテム**のインスタンスを購読することはできません。</span><span class="sxs-lookup"><span data-stu-id="4526e-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="4526e-154">Outlook では、委任されたアクセス許可は、サインインしているユーザーのメールボックス内のフォルダー内のアイテムのサブスクライブをサポートします。</span><span class="sxs-lookup"><span data-stu-id="4526e-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="4526e-155">つまり、委任されたアクセス許可のカレンダーを使用することはできません。別のユーザーのメールボックス内のイベントをサブスクライブするには、をお読みください。</span><span class="sxs-lookup"><span data-stu-id="4526e-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="4526e-156">Outlook の連絡先、イベント、または_共有フォルダーまたは委任_されたフォルダー内のメッセージの変更通知を購読するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4526e-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="4526e-157">対応するアプリケーションのアクセス許可を使用して、テナント内の_任意_のユーザーのフォルダーまたはメールボックス内のアイテムの変更をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="4526e-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="4526e-158">共有または委任されたフォルダー内のアイテムの通知を変更するためのサブスクライブをサポートして**い**ないため、Outlook 共有のアクセス許可 (連絡先. 共有、読み取り/書き込み可能) を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="4526e-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="4526e-159">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4526e-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4526e-160">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4526e-160">Request headers</span></span>

| <span data-ttu-id="4526e-161">名前</span><span class="sxs-lookup"><span data-stu-id="4526e-161">Name</span></span>       | <span data-ttu-id="4526e-162">型</span><span class="sxs-lookup"><span data-stu-id="4526e-162">Type</span></span> | <span data-ttu-id="4526e-163">説明</span><span class="sxs-lookup"><span data-stu-id="4526e-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4526e-164">Authorization</span><span class="sxs-lookup"><span data-stu-id="4526e-164">Authorization</span></span>  | <span data-ttu-id="4526e-165">string</span><span class="sxs-lookup"><span data-stu-id="4526e-165">string</span></span>  | <span data-ttu-id="4526e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4526e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4526e-168">要求本文</span><span class="sxs-lookup"><span data-stu-id="4526e-168">Request body</span></span>

<span data-ttu-id="4526e-169">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4526e-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4526e-170">応答</span><span class="sxs-lookup"><span data-stu-id="4526e-170">Response</span></span>

<span data-ttu-id="4526e-171">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4526e-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4526e-172">例</span><span class="sxs-lookup"><span data-stu-id="4526e-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4526e-173">要求</span><span class="sxs-lookup"><span data-stu-id="4526e-173">Request</span></span>

<span data-ttu-id="4526e-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4526e-174">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="4526e-175">応答</span><span class="sxs-lookup"><span data-stu-id="4526e-175">Response</span></span>

<span data-ttu-id="4526e-176">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4526e-176">Here is an example of the response.</span></span>
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
