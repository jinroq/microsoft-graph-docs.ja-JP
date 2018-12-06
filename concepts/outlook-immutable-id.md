---
title: Outlook リソースの不変の識別子を取得します。
description: 'または大きなストレスが発生した可能性があることに気付きませんでしたか、注目に値する動作を outlook のアイテム (メッセージ、イベント、連絡先、タスクなど) がある: その Id を変更します。 しない場合に発生する多くの場合、だけアイテムを移動するが、後で使用できるオフラインの Id を格納するアプリケーションで実際に問題が発生することができます。 不変の識別子は、アイテムの有効期間は変更されませんが、ID を取得するようにアプリケーションを有効にします。'
ms.openlocfilehash: a7b188c968ad6e0bf93f92ec99cb473075f29a4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092514"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="8aa20-105">Outlook リソースの不変の識別子を取得します。</span><span class="sxs-lookup"><span data-stu-id="8aa20-105">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="8aa20-106">または大きなストレスが発生した可能性があることに気付きませんでしたか、注目に値する動作を outlook のアイテム (メッセージ、イベント、連絡先、タスクなど) がある: その Id を変更します。</span><span class="sxs-lookup"><span data-stu-id="8aa20-106">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="8aa20-107">しない場合に発生する多くの場合、だけアイテムを移動するが、後で使用できるオフラインの Id を格納するアプリケーションで実際に問題が発生することができます。</span><span class="sxs-lookup"><span data-stu-id="8aa20-107">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="8aa20-108">不変の識別子は、アイテムの有効期間は変更されませんが、ID を取得するようにアプリケーションを有効にします。</span><span class="sxs-lookup"><span data-stu-id="8aa20-108">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

> <span data-ttu-id="8aa20-109">**重要な:** 不変の識別子は、Microsoft Graph で/beta のバージョンでの使用のみです。</span><span class="sxs-lookup"><span data-stu-id="8aa20-109">**Important:** Immutable identifiers are only avaiable on the /beta version in Microsoft Graph.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="8aa20-110">しくみ</span><span class="sxs-lookup"><span data-stu-id="8aa20-110">How it works</span></span>

<span data-ttu-id="8aa20-111">不変の ID は、Microsoft のグラフのオプション機能です。</span><span class="sxs-lookup"><span data-stu-id="8aa20-111">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="8aa20-112">オプトインすると、アプリケーションは、API 要求に追加の HTTP ヘッダーを送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8aa20-112">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="8aa20-113">このヘッダーに付属しています要求にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="8aa20-113">This header only applies to the request it is included with.</span></span> <span data-ttu-id="8aa20-114">常に不変の Id を使用する場合は、API のすべての要求でこのヘッダーを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="8aa20-114">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="8aa20-115">不変の Id の有効期間</span><span class="sxs-lookup"><span data-stu-id="8aa20-115">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="8aa20-116">アイテムが同じメールボックスに保持している限り、アイテムの変更不可の ID は変更されません。</span><span class="sxs-lookup"><span data-stu-id="8aa20-116">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="8aa20-117">メールボックス内の別のフォルダーにアイテムを移動する場合に、不変の ID が変更されないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="8aa20-117">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="8aa20-118">ただし場合は、不変の ID は変更されます。</span><span class="sxs-lookup"><span data-stu-id="8aa20-118">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="8aa20-119">ユーザーがアーカイブ メールボックスにアイテムを移動します。</span><span class="sxs-lookup"><span data-stu-id="8aa20-119">The user moves the item to an archive mailbox</span></span>
- <span data-ttu-id="8aa20-120">ユーザーが (PST ファイルのメッセージなど) にアイテムをエクスポートし、各自のメールボックスに再インポートすることです。</span><span class="sxs-lookup"><span data-stu-id="8aa20-120">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="8aa20-121">不変の ID をサポートしている項目</span><span class="sxs-lookup"><span data-stu-id="8aa20-121">Items that support immutable ID</span></span>

