---
title: サブスクリプションを取得する
description: サブスクリプションのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c6fe48d3eb72743de368a363330b63976c21156e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271471"
---
# <a name="get-subscription"></a><span data-ttu-id="f945a-103">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="f945a-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f945a-104">サブスクリプションのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="f945a-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="f945a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f945a-105">Permissions</span></span>

<span data-ttu-id="f945a-106">要求されたリソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、以下の表で指定されているアクセス許可がこの API を呼び出すため必要な最小限の特権となります。</span><span class="sxs-lookup"><span data-stu-id="f945a-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="f945a-107">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f945a-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f945a-108">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="f945a-108">Supported resource</span></span> | <span data-ttu-id="f945a-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f945a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f945a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f945a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f945a-111">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f945a-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="f945a-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="f945a-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="f945a-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f945a-113">Contacts.Read</span></span> | <span data-ttu-id="f945a-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f945a-114">Contacts.Read</span></span> | <span data-ttu-id="f945a-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f945a-115">Contacts.Read</span></span> |
|<span data-ttu-id="f945a-116">[driveItem](../resources/driveitem.md) (ユーザーの個人用 OneDrive)</span><span class="sxs-lookup"><span data-stu-id="f945a-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="f945a-117">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f945a-117">Not supported</span></span> | <span data-ttu-id="f945a-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f945a-118">Files.ReadWrite</span></span> | <span data-ttu-id="f945a-119">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f945a-119">Not supported</span></span> |
|<span data-ttu-id="f945a-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="f945a-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="f945a-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f945a-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="f945a-122">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f945a-122">Not supported</span></span> | <span data-ttu-id="f945a-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f945a-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="f945a-124">イベント</span><span class="sxs-lookup"><span data-stu-id="f945a-124">event</span></span>](../resources/event.md) | <span data-ttu-id="f945a-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f945a-125">Calendars.Read</span></span> | <span data-ttu-id="f945a-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f945a-126">Calendars.Read</span></span> | <span data-ttu-id="f945a-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f945a-127">Calendars.Read</span></span> |
|[<span data-ttu-id="f945a-128">グループ</span><span class="sxs-lookup"><span data-stu-id="f945a-128">group</span></span>](../resources/group.md) | <span data-ttu-id="f945a-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f945a-129">Group.Read.All</span></span> | <span data-ttu-id="f945a-130">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f945a-130">Not supported</span></span> | <span data-ttu-id="f945a-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f945a-131">Group.Read.All</span></span> |
|[<span data-ttu-id="f945a-132">グループ会話</span><span class="sxs-lookup"><span data-stu-id="f945a-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="f945a-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f945a-133">Group.Read.All</span></span> | <span data-ttu-id="f945a-134">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f945a-134">Not supported</span></span> | <span data-ttu-id="f945a-135">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f945a-135">Not supported</span></span> |
|[<span data-ttu-id="f945a-136">メッセージ</span><span class="sxs-lookup"><span data-stu-id="f945a-136">message</span></span>](../resources/message.md) | <span data-ttu-id="f945a-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f945a-137">Mail.Read</span></span> | <span data-ttu-id="f945a-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f945a-138">Mail.Read</span></span> | <span data-ttu-id="f945a-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f945a-139">Mail.Read</span></span> |
|[<span data-ttu-id="f945a-140">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="f945a-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="f945a-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f945a-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="f945a-142">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f945a-142">Not supported</span></span> | <span data-ttu-id="f945a-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f945a-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="f945a-144">ユーザー</span><span class="sxs-lookup"><span data-stu-id="f945a-144">user</span></span>](../resources/user.md) | <span data-ttu-id="f945a-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f945a-145">User.Read.All</span></span> | <span data-ttu-id="f945a-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f945a-146">User.Read.All</span></span> | <span data-ttu-id="f945a-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f945a-147">User.Read.All</span></span> |

> <span data-ttu-id="f945a-148">**注:** OneDrive と Outlook のアイテムのサブスクリプションについては、追加の制限があります。</span><span class="sxs-lookup"><span data-stu-id="f945a-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="f945a-149">この制限は、サブスクリプションの作成および管理 (サブスクリプションの取得、更新、削除) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="f945a-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="f945a-150">個人用 OneDrive では、そのドライブのルート フォルダーまたは任意のサブフォルダーにサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="f945a-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="f945a-151">OneDrive for Business の場合、サブスクライブできるのはルート フォルダーだけです。</span><span class="sxs-lookup"><span data-stu-id="f945a-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="f945a-152">サブスクライブしたフォルダー、または階層内の任意のファイル、フォルダー、あるいは他の driveItem オブジェクトの要求された種類の変更について通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="f945a-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="f945a-153">**ドライブ**、または個々のファイルなどのフォルダーではない **driveItem** インスタンスをサブスクライブすることはできません。</span><span class="sxs-lookup"><span data-stu-id="f945a-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="f945a-154">Outlook における委任されたアクセス許可では、サインインしているユーザーのメールボックス内のフォルダーにあるアイテムのみをサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="f945a-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="f945a-155">つまり、委任されたアクセス許可 Calendars.Read を使用して、別のユーザーのメールボックス内のイベントをサブスクライブすることなどはできません。</span><span class="sxs-lookup"><span data-stu-id="f945a-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="f945a-156">_共有または委任_フォルダーの Outlook 連絡先、イベント、メッセージの変更通知をサブスクライブするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="f945a-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="f945a-157">対応するアプリケーション アクセス許可を使用して、テナントの_任意_のユーザーのフォルダーまたはメールボックス内にあるアイテムの変更をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="f945a-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="f945a-158">Outlook 共有アクセス許可 (Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared、および対応する読み取り/書き込み) は使用しないでください。それらは、共有フォルダーまたは委任フォルダーにあるアイテムの変更通知のサブスクライブをサポート**していない**からです。</span><span class="sxs-lookup"><span data-stu-id="f945a-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="f945a-159">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f945a-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f945a-160">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f945a-160">Optional query parameters</span></span>

<span data-ttu-id="f945a-161">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f945a-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f945a-162">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f945a-162">Request headers</span></span>

| <span data-ttu-id="f945a-163">名前</span><span class="sxs-lookup"><span data-stu-id="f945a-163">Name</span></span>       | <span data-ttu-id="f945a-164">型</span><span class="sxs-lookup"><span data-stu-id="f945a-164">Type</span></span> | <span data-ttu-id="f945a-165">説明</span><span class="sxs-lookup"><span data-stu-id="f945a-165">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="f945a-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="f945a-166">Authorization</span></span>  | <span data-ttu-id="f945a-167">string</span><span class="sxs-lookup"><span data-stu-id="f945a-167">string</span></span>  | <span data-ttu-id="f945a-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f945a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f945a-170">要求本文</span><span class="sxs-lookup"><span data-stu-id="f945a-170">Request body</span></span>

<span data-ttu-id="f945a-171">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f945a-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f945a-172">応答</span><span class="sxs-lookup"><span data-stu-id="f945a-172">Response</span></span>

<span data-ttu-id="f945a-173">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f945a-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f945a-174">例</span><span class="sxs-lookup"><span data-stu-id="f945a-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f945a-175">要求</span><span class="sxs-lookup"><span data-stu-id="f945a-175">Request</span></span>

<span data-ttu-id="f945a-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f945a-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="f945a-177">応答</span><span class="sxs-lookup"><span data-stu-id="f945a-177">Response</span></span>

<span data-ttu-id="f945a-178">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f945a-178">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f945a-179">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f945a-179">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f945a-180">C#</span><span class="sxs-lookup"><span data-stu-id="f945a-180">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscription-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f945a-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="f945a-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscription-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f945a-182">目的-C</span><span class="sxs-lookup"><span data-stu-id="f945a-182">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_subscription-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
