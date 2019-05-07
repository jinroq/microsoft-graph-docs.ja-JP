---
title: Azure AD Graph と Microsoft Graph の機能の違い
description: アプリをすばやく簡単に移行できるように、Azure Active Directory (Azure AD) API と Microsoft Graph API の機能の違いについて説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e18bc286f4373c15da9d6a2360491e1b2f0371f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630245"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="c483b-103">Azure AD Graph と Microsoft Graph の機能の違い</span><span class="sxs-lookup"><span data-stu-id="c483b-103">Feature differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="c483b-104">この記事は、*手順 1:* [アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の API の相違点を確認します。</span><span class="sxs-lookup"><span data-stu-id="c483b-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="c483b-105">Microsoft Graph の多くの機能は、Azure AD Graph に対応しています。</span><span class="sxs-lookup"><span data-stu-id="c483b-105">Many features in Microsoft Graph work similarly to their Azure AD Graph counterparts.</span></span> <span data-ttu-id="c483b-106">ただし、いくつかの変更や改善が行われています。</span><span class="sxs-lookup"><span data-stu-id="c483b-106">However, a few have been changed and/or improved.</span></span> <span data-ttu-id="c483b-107">ここでは、これらの違いを活用するようにアプリを調整する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="c483b-107">Here, you'll learn how to adapt your apps to take advantage of these differences.</span></span>  <span data-ttu-id="c483b-108">多くの場合、変更は軽微ですが、労力を費やす価値があります。</span><span class="sxs-lookup"><span data-stu-id="c483b-108">Frequently, the changes are minor, but well worth the effort.</span></span>

<span data-ttu-id="c483b-109">この記事では、Microsoft Graph の処理方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="c483b-109">This article explores how Microsoft Graph handles:</span></span>

- <span data-ttu-id="c483b-110">ディレクトリ スキーマの拡張</span><span class="sxs-lookup"><span data-stu-id="c483b-110">Directory schema extensions</span></span>
- <span data-ttu-id="c483b-111">差分クエリ</span><span class="sxs-lookup"><span data-stu-id="c483b-111">Differential queries</span></span>
- <span data-ttu-id="c483b-112">バッチ処理</span><span class="sxs-lookup"><span data-stu-id="c483b-112">Batching</span></span>

## <a name="directory-schema-extensions"></a><span data-ttu-id="c483b-113">ディレクトリ スキーマの拡張</span><span class="sxs-lookup"><span data-stu-id="c483b-113">Directory schema extensions</span></span>

<span data-ttu-id="c483b-114">アプリで Azure AD Graph ディレクトリスキーマ拡張機能を使用している場合は、次のように、同じ基本 Api (Microsoft Graph 要求 Url を使用) を引き続き使用できます。</span><span class="sxs-lookup"><span data-stu-id="c483b-114">If your app uses Azure AD Graph directory schema extensions, you can continue to use the same basic APIs (with Microsoft Graph request URLs) to:</span></span>

- <span data-ttu-id="c483b-115">GET とを使用して拡張機能の値を読み取る`$select`</span><span class="sxs-lookup"><span data-stu-id="c483b-115">Read extension values using GET and `$select`</span></span>
- <span data-ttu-id="c483b-116">GET とを使用して拡張機能値を検索する`$filter`</span><span class="sxs-lookup"><span data-stu-id="c483b-116">Search on extension values using GET and `$filter`</span></span>
- <span data-ttu-id="c483b-117">PATCH を使用して拡張機能の値を更新する</span><span class="sxs-lookup"><span data-stu-id="c483b-117">Update extension values using PATCH</span></span>
- <span data-ttu-id="c483b-118">PATCH を使用して拡張機能の値を削除する ( **null**に設定)</span><span class="sxs-lookup"><span data-stu-id="c483b-118">Remove extension values using PATCH (set to **null**)</span></span>

