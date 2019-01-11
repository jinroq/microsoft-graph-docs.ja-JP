---
title: contact リソース型
description: 連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 6ff19278e6cf120404b892bb95881326ce281a72
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854377"
---
# <a name="contact-resource-type"></a><span data-ttu-id="74dff-104">contact リソース型</span><span class="sxs-lookup"><span data-stu-id="74dff-104">contact resource type</span></span>

<span data-ttu-id="74dff-p102">連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。</span><span class="sxs-lookup"><span data-stu-id="74dff-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="74dff-107">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="74dff-107">This resource supports:</span></span>

- <span data-ttu-id="74dff-108">[拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="74dff-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="74dff-109">[変更通知](/graph/webhooks)にサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="74dff-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="74dff-110">[デルタ](../api/contact-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="74dff-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="74dff-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="74dff-111">Methods</span></span>

| <span data-ttu-id="74dff-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="74dff-112">Method</span></span>       | <span data-ttu-id="74dff-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="74dff-113">Return Type</span></span>  |<span data-ttu-id="74dff-114">説明</span><span class="sxs-lookup"><span data-stu-id="74dff-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74dff-115">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="74dff-115">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="74dff-116">contact</span><span class="sxs-lookup"><span data-stu-id="74dff-116">contact</span></span>](contact.md) |<span data-ttu-id="74dff-117">連絡先オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="74dff-117">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="74dff-118">作成</span><span class="sxs-lookup"><span data-stu-id="74dff-118">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="74dff-119">contact</span><span class="sxs-lookup"><span data-stu-id="74dff-119">contact</span></span>](contact.md) |<span data-ttu-id="74dff-120">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="74dff-120">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="74dff-121">更新する</span><span class="sxs-lookup"><span data-stu-id="74dff-121">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="74dff-122">contact</span><span class="sxs-lookup"><span data-stu-id="74dff-122">contact</span></span>](contact.md) |<span data-ttu-id="74dff-123">連絡先オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="74dff-123">Update contact object.</span></span> |
|[<span data-ttu-id="74dff-124">削除</span><span class="sxs-lookup"><span data-stu-id="74dff-124">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="74dff-125">なし</span><span class="sxs-lookup"><span data-stu-id="74dff-125">None</span></span> |<span data-ttu-id="74dff-126">連絡先オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="74dff-126">Delete contact object.</span></span> |
|[<span data-ttu-id="74dff-127">delta</span><span class="sxs-lookup"><span data-stu-id="74dff-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="74dff-128">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="74dff-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="74dff-129">指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="74dff-129">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="74dff-130">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="74dff-130">**Open extensions**</span></span>| | |
|[<span data-ttu-id="74dff-131">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="74dff-131">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="74dff-132">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="74dff-132">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="74dff-133">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="74dff-133">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="74dff-134">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="74dff-134">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="74dff-135">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="74dff-135">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="74dff-136">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="74dff-136">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="74dff-137">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="74dff-137">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="74dff-138">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="74dff-138">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="74dff-139">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="74dff-139">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="74dff-140">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="74dff-140">**Extended properties**</span></span>| | |
|[<span data-ttu-id="74dff-141">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="74dff-141">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="74dff-142">contact</span><span class="sxs-lookup"><span data-stu-id="74dff-142">contact</span></span>](contact.md)  |<span data-ttu-id="74dff-143">新規または既存の連絡先に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="74dff-143">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="74dff-144">単一値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="74dff-144">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="74dff-145">contact</span><span class="sxs-lookup"><span data-stu-id="74dff-145">contact</span></span>](contact.md) | <span data-ttu-id="74dff-146">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="74dff-146">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="74dff-147">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="74dff-147">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="74dff-148">contact</span><span class="sxs-lookup"><span data-stu-id="74dff-148">contact</span></span>](contact.md) | <span data-ttu-id="74dff-149">新規または既存の連絡先に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="74dff-149">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="74dff-150">複数値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="74dff-150">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="74dff-151">contact</span><span class="sxs-lookup"><span data-stu-id="74dff-151">contact</span></span>](contact.md) | <span data-ttu-id="74dff-152">`$expand` を使用して、複数値の拡張プロパティを含む連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="74dff-152">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="74dff-153">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74dff-153">Properties</span></span>
| <span data-ttu-id="74dff-154">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74dff-154">Property</span></span>     | <span data-ttu-id="74dff-155">種類</span><span class="sxs-lookup"><span data-stu-id="74dff-155">Type</span></span>   |<span data-ttu-id="74dff-156">説明</span><span class="sxs-lookup"><span data-stu-id="74dff-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74dff-157">assistantName</span><span class="sxs-lookup"><span data-stu-id="74dff-157">assistantName</span></span>|<span data-ttu-id="74dff-158">String</span><span class="sxs-lookup"><span data-stu-id="74dff-158">String</span></span>|<span data-ttu-id="74dff-159">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="74dff-159">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="74dff-160">birthday</span><span class="sxs-lookup"><span data-stu-id="74dff-160">birthday</span></span>|<span data-ttu-id="74dff-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74dff-161">DateTimeOffset</span></span>|<span data-ttu-id="74dff-p103">連絡先の誕生日です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="74dff-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="74dff-165">businessAddress</span><span class="sxs-lookup"><span data-stu-id="74dff-165">businessAddress</span></span>|[<span data-ttu-id="74dff-166">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="74dff-166">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="74dff-167">連絡先の勤務先の住所。</span><span class="sxs-lookup"><span data-stu-id="74dff-167">The contact's business address.</span></span>|
|<span data-ttu-id="74dff-168">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="74dff-168">businessHomePage</span></span>|<span data-ttu-id="74dff-169">String</span><span class="sxs-lookup"><span data-stu-id="74dff-169">String</span></span>|<span data-ttu-id="74dff-170">連絡先の勤務先のホーム ページ。</span><span class="sxs-lookup"><span data-stu-id="74dff-170">The business home page of the contact.</span></span>|
|<span data-ttu-id="74dff-171">businessPhones</span><span class="sxs-lookup"><span data-stu-id="74dff-171">businessPhones</span></span>|<span data-ttu-id="74dff-172">String コレクション</span><span class="sxs-lookup"><span data-stu-id="74dff-172">String collection</span></span>|<span data-ttu-id="74dff-173">連絡先の勤務先の電話番号。</span><span class="sxs-lookup"><span data-stu-id="74dff-173">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="74dff-174">categories</span><span class="sxs-lookup"><span data-stu-id="74dff-174">categories</span></span>|<span data-ttu-id="74dff-175">String コレクション</span><span class="sxs-lookup"><span data-stu-id="74dff-175">String collection</span></span>|<span data-ttu-id="74dff-176">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="74dff-176">The categories associated with the contact.</span></span>|
|<span data-ttu-id="74dff-177">changeKey</span><span class="sxs-lookup"><span data-stu-id="74dff-177">changeKey</span></span>|<span data-ttu-id="74dff-178">String</span><span class="sxs-lookup"><span data-stu-id="74dff-178">String</span></span>|<span data-ttu-id="74dff-p104">連絡先のバージョンを識別します。連絡先を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="74dff-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="74dff-182">children</span><span class="sxs-lookup"><span data-stu-id="74dff-182">children</span></span>|<span data-ttu-id="74dff-183">String コレクション</span><span class="sxs-lookup"><span data-stu-id="74dff-183">String collection</span></span>|<span data-ttu-id="74dff-184">連絡先の子供の名前。</span><span class="sxs-lookup"><span data-stu-id="74dff-184">The names of the contact's children.</span></span>|
|<span data-ttu-id="74dff-185">companyName</span><span class="sxs-lookup"><span data-stu-id="74dff-185">companyName</span></span>|<span data-ttu-id="74dff-186">String</span><span class="sxs-lookup"><span data-stu-id="74dff-186">String</span></span>|<span data-ttu-id="74dff-187">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="74dff-187">The name of the contact's company.</span></span>|
|<span data-ttu-id="74dff-188">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74dff-188">createdDateTime</span></span>|<span data-ttu-id="74dff-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74dff-189">DateTimeOffset</span></span>|<span data-ttu-id="74dff-p105">連絡先が作成された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="74dff-p105">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="74dff-193">department</span><span class="sxs-lookup"><span data-stu-id="74dff-193">department</span></span>|<span data-ttu-id="74dff-194">String</span><span class="sxs-lookup"><span data-stu-id="74dff-194">String</span></span>|<span data-ttu-id="74dff-195">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="74dff-195">The contact's department.</span></span>|
|<span data-ttu-id="74dff-196">displayName</span><span class="sxs-lookup"><span data-stu-id="74dff-196">displayName</span></span>|<span data-ttu-id="74dff-197">String</span><span class="sxs-lookup"><span data-stu-id="74dff-197">String</span></span>|<span data-ttu-id="74dff-198">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="74dff-198">The contact's display name.</span></span> <span data-ttu-id="74dff-199">[作成](../api/user-post-contacts.md)または[更新](../api/contact-update.md)操作では、表示名を指定できます。</span><span class="sxs-lookup"><span data-stu-id="74dff-199">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="74dff-200">その他のプロパティを後で更新プログラムが原因で、自動的に生成された値を指定した表示名の値を上書きすることに注意します。</span><span class="sxs-lookup"><span data-stu-id="74dff-200">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="74dff-201">既存の値を保持するには、必ず、[更新](../api/contact-update.md)操作の表示名としてです。</span><span class="sxs-lookup"><span data-stu-id="74dff-201">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="74dff-202">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="74dff-202">emailAddresses</span></span>|<span data-ttu-id="74dff-203">[EmailAddress](emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="74dff-203">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="74dff-204">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="74dff-204">The contact's email addresses.</span></span>|
|<span data-ttu-id="74dff-205">fileAs</span><span class="sxs-lookup"><span data-stu-id="74dff-205">fileAs</span></span>|<span data-ttu-id="74dff-206">String</span><span class="sxs-lookup"><span data-stu-id="74dff-206">String</span></span>|<span data-ttu-id="74dff-207">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="74dff-207">The name the contact is filed under.</span></span>|
|<span data-ttu-id="74dff-208">generation</span><span class="sxs-lookup"><span data-stu-id="74dff-208">generation</span></span>|<span data-ttu-id="74dff-209">String</span><span class="sxs-lookup"><span data-stu-id="74dff-209">String</span></span>|<span data-ttu-id="74dff-210">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="74dff-210">The contact's generation.</span></span>|
|<span data-ttu-id="74dff-211">givenName</span><span class="sxs-lookup"><span data-stu-id="74dff-211">givenName</span></span>|<span data-ttu-id="74dff-212">String</span><span class="sxs-lookup"><span data-stu-id="74dff-212">String</span></span>|<span data-ttu-id="74dff-213">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="74dff-213">The contact's given name.</span></span>|
|<span data-ttu-id="74dff-214">homeAddress</span><span class="sxs-lookup"><span data-stu-id="74dff-214">homeAddress</span></span>|[<span data-ttu-id="74dff-215">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="74dff-215">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="74dff-216">連絡先の自宅住所。</span><span class="sxs-lookup"><span data-stu-id="74dff-216">The contact's home address.</span></span>|
|<span data-ttu-id="74dff-217">homePhones</span><span class="sxs-lookup"><span data-stu-id="74dff-217">homePhones</span></span>|<span data-ttu-id="74dff-218">String コレクション</span><span class="sxs-lookup"><span data-stu-id="74dff-218">String collection</span></span>|<span data-ttu-id="74dff-219">連絡先の自宅の電話番号。</span><span class="sxs-lookup"><span data-stu-id="74dff-219">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="74dff-220">id</span><span class="sxs-lookup"><span data-stu-id="74dff-220">id</span></span>|<span data-ttu-id="74dff-221">String</span><span class="sxs-lookup"><span data-stu-id="74dff-221">String</span></span>|<span data-ttu-id="74dff-p107">連絡先の一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="74dff-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="74dff-224">imAddresses</span><span class="sxs-lookup"><span data-stu-id="74dff-224">imAddresses</span></span>|<span data-ttu-id="74dff-225">String コレクション</span><span class="sxs-lookup"><span data-stu-id="74dff-225">String collection</span></span>|<span data-ttu-id="74dff-226">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="74dff-226">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="74dff-227">initials</span><span class="sxs-lookup"><span data-stu-id="74dff-227">initials</span></span>|<span data-ttu-id="74dff-228">String</span><span class="sxs-lookup"><span data-stu-id="74dff-228">String</span></span>|<span data-ttu-id="74dff-229">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="74dff-229">The contact's initials.</span></span>|
|<span data-ttu-id="74dff-230">jobTitle</span><span class="sxs-lookup"><span data-stu-id="74dff-230">jobTitle</span></span>|<span data-ttu-id="74dff-231">String</span><span class="sxs-lookup"><span data-stu-id="74dff-231">String</span></span>|<span data-ttu-id="74dff-232">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="74dff-232">The contact’s job title.</span></span>|
|<span data-ttu-id="74dff-233">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74dff-233">lastModifiedDateTime</span></span>|<span data-ttu-id="74dff-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74dff-234">DateTimeOffset</span></span>|<span data-ttu-id="74dff-p108">連絡先が変更された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="74dff-p108">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="74dff-238">manager</span><span class="sxs-lookup"><span data-stu-id="74dff-238">manager</span></span>|<span data-ttu-id="74dff-239">String</span><span class="sxs-lookup"><span data-stu-id="74dff-239">String</span></span>|<span data-ttu-id="74dff-240">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="74dff-240">The name of the contact's manager.</span></span>
|<span data-ttu-id="74dff-241">middleName</span><span class="sxs-lookup"><span data-stu-id="74dff-241">middleName</span></span>|<span data-ttu-id="74dff-242">String</span><span class="sxs-lookup"><span data-stu-id="74dff-242">String</span></span>|<span data-ttu-id="74dff-243">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="74dff-243">The contact's middle name.</span></span>|
|<span data-ttu-id="74dff-244">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="74dff-244">mobilePhone</span></span>|<span data-ttu-id="74dff-245">String</span><span class="sxs-lookup"><span data-stu-id="74dff-245">String</span></span>|<span data-ttu-id="74dff-246">連絡先の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="74dff-246">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="74dff-247">nickName</span><span class="sxs-lookup"><span data-stu-id="74dff-247">nickName</span></span>|<span data-ttu-id="74dff-248">String</span><span class="sxs-lookup"><span data-stu-id="74dff-248">String</span></span>|<span data-ttu-id="74dff-249">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="74dff-249">The contact's nickname.</span></span>|
|<span data-ttu-id="74dff-250">officeLocation</span><span class="sxs-lookup"><span data-stu-id="74dff-250">officeLocation</span></span>|<span data-ttu-id="74dff-251">String</span><span class="sxs-lookup"><span data-stu-id="74dff-251">String</span></span>|<span data-ttu-id="74dff-252">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="74dff-252">The location of the contact's office.</span></span>|
|<span data-ttu-id="74dff-253">otherAddress</span><span class="sxs-lookup"><span data-stu-id="74dff-253">otherAddress</span></span>|[<span data-ttu-id="74dff-254">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="74dff-254">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="74dff-255">連絡先の別の住所。</span><span class="sxs-lookup"><span data-stu-id="74dff-255">Other addresses for the contact.</span></span>|
|<span data-ttu-id="74dff-256">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="74dff-256">parentFolderId</span></span>|<span data-ttu-id="74dff-257">String</span><span class="sxs-lookup"><span data-stu-id="74dff-257">String</span></span>|<span data-ttu-id="74dff-258">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="74dff-258">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="74dff-259">personalNotes</span><span class="sxs-lookup"><span data-stu-id="74dff-259">personalNotes</span></span>|<span data-ttu-id="74dff-260">String</span><span class="sxs-lookup"><span data-stu-id="74dff-260">String</span></span>|<span data-ttu-id="74dff-261">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="74dff-261">The user's notes about the contact.</span></span>|
|<span data-ttu-id="74dff-262">profession</span><span class="sxs-lookup"><span data-stu-id="74dff-262">profession</span></span>|<span data-ttu-id="74dff-263">String</span><span class="sxs-lookup"><span data-stu-id="74dff-263">String</span></span>|<span data-ttu-id="74dff-264">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="74dff-264">The contact's profession.</span></span>|
|<span data-ttu-id="74dff-265">spouseName</span><span class="sxs-lookup"><span data-stu-id="74dff-265">spouseName</span></span>|<span data-ttu-id="74dff-266">String</span><span class="sxs-lookup"><span data-stu-id="74dff-266">String</span></span>|<span data-ttu-id="74dff-267">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="74dff-267">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="74dff-268">姓</span><span class="sxs-lookup"><span data-stu-id="74dff-268">surname</span></span>|<span data-ttu-id="74dff-269">String</span><span class="sxs-lookup"><span data-stu-id="74dff-269">String</span></span>|<span data-ttu-id="74dff-270">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="74dff-270">The contact's surname.</span></span>|
|<span data-ttu-id="74dff-271">タイトル</span><span class="sxs-lookup"><span data-stu-id="74dff-271">title</span></span>|<span data-ttu-id="74dff-272">String</span><span class="sxs-lookup"><span data-stu-id="74dff-272">String</span></span>|<span data-ttu-id="74dff-273">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="74dff-273">The contact's title.</span></span>|
|<span data-ttu-id="74dff-274">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="74dff-274">yomiCompanyName</span></span>|<span data-ttu-id="74dff-275">String</span><span class="sxs-lookup"><span data-stu-id="74dff-275">String</span></span>|<span data-ttu-id="74dff-276">連絡先の会社名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="74dff-276">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="74dff-277">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="74dff-277">yomiGivenName</span></span>|<span data-ttu-id="74dff-278">String</span><span class="sxs-lookup"><span data-stu-id="74dff-278">String</span></span>|<span data-ttu-id="74dff-279">連絡先の名 (ファースト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="74dff-279">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="74dff-280">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="74dff-280">yomiSurname</span></span>|<span data-ttu-id="74dff-281">String</span><span class="sxs-lookup"><span data-stu-id="74dff-281">String</span></span>|<span data-ttu-id="74dff-282">連絡先の姓 (ラスト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="74dff-282">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74dff-283">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="74dff-283">Relationships</span></span>
| <span data-ttu-id="74dff-284">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="74dff-284">Relationship</span></span> | <span data-ttu-id="74dff-285">型</span><span class="sxs-lookup"><span data-stu-id="74dff-285">Type</span></span>   |<span data-ttu-id="74dff-286">説明</span><span class="sxs-lookup"><span data-stu-id="74dff-286">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74dff-287">extensions</span><span class="sxs-lookup"><span data-stu-id="74dff-287">extensions</span></span>|<span data-ttu-id="74dff-288">[extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="74dff-288">[extension](extension.md) collection</span></span>|<span data-ttu-id="74dff-p109">連絡先に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="74dff-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="74dff-292">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="74dff-292">multiValueExtendedProperties</span></span>|<span data-ttu-id="74dff-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="74dff-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="74dff-p110">連絡先に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="74dff-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="74dff-297">photo</span><span class="sxs-lookup"><span data-stu-id="74dff-297">photo</span></span>|[<span data-ttu-id="74dff-298">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="74dff-298">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="74dff-p111">連絡先の写真 (オプション)。連絡先の写真を取得また設定することができます。</span><span class="sxs-lookup"><span data-stu-id="74dff-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="74dff-301">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="74dff-301">singleValueExtendedProperties</span></span>|<span data-ttu-id="74dff-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="74dff-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="74dff-p112">連絡先に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="74dff-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74dff-306">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74dff-306">JSON representation</span></span>

<span data-ttu-id="74dff-307">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="74dff-307">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact",
  "@odata.annotations": [
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a><span data-ttu-id="74dff-308">関連項目</span><span class="sxs-lookup"><span data-stu-id="74dff-308">See also</span></span>

- [<span data-ttu-id="74dff-309">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="74dff-309">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="74dff-310">フォルダー内のメッセージへの増分変更を取得する</span><span class="sxs-lookup"><span data-stu-id="74dff-310">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="74dff-311">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="74dff-311">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="74dff-312">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="74dff-312">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="74dff-313">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="74dff-313">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
