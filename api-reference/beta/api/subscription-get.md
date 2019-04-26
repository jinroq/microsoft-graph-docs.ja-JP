---
title: サブスクリプションを取得する
description: サブスクリプションのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 2ed0d30da74859650ef159f264618b0145644d76
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330559"
---
# <a name="get-subscription"></a><span data-ttu-id="00729-103">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="00729-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00729-104">サブスクリプションのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="00729-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="00729-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00729-105">Permissions</span></span>

<span data-ttu-id="00729-106">要求されたリソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、以下の表で指定されているアクセス許可がこの API を呼び出すため必要な最小限の特権となります。</span><span class="sxs-lookup"><span data-stu-id="00729-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="00729-107">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00729-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00729-108">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="00729-108">Supported resource</span></span> | <span data-ttu-id="00729-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00729-109">Delegated (work or school account)</span></span> | <span data-ttu-id="00729-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00729-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00729-111">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00729-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="00729-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="00729-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="00729-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="00729-113">Contacts.Read</span></span> | <span data-ttu-id="00729-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="00729-114">Contacts.Read</span></span> | <span data-ttu-id="00729-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="00729-115">Contacts.Read</span></span> |
|<span data-ttu-id="00729-116">[driveItem](../resources/driveitem.md) (ユーザーの個人用 OneDrive)</span><span class="sxs-lookup"><span data-stu-id="00729-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="00729-117">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="00729-117">Not supported</span></span> | <span data-ttu-id="00729-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00729-118">Files.ReadWrite</span></span> | <span data-ttu-id="00729-119">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="00729-119">Not supported</span></span> |
|<span data-ttu-id="00729-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="00729-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="00729-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00729-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="00729-122">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="00729-122">Not supported</span></span> | <span data-ttu-id="00729-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00729-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="00729-124">イベント</span><span class="sxs-lookup"><span data-stu-id="00729-124">event</span></span>](../resources/event.md) | <span data-ttu-id="00729-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="00729-125">Calendars.Read</span></span> | <span data-ttu-id="00729-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="00729-126">Calendars.Read</span></span> | <span data-ttu-id="00729-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="00729-127">Calendars.Read</span></span> |
|[<span data-ttu-id="00729-128">グループ</span><span class="sxs-lookup"><span data-stu-id="00729-128">group</span></span>](../resources/group.md) | <span data-ttu-id="00729-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="00729-129">Group.Read.All</span></span> | <span data-ttu-id="00729-130">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="00729-130">Not supported</span></span> | <span data-ttu-id="00729-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="00729-131">Group.Read.All</span></span> |
|[<span data-ttu-id="00729-132">グループ会話</span><span class="sxs-lookup"><span data-stu-id="00729-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="00729-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="00729-133">Group.Read.All</span></span> | <span data-ttu-id="00729-134">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="00729-134">Not supported</span></span> | <span data-ttu-id="00729-135">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="00729-135">Not supported</span></span> |
|[<span data-ttu-id="00729-136">メッセージ</span><span class="sxs-lookup"><span data-stu-id="00729-136">message</span></span>](../resources/message.md) | <span data-ttu-id="00729-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="00729-137">Mail.Read</span></span> | <span data-ttu-id="00729-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="00729-138">Mail.Read</span></span> | <span data-ttu-id="00729-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="00729-139">Mail.Read</span></span> |
|[<span data-ttu-id="00729-140">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="00729-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="00729-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00729-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="00729-142">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="00729-142">Not supported</span></span> | <span data-ttu-id="00729-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00729-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="00729-144">ユーザー</span><span class="sxs-lookup"><span data-stu-id="00729-144">user</span></span>](../resources/user.md) | <span data-ttu-id="00729-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="00729-145">User.Read.All</span></span> | <span data-ttu-id="00729-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="00729-146">User.Read.All</span></span> | <span data-ttu-id="00729-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="00729-147">User.Read.All</span></span> |

> <span data-ttu-id="00729-148">**注:** OneDrive と Outlook のアイテムのサブスクリプションについては、追加の制限があります。</span><span class="sxs-lookup"><span data-stu-id="00729-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="00729-149">この制限は、サブスクリプションの作成および管理 (サブスクリプションの取得、更新、削除) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="00729-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="00729-150">個人用 OneDrive では、そのドライブのルート フォルダーまたは任意のサブフォルダーにサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="00729-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="00729-151">OneDrive for Business の場合、サブスクライブできるのはルート フォルダーだけです。</span><span class="sxs-lookup"><span data-stu-id="00729-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="00729-152">サブスクライブしたフォルダー、または階層内の任意のファイル、フォルダー、あるいは他の driveItem オブジェクトの要求された種類の変更について通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="00729-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="00729-153">**ドライブ**、または個々のファイルなどのフォルダーではない **driveItem** インスタンスをサブスクライブすることはできません。</span><span class="sxs-lookup"><span data-stu-id="00729-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="00729-154">Outlook における委任されたアクセス許可では、サインインしているユーザーのメールボックス内のフォルダーにあるアイテムのみをサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="00729-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="00729-155">つまり、委任されたアクセス許可 Calendars.Read を使用して、別のユーザーのメールボックス内のイベントをサブスクライブすることなどはできません。</span><span class="sxs-lookup"><span data-stu-id="00729-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="00729-156">_共有または委任_フォルダーの Outlook 連絡先、イベント、メッセージの変更通知をサブスクライブするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="00729-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="00729-157">対応するアプリケーション アクセス許可を使用して、テナントの_任意_のユーザーのフォルダーまたはメールボックス内にあるアイテムの変更をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="00729-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="00729-158">Outlook 共有アクセス許可 (Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared、および対応する読み取り/書き込み) は使用しないでください。それらは、共有フォルダーまたは委任フォルダーにあるアイテムの変更通知のサブスクライブをサポート**していない**からです。</span><span class="sxs-lookup"><span data-stu-id="00729-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="00729-159">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00729-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00729-160">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="00729-160">Optional query parameters</span></span>

<span data-ttu-id="00729-161">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="00729-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00729-162">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00729-162">Request headers</span></span>

| <span data-ttu-id="00729-163">名前</span><span class="sxs-lookup"><span data-stu-id="00729-163">Name</span></span>       | <span data-ttu-id="00729-164">型</span><span class="sxs-lookup"><span data-stu-id="00729-164">Type</span></span> | <span data-ttu-id="00729-165">説明</span><span class="sxs-lookup"><span data-stu-id="00729-165">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="00729-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="00729-166">Authorization</span></span>  | <span data-ttu-id="00729-167">string</span><span class="sxs-lookup"><span data-stu-id="00729-167">string</span></span>  | <span data-ttu-id="00729-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="00729-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00729-170">要求本文</span><span class="sxs-lookup"><span data-stu-id="00729-170">Request body</span></span>

<span data-ttu-id="00729-171">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="00729-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00729-172">応答</span><span class="sxs-lookup"><span data-stu-id="00729-172">Response</span></span>

<span data-ttu-id="00729-173">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="00729-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00729-174">例</span><span class="sxs-lookup"><span data-stu-id="00729-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="00729-175">要求</span><span class="sxs-lookup"><span data-stu-id="00729-175">Request</span></span>

<span data-ttu-id="00729-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00729-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="00729-177">応答</span><span class="sxs-lookup"><span data-stu-id="00729-177">Response</span></span>

<span data-ttu-id="00729-178">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="00729-178">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
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
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
