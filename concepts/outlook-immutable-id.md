---
title: Outlook リソースの不変 ID の取得
description: Outlook アイテム (メッセージ、イベント、連絡先、タスク) には、ユーザーは気づいていないか、大きな不満を感じている可能性のある、興味深い動作があります。それは、ID の変更です。 これは頻繁に発生するものではなく、アイテムが移動された場合のみ発生します。ただし、後で使用するために ID をオフラインで格納するアプリの場合、これは深刻な問題になることがあります。 不変 ID を使用すると、お使いのアプリケーションで、アイテムの有効期間中は変更のない ID を取得できます。
ms.openlocfilehash: a7b188c968ad6e0bf93f92ec99cb473075f29a4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092514"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="457b4-105">Outlook リソースの不変 ID の取得</span><span class="sxs-lookup"><span data-stu-id="457b4-105">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="457b4-106">Outlook アイテム (メッセージ、イベント、連絡先、タスク) には、ユーザーは気づいていないか、大きな不満を感じている可能性のある、興味深い動作があります。それは、ID の変更です。</span><span class="sxs-lookup"><span data-stu-id="457b4-106">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="457b4-107">これは頻繁に発生するものではなく、アイテムが移動された場合のみ発生します。ただし、後で使用するために ID をオフラインで格納するアプリの場合、これは深刻な問題になることがあります。</span><span class="sxs-lookup"><span data-stu-id="457b4-107">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="457b4-108">不変 ID を使用すると、お使いのアプリケーションで、アイテムの有効期間中は変更のない ID を取得できます。</span><span class="sxs-lookup"><span data-stu-id="457b4-108">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

> <span data-ttu-id="457b4-109">**重要:** 不変 ID は、Microsoft Graph のベータ版のみで使用できます。</span><span class="sxs-lookup"><span data-stu-id="457b4-109">**Important:** Immutable identifiers are only avaiable on the /beta version in Microsoft Graph.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="457b4-110">しくみ</span><span class="sxs-lookup"><span data-stu-id="457b4-110">How it works</span></span>

<span data-ttu-id="457b4-111">不変 ID は、Microsoft Graph のオプション機能です。</span><span class="sxs-lookup"><span data-stu-id="457b4-111">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="457b4-112">オプト インするには、アプリケーションから、API 要求に追加の HTTP ヘッダーを含めて送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="457b4-112">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="457b4-113">このヘッダーは、それが含まれる要求にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="457b4-113">This header only applies to the request it is included with.</span></span> <span data-ttu-id="457b4-114">常に不変 ID を使用したい場合は、このヘッダーをすべての API 要求に含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="457b4-114">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="457b4-115">不変 ID の有効期間</span><span class="sxs-lookup"><span data-stu-id="457b4-115">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="457b4-116">アイテムの不変 ID は、アイテムが同じメールボックス内にある限り、変更されません。</span><span class="sxs-lookup"><span data-stu-id="457b4-116">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="457b4-117">つまり、アイテムがメールボックス内の別のフォルダーに移動しても、不変 ID は変更されません。</span><span class="sxs-lookup"><span data-stu-id="457b4-117">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="457b4-118">ただし、次の場合、不変 ID は変更されます。</span><span class="sxs-lookup"><span data-stu-id="457b4-118">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="457b4-119">ユーザーがアイテムをアーカイブ メールボックスに移動した</span><span class="sxs-lookup"><span data-stu-id="457b4-119">The user moves the item to an archive mailbox</span></span>
- <span data-ttu-id="457b4-120">ユーザーがアイテムをエクスポートし (PST へのエクスポート、MSG ファイルとしてのエクスポートなど)、それをメールボックスに再度インポートした</span><span class="sxs-lookup"><span data-stu-id="457b4-120">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="457b4-121">不変 ID をサポートするアイテム</span><span class="sxs-lookup"><span data-stu-id="457b4-121">Items that support immutable ID</span></span>