<span data-ttu-id="8aa20-122">次の項目では、不変の Id をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8aa20-122">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="8aa20-123">メッセージ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8aa20-123">message resource type</span></span>](/graph/api/resources/message?view=graph-rest-beta)
- [<span data-ttu-id="8aa20-124">添付ファイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8aa20-124">attachment resource type</span></span>](/graph/api/resources/attachment?view=graph-rest-beta)
- [<span data-ttu-id="8aa20-125">イベント リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8aa20-125">event resource type</span></span>](/graph/api/resources/event?view=graph-rest-beta)
- [<span data-ttu-id="8aa20-126">eventMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8aa20-126">eventMessage resource type</span></span>](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [<span data-ttu-id="8aa20-127">contact リソース型</span><span class="sxs-lookup"><span data-stu-id="8aa20-127">contact resource type</span></span>](/graph/api/resources/contact?view=graph-rest-beta)
- [<span data-ttu-id="8aa20-128">outlookTask リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8aa20-128">outlookTask resource type</span></span>](/graph/api/resources/outlooktask?view=graph-rest-beta)

<span data-ttu-id="8aa20-129">コンテナーの種類 (mailFolder、予定表など) は、不変の ID をサポートしていませんが、正規の Id の定数が存在しました。</span><span class="sxs-lookup"><span data-stu-id="8aa20-129">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="8aa20-130">変更通知の ID を変更できません。</span><span class="sxs-lookup"><span data-stu-id="8aa20-130">Immutable ID with change notifications</span></span>

<span data-ttu-id="8aa20-131">含めることによって不変の Id での変更通知を送信する Microsoft Graph を要求することができます、`Prefer: IdType="ImmutableId"`ヘッダーと[サブスクリプションを作成](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)します。</span><span class="sxs-lookup"><span data-stu-id="8aa20-131">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span> <span data-ttu-id="8aa20-132">ヘッダーなしで作成された既存のサブスクリプションは、ID の既定の形式を使用する続行されます。</span><span class="sxs-lookup"><span data-stu-id="8aa20-132">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="8aa20-133">不変の Id を使用する既存のサブスクリプションを切り替えるには、削除し、ヘッダーを使用してそれらを再作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8aa20-133">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="8aa20-134">デルタのクエリを使用して ID を変更できません。</span><span class="sxs-lookup"><span data-stu-id="8aa20-134">Immutable ID with delta query</span></span>

<span data-ttu-id="8aa20-135">Microsoft Graph などによってサポートされているリソースの種類の[クエリ応答のデルタ](delta-query-overview.md)に不変の Id を返すことを要求することができます、`Prefer: IdType="ImmutableId"`ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="8aa20-135">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="8aa20-136">`nextLink`と`deltaLink`アプリケーションは、不変の ID の利用を再同期化する必要はありませんので、デルタのクエリによって返される値は両方の ID の形式と互換性のあります。</span><span class="sxs-lookup"><span data-stu-id="8aa20-136">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="8aa20-137">今後、不変の Id を取得するヘッダーを使用することができ、[更新](#updating-existing-data)することできます、アプリケーションのストレージとは別にします。</span><span class="sxs-lookup"><span data-stu-id="8aa20-137">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="8aa20-138">既存データの更新</span><span class="sxs-lookup"><span data-stu-id="8aa20-138">Updating existing data</span></span>

<span data-ttu-id="8aa20-139">既に何千もの正規の Id を格納するデータベースがあれば、 [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta)関数を使用して、変更不可能な形式にこれらの Id を移行できます。</span><span class="sxs-lookup"><span data-stu-id="8aa20-139">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) function.</span></span> <span data-ttu-id="8aa20-140">ターゲット形式に変換するのには Id を 1000 までの配列を提供することができます。</span><span class="sxs-lookup"><span data-stu-id="8aa20-140">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> <span data-ttu-id="8aa20-141">**注:** 使用することができます`translateExchangeIds`Exchange Web サービス アプリケーションは、Microsoft Graph を移行します。</span><span class="sxs-lookup"><span data-stu-id="8aa20-141">**Note:** You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="8aa20-142">例</span><span class="sxs-lookup"><span data-stu-id="8aa20-142">Example</span></span>

<span data-ttu-id="8aa20-143">不変グラフ ID への通常のグラフ ID を変換する次の使用例</span><span class="sxs-lookup"><span data-stu-id="8aa20-143">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="8aa20-144">要求</span><span class="sxs-lookup"><span data-stu-id="8aa20-144">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8aa20-145">応答</span><span class="sxs-lookup"><span data-stu-id="8aa20-145">Response</span></span>

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