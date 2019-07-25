---
title: サブスクリプションを更新する
description: サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: ca0a6f47a4841864b18c720559b7b0420a130404
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894330"
---
# <a name="update-subscription"></a><span data-ttu-id="109a5-103">サブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="109a5-103">Update subscription</span></span>

<span data-ttu-id="109a5-104">サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。</span><span class="sxs-lookup"><span data-stu-id="109a5-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="109a5-105">サブスクリプションは、リソースの種類によって異なる時間が経過すると有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="109a5-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="109a5-106">通知が失われないようにするために、アプリは有効期限の前にサブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="109a5-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="109a5-107">リソースの種類ごとのサブスクリプションの最大長の[サブスクリプション](../resources/subscription.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="109a5-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="109a5-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="109a5-108">Permissions</span></span>

<span data-ttu-id="109a5-109">要求されたリソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、以下の表で指定されているアクセス許可がこの API を呼び出すため必要な最小限の特権となります。</span><span class="sxs-lookup"><span data-stu-id="109a5-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="109a5-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="109a5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="109a5-111">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="109a5-111">Supported resource</span></span> | <span data-ttu-id="109a5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="109a5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="109a5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="109a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="109a5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="109a5-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="109a5-115">連絡先</span><span class="sxs-lookup"><span data-stu-id="109a5-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="109a5-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="109a5-116">Contacts.Read</span></span> | <span data-ttu-id="109a5-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="109a5-117">Contacts.Read</span></span> | <span data-ttu-id="109a5-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="109a5-118">Contacts.Read</span></span> |
|<span data-ttu-id="109a5-119">[driveItem](../resources/driveitem.md) (ユーザーの個人用 OneDrive)</span><span class="sxs-lookup"><span data-stu-id="109a5-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="109a5-120">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="109a5-120">Not supported</span></span> | <span data-ttu-id="109a5-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="109a5-121">Files.ReadWrite</span></span> | <span data-ttu-id="109a5-122">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="109a5-122">Not supported</span></span> |
|<span data-ttu-id="109a5-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="109a5-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="109a5-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="109a5-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="109a5-125">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="109a5-125">Not supported</span></span> | <span data-ttu-id="109a5-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="109a5-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="109a5-127">イベント</span><span class="sxs-lookup"><span data-stu-id="109a5-127">event</span></span>](../resources/event.md) | <span data-ttu-id="109a5-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="109a5-128">Calendars.Read</span></span> | <span data-ttu-id="109a5-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="109a5-129">Calendars.Read</span></span> | <span data-ttu-id="109a5-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="109a5-130">Calendars.Read</span></span> |
|[<span data-ttu-id="109a5-131">グループ</span><span class="sxs-lookup"><span data-stu-id="109a5-131">group</span></span>](../resources/group.md) | <span data-ttu-id="109a5-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="109a5-132">Group.Read.All</span></span> | <span data-ttu-id="109a5-133">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="109a5-133">Not supported</span></span> | <span data-ttu-id="109a5-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="109a5-134">Group.Read.All</span></span> |
|[<span data-ttu-id="109a5-135">グループ会話</span><span class="sxs-lookup"><span data-stu-id="109a5-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="109a5-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="109a5-136">Group.Read.All</span></span> | <span data-ttu-id="109a5-137">非サポート</span><span class="sxs-lookup"><span data-stu-id="109a5-137">Not supported</span></span> | <span data-ttu-id="109a5-138">非サポート</span><span class="sxs-lookup"><span data-stu-id="109a5-138">Not supported</span></span> |
|[<span data-ttu-id="109a5-139">メッセージ</span><span class="sxs-lookup"><span data-stu-id="109a5-139">message</span></span>](../resources/message.md) | <span data-ttu-id="109a5-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="109a5-140">Mail.Read</span></span> | <span data-ttu-id="109a5-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="109a5-141">Mail.Read</span></span> | <span data-ttu-id="109a5-142">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="109a5-142">Mail.Read</span></span> |
|[<span data-ttu-id="109a5-143">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="109a5-143">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="109a5-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="109a5-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="109a5-145">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="109a5-145">Not supported</span></span> | <span data-ttu-id="109a5-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="109a5-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="109a5-147">ユーザー</span><span class="sxs-lookup"><span data-stu-id="109a5-147">user</span></span>](../resources/user.md) | <span data-ttu-id="109a5-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="109a5-148">User.Read.All</span></span> | <span data-ttu-id="109a5-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="109a5-149">User.Read.All</span></span> | <span data-ttu-id="109a5-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="109a5-150">User.Read.All</span></span> |

> <span data-ttu-id="109a5-151">**注:** OneDrive と Outlook のアイテムのサブスクリプションについては、追加の制限があります。</span><span class="sxs-lookup"><span data-stu-id="109a5-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="109a5-152">この制限は、サブスクリプションの作成および管理 (サブスクリプションの取得、更新、削除) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="109a5-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="109a5-153">個人用 OneDrive では、そのドライブのルート フォルダーまたは任意のサブフォルダーにサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="109a5-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="109a5-154">OneDrive for Business の場合、サブスクライブできるのはルート フォルダーだけです。</span><span class="sxs-lookup"><span data-stu-id="109a5-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="109a5-155">サブスクライブしたフォルダー、または階層内の任意のファイル、フォルダー、あるいは他の driveItem オブジェクトの要求された種類の変更について通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="109a5-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="109a5-156">**ドライブ**、または個々のファイルなどのフォルダーではない **driveItem** インスタンスをサブスクライブすることはできません。</span><span class="sxs-lookup"><span data-stu-id="109a5-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="109a5-157">Outlook における委任されたアクセス許可では、サインインしているユーザーのメールボックス内のフォルダーにあるアイテムのみをサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="109a5-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="109a5-158">つまり、委任されたアクセス許可 Calendars.Read を使用して、別のユーザーのメールボックス内のイベントをサブスクライブすることなどはできません。</span><span class="sxs-lookup"><span data-stu-id="109a5-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="109a5-159">_共有または委任_フォルダーの Outlook 連絡先、イベント、メッセージの変更通知をサブスクライブするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="109a5-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="109a5-160">対応するアプリケーション アクセス許可を使用して、テナントの_任意_のユーザーのフォルダーまたはメールボックス内にあるアイテムの変更をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="109a5-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="109a5-161">Outlook 共有アクセス許可 (Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared、および対応する読み取り/書き込み) は使用しないでください。それらは、共有フォルダーまたは委任フォルダーにあるアイテムの変更通知のサブスクライブをサポート**していない**からです。</span><span class="sxs-lookup"><span data-stu-id="109a5-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="109a5-162">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="109a5-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="109a5-163">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="109a5-163">Request headers</span></span>

| <span data-ttu-id="109a5-164">名前</span><span class="sxs-lookup"><span data-stu-id="109a5-164">Name</span></span>       | <span data-ttu-id="109a5-165">型</span><span class="sxs-lookup"><span data-stu-id="109a5-165">Type</span></span> | <span data-ttu-id="109a5-166">説明</span><span class="sxs-lookup"><span data-stu-id="109a5-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="109a5-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="109a5-167">Authorization</span></span>  | <span data-ttu-id="109a5-168">string</span><span class="sxs-lookup"><span data-stu-id="109a5-168">string</span></span>  | <span data-ttu-id="109a5-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="109a5-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="109a5-171">応答</span><span class="sxs-lookup"><span data-stu-id="109a5-171">Response</span></span>

<span data-ttu-id="109a5-172">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="109a5-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="109a5-173">例</span><span class="sxs-lookup"><span data-stu-id="109a5-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="109a5-174">要求</span><span class="sxs-lookup"><span data-stu-id="109a5-174">Request</span></span>

<span data-ttu-id="109a5-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="109a5-175">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="109a5-176">プロトコル</span><span class="sxs-lookup"><span data-stu-id="109a5-176">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="109a5-177">C#</span><span class="sxs-lookup"><span data-stu-id="109a5-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="109a5-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="109a5-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="109a5-179">目的-C</span><span class="sxs-lookup"><span data-stu-id="109a5-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="109a5-180">Java</span><span class="sxs-lookup"><span data-stu-id="109a5-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="109a5-181">応答</span><span class="sxs-lookup"><span data-stu-id="109a5-181">Response</span></span>

<span data-ttu-id="109a5-182">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="109a5-182">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