<span data-ttu-id="c483b-119">ただし、Microsoft Graph では、Azure AD Graph ディレクトリのスキーマ拡張機能の定義を管理したり、テナントで使用可能なすべてのスキーマ拡張機能の定義を表示したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="c483b-119">However, Microsoft Graph doesn't provide a way to manage Azure AD Graph directory schema extension definitions or to view all schema extension definitions available in a tenant.</span></span>

<span data-ttu-id="c483b-120">代わりに、Microsoft Graph は、拡張可能なスキーマ拡張機能を提供します。ここでは、Azure AD Graph ディレクトリスキーマの extentions との下位互換性がありません。</span><span class="sxs-lookup"><span data-stu-id="c483b-120">Instead, Microsoft Graph provides an enhanced schema extensions developer experience, which today is not backwards compatible with Azure AD Graph directory schema extentions.</span></span> <span data-ttu-id="c483b-121">詳細については、「 [add custom data」の「スキーマ拡張機能](/graph/extensibility-overview#schema-extensions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c483b-121">To learn more, see [schema extensions in add custom data](/graph/extensibility-overview#schema-extensions).</span></span>

### <a name="recommended-migration-approach"></a><span data-ttu-id="c483b-122">推奨される移行方法</span><span class="sxs-lookup"><span data-stu-id="c483b-122">Recommended migration approach</span></span>

<span data-ttu-id="c483b-123">Azure AD Graph アプリがディレクトリスキーマ拡張機能を使用している場合は、アプリを Microsoft Graph に移行するための段階的なアプローチを取ります。</span><span class="sxs-lookup"><span data-stu-id="c483b-123">If your Azure AD Graph app uses directory schema extensions, take an incremental approach to migrate the app to Microsoft Graph.</span></span>

<span data-ttu-id="c483b-124">最初に、アプリを Microsoft Graph API 呼び出しを使用するように切り替えますが、アプリは Azure AD Graph ディレクトリスキーマ拡張機能を引き続き利用できます。</span><span class="sxs-lookup"><span data-stu-id="c483b-124">First, switch your app to using Microsoft Graph API calls, but let the app continue to leverage Azure AD Graph directory schema extensions.</span></span>

<span data-ttu-id="c483b-125">その後、Microsoft Graph スキーマ拡張機能の使用に切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="c483b-125">Then, you can switch to using Microsoft Graph schema extensions.</span></span> <span data-ttu-id="c483b-126">場合によっては、切り替えは適切ではありません。</span><span class="sxs-lookup"><span data-stu-id="c483b-126">In some cases, switching will not be appropriate.</span></span> <span data-ttu-id="c483b-127">次の場合に切り替えません。</span><span class="sxs-lookup"><span data-stu-id="c483b-127">Do not switch if:</span></span>

- <span data-ttu-id="c483b-128">アプリは AD Connect によって作成されたディレクトリスキーマ拡張機能を使用します。</span><span class="sxs-lookup"><span data-stu-id="c483b-128">Your app uses directory schema extensions created through AD Connect, or</span></span>
- <span data-ttu-id="c483b-129">アプリは、トークンクレームのディレクトリスキーマ拡張値に依存します。</span><span class="sxs-lookup"><span data-stu-id="c483b-129">Your app relies on directory schema extension values in token claims.</span></span>

><span data-ttu-id="c483b-130">**注**: Microsoft Graph スキーマ拡張プロパティを、オプションのクレームを使用してトークン内のクレームとして使用することもまだサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c483b-130">**NOTE**: Using Microsoft Graph schema extension properties as claims in a token using optional claims is also not yet supported.</span></span>

<span data-ttu-id="c483b-131">新しい Microsoft Graph スキーマ拡張モデルに切り替えるには、次の操作を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="c483b-131">To switch to the newer Microsoft Graph schema extension model, you'll need to:</span></span>

- <span data-ttu-id="c483b-132">Microsoft Graph を使用して、新しいスキーマ拡張機能の定義を定義します。</span><span class="sxs-lookup"><span data-stu-id="c483b-132">Define new schema extension definitions using Microsoft Graph.</span></span>
- <span data-ttu-id="c483b-133">新しいスキーマ拡張機能の定義をサポートするようにアプリを更新します。</span><span class="sxs-lookup"><span data-stu-id="c483b-133">Update the app to support the new schema extension definitions.</span></span>
- <span data-ttu-id="c483b-134">Azure AD スキーマ拡張機能のプロパティから新しい Microsoft Graph スキーマ拡張プロパティにデータを移行します。</span><span class="sxs-lookup"><span data-stu-id="c483b-134">Migrate the data from the Azure AD schema extension properties to the new Microsoft Graph schema extension properties.</span></span>  <span data-ttu-id="c483b-135">データの自動移行はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c483b-135">Automatic migration of data is not supported.</span></span>

## <a name="differential-queries"></a><span data-ttu-id="c483b-136">差分クエリ</span><span class="sxs-lookup"><span data-stu-id="c483b-136">Differential queries</span></span>

<span data-ttu-id="c483b-137">Azure AD Graph と Microsoft Graph では、クエリを使用して変更を追跡できます。</span><span class="sxs-lookup"><span data-stu-id="c483b-137">Azure AD Graph and Microsoft Graph let you track changes using queries.</span></span>  <span data-ttu-id="c483b-138">高レベルの方法は、2つの Api 間で似ていますが、構文が異なります。</span><span class="sxs-lookup"><span data-stu-id="c483b-138">The high-level approach is similar between the two APIs, but the syntax is different.</span></span>  

<span data-ttu-id="c483b-139">Azure AD Graph は、これらの差分クエリを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="c483b-139">Azure AD Graph calls these differential queries.</span></span>  <span data-ttu-id="c483b-140">Microsoft Graph では、これらは[デルタクエリ](/graph/delta-query-overview)です。</span><span class="sxs-lookup"><span data-stu-id="c483b-140">In Microsoft Graph, they're [delta queries](/graph/delta-query-overview).</span></span>

<span data-ttu-id="c483b-141">次の表では、主な類似点と相違点について取り上げます。</span><span class="sxs-lookup"><span data-stu-id="c483b-141">The following table highlights key similarities and differences:</span></span>

||<span data-ttu-id="c483b-142">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="c483b-142">Azure AD Graph</span></span> | <span data-ttu-id="c483b-143">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c483b-143">Microsoft Graph</span></span> |
|----|----|----|
| <span data-ttu-id="c483b-144">_最初のデータ要求_</span><span class="sxs-lookup"><span data-stu-id="c483b-144">_Initial data request_</span></span> | <span data-ttu-id="c483b-145">クエリパラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="c483b-145">Uses a query parameter:</span></span><br>`GET /groups?deltaLink=` | <span data-ttu-id="c483b-146">関数を使用します。</span><span class="sxs-lookup"><span data-stu-id="c483b-146">Uses a function:</span></span> <br> `GET /groups/delta` |
| <span data-ttu-id="c483b-147">_新しい変更を取得する_</span><span class="sxs-lookup"><span data-stu-id="c483b-147">_Get new changes_</span></span> | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| <span data-ttu-id="c483b-148">_今すぐ同期_</span><span class="sxs-lookup"><span data-stu-id="c483b-148">_Sync from now_</span></span> |<span data-ttu-id="c483b-149">カスタム HTTP ヘッダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="c483b-149">Uses a custom HTTP header:</span></span><br> `ocp-aad-dq-include-only-delta-token: true` | <span data-ttu-id="c483b-150">クエリパラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="c483b-150">Uses a query parameter:</span></span> <br> `GET /groups/delta?$deltaToken=latest` |
| <span data-ttu-id="c483b-151">_DirectoryObjects の変更を追跡する_</span><span class="sxs-lookup"><span data-stu-id="c483b-151">_Track changes for directoryObjects_</span></span> | <span data-ttu-id="c483b-152">同じ操作で複数のリソース (ユーザーとグループ) の変更を取得します。&nbsp;&nbsp;</span><span class="sxs-lookup"><span data-stu-id="c483b-152">Gets changes for multiple resource (user and group) in the same operation:&nbsp;&nbsp;</span></span><br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | <span data-ttu-id="c483b-153">は、Microsoft Graph で個別のクエリを使用し、1つはリソースごとに使用します。</span><span class="sxs-lookup"><span data-stu-id="c483b-153">Uses separate queries with Microsoft Graph, one for each resource.</span></span> |
| <span data-ttu-id="c483b-154">_リソースおよびリレーションシップの変更を取得する_</span><span class="sxs-lookup"><span data-stu-id="c483b-154">_Get resource and relationship changes_</span></span> | <span data-ttu-id="c483b-155">リソースがリレーションシップを持っている場合、すべての要求はリソースおよびリレーションシップの変更を返します。</span><span class="sxs-lookup"><span data-stu-id="c483b-155">All requests return resource and relationship changes, if the resource has relationships.</span></span> | `GET /groups/delta?$expand=members` |
| <span data-ttu-id="c483b-156">_新規および変更されたアイテムを示す応答_</span><span class="sxs-lookup"><span data-stu-id="c483b-156">_Response indicating new and changed items_</span></span> | <ul><li><p><span data-ttu-id="c483b-157">標準表現を使用して、新しく作成されたインスタンスを表します。</span><span class="sxs-lookup"><span data-stu-id="c483b-157">Represents newly created instances using their standard representation.</span></span></p></li><li><p><span data-ttu-id="c483b-158">更新されたインスタンスは、*少なく*とも更新されたプロパティを持つ id で表されます。</span><span class="sxs-lookup"><span data-stu-id="c483b-158">Updated instances are represented by their id with *at least* the properties that have been updated.</span></span> <span data-ttu-id="c483b-159">その他のプロパティが含まれている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c483b-159">Other properties may be included.</span></span></p></li><li><p><span data-ttu-id="c483b-160">リレーションシップは、 `directoryLinkChange`型として表されます。</span><span class="sxs-lookup"><span data-stu-id="c483b-160">Relationships are represented as the `directoryLinkChange` type.</span></span></p></li></ul>|<ul><li><p><span data-ttu-id="c483b-161">標準表現を使用して、新しく作成されたインスタンスを表します。</span><span class="sxs-lookup"><span data-stu-id="c483b-161">Represents newly created instances using their standard representation.</span></span></p></li><li><p><span data-ttu-id="c483b-162">更新されたインスタンスは、*少なく*とも更新されたプロパティを持つ id で表されます。</span><span class="sxs-lookup"><span data-stu-id="c483b-162">Updated instances are represented by their id with *at least* the properties that have been updated.</span></span> <span data-ttu-id="c483b-163">その他のプロパティが含まれている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c483b-163">Other properties may be included.</span></span></p></li><li><p><span data-ttu-id="c483b-164">リレーションシップは、標準のリソース表現における注釈として表されます。</span><span class="sxs-lookup"><span data-stu-id="c483b-164">Relationships are represented as annotations on the standard resource representation.</span></span> <span data-ttu-id="c483b-165">これらの注釈は、 `propertyName@delta`グループのメンバーシップ`members@delta`の変更などの形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="c483b-165">These annotations use the format `propertyName@delta`, for example `members@delta` for a group's membership changes.</span></span></p></li></ul> |
| <span data-ttu-id="c483b-166">_削除済みアイテムを示す応答_</span><span class="sxs-lookup"><span data-stu-id="c483b-166">_Response indicating  deleted items_</span></span>| <span data-ttu-id="c483b-167">*Aad*が true に設定された追加のプロパティを持つ削除済みアイテムがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="c483b-167">Indicates a deleted item with an additional property of *aad.isDeleted* set to true.</span></span> | <span data-ttu-id="c483b-168">削除された注釈が\@含まれる削除済みアイテムを示します。</span><span class="sxs-lookup"><span data-stu-id="c483b-168">Indicates a deleted item with the \@removed annotation.</span></span> <span data-ttu-id="c483b-169">また、アイテムが削除された場合でも、復元できるかどうか、または完全に削除されているかどうかを示す理由コードが含まれている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c483b-169">It may also contain a reason code, which indicates if the item is deleted, but can be restored, or is permanently deleted.</span></span> |

<span data-ttu-id="c483b-170">アプリに既に状態データが格納されている場合は、前に示した「今すぐ同期」を使用して、デルタクエリへの移行を管理することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="c483b-170">If your app is already storing state data, consider using the "sync from now" shown earlier to help manage the transition to delta queries.</span></span>

## <a name="batching"></a><span data-ttu-id="c483b-171">バッチ処理</span><span class="sxs-lookup"><span data-stu-id="c483b-171">Batching</span></span>

<span data-ttu-id="c483b-172">Azure AD Graph は、マルチパート MIME メッセージと呼ばれるシステムを使用して、バッチ処理を管理しています。</span><span class="sxs-lookup"><span data-stu-id="c483b-172">Azure AD Graph used a system called multi-part MIME messages to manage batching.</span></span>  <span data-ttu-id="c483b-173">Microsoft Graph では、1回のバッチ操作で最大20個の要求を許可するために、 [JSON バッチ](json-batching.md)処理を使用します。</span><span class="sxs-lookup"><span data-stu-id="c483b-173">Microsoft Graph uses [JSON batching](json-batching.md) to permit up to 20 requests in a single batch operation.</span></span> <span data-ttu-id="c483b-174">JSON のバッチ処理機構は、特に JSON 解析ライブラリと組み合わせて使用する方がはるかに簡単です。</span><span class="sxs-lookup"><span data-stu-id="c483b-174">The JSON batching mechanism is significantly simpler to use, especially together with JSON parsing libraries.</span></span>  <span data-ttu-id="c483b-175">また、バッチ処理を順序付けることもできます。</span><span class="sxs-lookup"><span data-stu-id="c483b-175">It also allows for sequencing batch operations.</span></span>  <span data-ttu-id="c483b-176">ただし、Azure AD Graph のバッチ処理方法との下位互換性はありません。</span><span class="sxs-lookup"><span data-stu-id="c483b-176">However, it is not backwards compatible with the Azure AD Graph batching approach.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c483b-177">次のステップ</span><span class="sxs-lookup"><span data-stu-id="c483b-177">Next Steps</span></span>

- <span data-ttu-id="c483b-178">Azure AD Graph と Microsoft Graph の[リソースの相違点](migrate-azure-ad-graph-resource-differences.md)について説明します。</span><span class="sxs-lookup"><span data-stu-id="c483b-178">Learn about [resource differences](migrate-azure-ad-graph-resource-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="c483b-179">[開く] [[カスタムデータの追加](/graph/extensibility-overview)] を参照して、オープンおよびスキーマの拡張機能に関する情報を確認します</span><span class="sxs-lookup"><span data-stu-id="c483b-179">Explore [add custom data](/graph/extensibility-overview) for information about open and schema extensions.</span></span>
- <span data-ttu-id="c483b-180">[デルタクエリ](/graph/delta-query-overview)を調査して、Microsoft Graph の差分クエリのバージョンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c483b-180">Explore [delta queries](/graph/delta-query-overview) to learn about Microsoft Graph's version of differential query.</span></span>
- <span data-ttu-id="c483b-181">Microsoft Graph でのバッチ処理の動作を理解するために、 [JSON バッチ](json-batching.md)を調査します。</span><span class="sxs-lookup"><span data-stu-id="c483b-181">Explore [JSON batching](json-batching.md) to understand how batching works in Microsoft Graph.</span></span>
- <span data-ttu-id="c483b-182">[Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="c483b-182">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->
