---
title: サブスクリプションを更新する
description: サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 1bf693fb8551db916807570459d9658fa02665f1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167803"
---
# <a name="update-subscription"></a><span data-ttu-id="04673-103">サブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="04673-103">Update subscription</span></span>

<span data-ttu-id="04673-104">サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。</span><span class="sxs-lookup"><span data-stu-id="04673-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="04673-105">サブスクリプションは、リソースの種類によって異なる時間が経過すると有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="04673-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="04673-106">通知が失われないようにするために、アプリは有効期限の前にサブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04673-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="04673-107">リソースの種類ごとのサブスクリプションの最大長の[サブスクリプション](../resources/subscription.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04673-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="04673-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04673-108">Permissions</span></span>

<span data-ttu-id="04673-109">リソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可は、この API を呼び出すために必要な最低限の特権です。</span><span class="sxs-lookup"><span data-stu-id="04673-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="04673-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04673-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04673-111">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="04673-111">Supported resource</span></span> | <span data-ttu-id="04673-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04673-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04673-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04673-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04673-114">Application</span><span class="sxs-lookup"><span data-stu-id="04673-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="04673-115">連絡先</span><span class="sxs-lookup"><span data-stu-id="04673-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="04673-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="04673-116">Contacts.Read</span></span> | <span data-ttu-id="04673-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="04673-117">Contacts.Read</span></span> | <span data-ttu-id="04673-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="04673-118">Contacts.Read</span></span> |
|<span data-ttu-id="04673-119">[ドライブ項目](../resources/driveitem.md)(ユーザーの個人用 OneDrive)</span><span class="sxs-lookup"><span data-stu-id="04673-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="04673-120">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="04673-120">Not supported</span></span> | <span data-ttu-id="04673-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04673-121">Files.ReadWrite</span></span> | <span data-ttu-id="04673-122">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="04673-122">Not supported</span></span> |
|<span data-ttu-id="04673-123">[ドライブ項目](../resources/driveitem.md)(OneDrive for business)</span><span class="sxs-lookup"><span data-stu-id="04673-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="04673-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04673-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="04673-125">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="04673-125">Not supported</span></span> | <span data-ttu-id="04673-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04673-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="04673-127">event</span><span class="sxs-lookup"><span data-stu-id="04673-127">event</span></span>](../resources/event.md) | <span data-ttu-id="04673-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="04673-128">Calendars.Read</span></span> | <span data-ttu-id="04673-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="04673-129">Calendars.Read</span></span> | <span data-ttu-id="04673-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="04673-130">Calendars.Read</span></span> |
|[<span data-ttu-id="04673-131">group</span><span class="sxs-lookup"><span data-stu-id="04673-131">group</span></span>](../resources/group.md) | <span data-ttu-id="04673-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04673-132">Group.Read.All</span></span> | <span data-ttu-id="04673-133">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="04673-133">Not supported</span></span> | <span data-ttu-id="04673-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04673-134">Group.Read.All</span></span> |
|[<span data-ttu-id="04673-135">グループ会話</span><span class="sxs-lookup"><span data-stu-id="04673-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="04673-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04673-136">Group.Read.All</span></span> | <span data-ttu-id="04673-137">使用不可</span><span class="sxs-lookup"><span data-stu-id="04673-137">Not supported</span></span> | <span data-ttu-id="04673-138">使用不可</span><span class="sxs-lookup"><span data-stu-id="04673-138">Not supported</span></span> |
|[<span data-ttu-id="04673-139">message</span><span class="sxs-lookup"><span data-stu-id="04673-139">message</span></span>](../resources/message.md) | <span data-ttu-id="04673-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="04673-140">Mail.Read</span></span> | <span data-ttu-id="04673-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="04673-141">Mail.Read</span></span> | <span data-ttu-id="04673-142">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="04673-142">Mail.Read</span></span> |
|[<span data-ttu-id="04673-143">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="04673-143">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="04673-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04673-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="04673-145">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="04673-145">Not supported</span></span> | <span data-ttu-id="04673-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04673-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="04673-147">user</span><span class="sxs-lookup"><span data-stu-id="04673-147">user</span></span>](../resources/user.md) | <span data-ttu-id="04673-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="04673-148">User.Read.All</span></span> | <span data-ttu-id="04673-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="04673-149">User.Read.All</span></span> | <span data-ttu-id="04673-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="04673-150">User.Read.All</span></span> |

> <span data-ttu-id="04673-151">**注:** OneDrive および Outlook アイテムのサブスクリプションには、追加の制限があります。</span><span class="sxs-lookup"><span data-stu-id="04673-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="04673-152">この制限は、サブスクリプションの作成と管理 (サブスクリプションの取得、更新、および削除) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="04673-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="04673-153">個人用 OneDrive では、ルートフォルダーまたはそのドライブの任意のサブフォルダーを購読できます。</span><span class="sxs-lookup"><span data-stu-id="04673-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="04673-154">OneDrive for business では、ルートフォルダーのみをサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="04673-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="04673-155">通知は、サブスクライブされたフォルダー、または、階層内の任意のファイル、フォルダー、またはその他のファイル、フォルダー、またはその他のファイル、フォルダー、またはその他のファイル、フォルダー、またはその他の</span><span class="sxs-lookup"><span data-stu-id="04673-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="04673-156">個別のファイルなど、フォルダーではない**drive**または**drive アイテム**のインスタンスを購読することはできません。</span><span class="sxs-lookup"><span data-stu-id="04673-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="04673-157">Outlook では、委任されたアクセス許可は、サインインしているユーザーのメールボックス内のフォルダー内のアイテムのサブスクライブをサポートします。</span><span class="sxs-lookup"><span data-stu-id="04673-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="04673-158">つまり、委任されたアクセス許可のカレンダーを使用することはできません。別のユーザーのメールボックス内のイベントをサブスクライブするには、をお読みください。</span><span class="sxs-lookup"><span data-stu-id="04673-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="04673-159">Outlook の連絡先、イベント、または_共有フォルダーまたは委任_されたフォルダー内のメッセージの変更通知を購読するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="04673-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="04673-160">対応するアプリケーションのアクセス許可を使用して、テナント内の_任意_のユーザーのフォルダーまたはメールボックス内のアイテムの変更をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="04673-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="04673-161">共有または委任されたフォルダー内のアイテムの通知を変更するためのサブスクライブをサポートして**い**ないため、Outlook 共有のアクセス許可 (連絡先. 共有、読み取り/書き込み可能) を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="04673-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="04673-162">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04673-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="04673-163">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04673-163">Request headers</span></span>

| <span data-ttu-id="04673-164">名前</span><span class="sxs-lookup"><span data-stu-id="04673-164">Name</span></span>       | <span data-ttu-id="04673-165">型</span><span class="sxs-lookup"><span data-stu-id="04673-165">Type</span></span> | <span data-ttu-id="04673-166">説明</span><span class="sxs-lookup"><span data-stu-id="04673-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="04673-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="04673-167">Authorization</span></span>  | <span data-ttu-id="04673-168">string</span><span class="sxs-lookup"><span data-stu-id="04673-168">string</span></span>  | <span data-ttu-id="04673-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04673-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="04673-171">応答</span><span class="sxs-lookup"><span data-stu-id="04673-171">Response</span></span>

<span data-ttu-id="04673-172">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="04673-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04673-173">例</span><span class="sxs-lookup"><span data-stu-id="04673-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="04673-174">要求</span><span class="sxs-lookup"><span data-stu-id="04673-174">Request</span></span>

<span data-ttu-id="04673-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04673-175">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="04673-176">応答</span><span class="sxs-lookup"><span data-stu-id="04673-176">Response</span></span>

<span data-ttu-id="04673-177">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="04673-177">Here is an example of the response.</span></span>
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