<span data-ttu-id="457b4-122">不変 ID をサポートするアイテムは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="457b4-122">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="457b4-123">message リソース型</span><span class="sxs-lookup"><span data-stu-id="457b4-123">message resource type</span></span>](/graph/api/resources/message?view=graph-rest-beta)
- [<span data-ttu-id="457b4-124">attachment リソース型</span><span class="sxs-lookup"><span data-stu-id="457b4-124">attachment resource type</span></span>](/graph/api/resources/attachment?view=graph-rest-beta)
- [<span data-ttu-id="457b4-125">event リソース型</span><span class="sxs-lookup"><span data-stu-id="457b4-125">event resource type</span></span>](/graph/api/resources/event?view=graph-rest-beta)
- [<span data-ttu-id="457b4-126">eventMessage リソース型</span><span class="sxs-lookup"><span data-stu-id="457b4-126">eventMessage resource type</span></span>](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [<span data-ttu-id="457b4-127">contact リソース型</span><span class="sxs-lookup"><span data-stu-id="457b4-127">contact resource type</span></span>](/graph/api/resources/contact?view=graph-rest-beta)
- [<span data-ttu-id="457b4-128">outlookTask リソース型</span><span class="sxs-lookup"><span data-stu-id="457b4-128">outlookTask resource type</span></span>](/graph/api/resources/outlooktask?view=graph-rest-beta)

<span data-ttu-id="457b4-129">コンテナー型 (mailFolder、calendar など) は不変 ID をサポートしませんが、コンテナー型の標準 ID は既に不変です。</span><span class="sxs-lookup"><span data-stu-id="457b4-129">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="457b4-130">変更通知を使用する不変 ID</span><span class="sxs-lookup"><span data-stu-id="457b4-130">Immutable ID with change notifications</span></span>

<span data-ttu-id="457b4-131">[サブスクリプションの作成](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)時に `Prefer: IdType="ImmutableId"`ヘッダーを含めることで、Microsoft Graph が変更通知で不変 ID を送信するように要求することができます。</span><span class="sxs-lookup"><span data-stu-id="457b4-131">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span> <span data-ttu-id="457b4-132">このヘッダーなしで作成された既存のサブスクリプションは、既定の ID 形式を使用し続けます。</span><span class="sxs-lookup"><span data-stu-id="457b4-132">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="457b4-133">既存のサブスクリプションを、不変 ID を使用するように切り替えるには、そのサブスクリプションを削除し、このヘッダーを使用して作成し直す必要があります。</span><span class="sxs-lookup"><span data-stu-id="457b4-133">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="457b4-134">デルタ クエリを使用する不変 ID</span><span class="sxs-lookup"><span data-stu-id="457b4-134">Immutable ID with delta query</span></span>

<span data-ttu-id="457b4-135">`Prefer: IdType="ImmutableId"` ヘッダーを含めることで、Microsoft Graph が不変 ID を、サポートされるリソース型に関する[デルタ クエリ応答](delta-query-overview.md)で返すように要求することができます。</span><span class="sxs-lookup"><span data-stu-id="457b4-135">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="457b4-136">デルタ クエリによって返される `nextLink` と `deltaLink` の各値は、両方の ID 形式に対応しているので、アプリケーションは、不変 ID を利用するために再同期する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="457b4-136">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="457b4-137">今後は、このヘッダーを使用して不変 ID を取得でき、[アプリの記憶域を個別に更新する](#updating-existing-data)ことができます。</span><span class="sxs-lookup"><span data-stu-id="457b4-137">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="457b4-138">既存のデータの更新</span><span class="sxs-lookup"><span data-stu-id="457b4-138">Updating existing data</span></span>

<span data-ttu-id="457b4-139">データベースが既に何千個もの標準 ID でいっぱいになっている場合、[translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) 関数を使用して、それらの ID を不変形式に移行することができます。</span><span class="sxs-lookup"><span data-stu-id="457b4-139">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) function.</span></span> <span data-ttu-id="457b4-140">最大 1000 個もの ID をターゲット形式に変換できます。</span><span class="sxs-lookup"><span data-stu-id="457b4-140">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> <span data-ttu-id="457b4-141">**注:** `translateExchangeIds` を使用して、Exchange Web サービス アプリケーションを Microsoft Graph に移行することもできます。</span><span class="sxs-lookup"><span data-stu-id="457b4-141">**Note:** You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="457b4-142">例</span><span class="sxs-lookup"><span data-stu-id="457b4-142">Example</span></span>

<span data-ttu-id="457b4-143">次の例では、標準の Graph ID を不変の Graph ID に変換します。</span><span class="sxs-lookup"><span data-stu-id="457b4-143">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="457b4-144">要求</span><span class="sxs-lookup"><span data-stu-id="457b4-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a><span data-ttu-id="457b4-145">応答</span><span class="sxs-lookup"><span data-stu-id="457b4-145">Response</span></span>

```http
HTTP 200 OK

{
  "value": [
    {
      "targetId": "AAkALgAA...",
      "sourceId": "AQMkAGM2..."
    }
  ]
}
```