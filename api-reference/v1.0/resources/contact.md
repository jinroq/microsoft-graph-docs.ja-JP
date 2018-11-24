# <a name="contact-resource-type"></a><span data-ttu-id="9b6d6-101">contact リソース型</span><span class="sxs-lookup"><span data-stu-id="9b6d6-101">contact resource type</span></span>

<span data-ttu-id="9b6d6-p101">連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p101">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="9b6d6-104">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-104">This resource supports:</span></span>

- <span data-ttu-id="9b6d6-105">[拡張機能](../../../concepts/extensibility_overview.md)として、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-105">Adding your own data to custom properties as [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="9b6d6-106">[変更通知](../../../concepts/webhooks.md)にサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-106">Subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>
- <span data-ttu-id="9b6d6-107">[デルタ](../api/contact_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-107">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="9b6d6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b6d6-108">Methods</span></span>

| <span data-ttu-id="9b6d6-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b6d6-109">Method</span></span>       | <span data-ttu-id="9b6d6-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9b6d6-110">Return Type</span></span>  |<span data-ttu-id="9b6d6-111">説明</span><span class="sxs-lookup"><span data-stu-id="9b6d6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b6d6-112">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-112">Get contact</span></span>](../api/contact_get.md) | [<span data-ttu-id="9b6d6-113">contact</span><span class="sxs-lookup"><span data-stu-id="9b6d6-113">contact</span></span>](contact.md) |<span data-ttu-id="9b6d6-114">連絡先オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-114">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="9b6d6-115">作成</span><span class="sxs-lookup"><span data-stu-id="9b6d6-115">Create</span></span>](../api/user_post_contacts.md) | [<span data-ttu-id="9b6d6-116">contact</span><span class="sxs-lookup"><span data-stu-id="9b6d6-116">contact</span></span>](contact.md) |<span data-ttu-id="9b6d6-117">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-117">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="9b6d6-118">更新する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-118">Update</span></span>](../api/contact_update.md) | [<span data-ttu-id="9b6d6-119">contact</span><span class="sxs-lookup"><span data-stu-id="9b6d6-119">contact</span></span>](contact.md) |<span data-ttu-id="9b6d6-120">連絡先オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-120">Update contact object.</span></span> |
|[<span data-ttu-id="9b6d6-121">削除</span><span class="sxs-lookup"><span data-stu-id="9b6d6-121">Delete</span></span>](../api/contact_delete.md) | <span data-ttu-id="9b6d6-122">なし</span><span class="sxs-lookup"><span data-stu-id="9b6d6-122">None</span></span> |<span data-ttu-id="9b6d6-123">連絡先オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-123">Delete contact object.</span></span> |
|[<span data-ttu-id="9b6d6-124">delta</span><span class="sxs-lookup"><span data-stu-id="9b6d6-124">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="9b6d6-125">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9b6d6-125">[contact](contact.md) collection</span></span>| <span data-ttu-id="9b6d6-126">指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-126">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="9b6d6-127">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="9b6d6-127">**Open extensions**</span></span>| | |
|[<span data-ttu-id="9b6d6-128">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-128">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="9b6d6-129">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="9b6d6-129">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="9b6d6-130">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-130">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="9b6d6-131">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-131">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="9b6d6-132">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9b6d6-132">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="9b6d6-133">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-133">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="9b6d6-134">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="9b6d6-134">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="9b6d6-135">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-135">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="9b6d6-136">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-136">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="9b6d6-137">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="9b6d6-137">**Extended properties**</span></span>| | |
|[<span data-ttu-id="9b6d6-138">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-138">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="9b6d6-139">contact</span><span class="sxs-lookup"><span data-stu-id="9b6d6-139">contact</span></span>](contact.md)  |<span data-ttu-id="9b6d6-140">新規または既存の連絡先に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-140">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="9b6d6-141">単一値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-141">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="9b6d6-142">contact</span><span class="sxs-lookup"><span data-stu-id="9b6d6-142">contact</span></span>](contact.md) | <span data-ttu-id="9b6d6-143">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-143">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="9b6d6-144">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-144">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="9b6d6-145">contact</span><span class="sxs-lookup"><span data-stu-id="9b6d6-145">contact</span></span>](contact.md) | <span data-ttu-id="9b6d6-146">新規または既存の連絡先に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-146">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="9b6d6-147">複数値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-147">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="9b6d6-148">contact</span><span class="sxs-lookup"><span data-stu-id="9b6d6-148">contact</span></span>](contact.md) | <span data-ttu-id="9b6d6-149">`$expand` を使用して、複数値の拡張プロパティを含む連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-149">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="9b6d6-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b6d6-150">Properties</span></span>
| <span data-ttu-id="9b6d6-151">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b6d6-151">Property</span></span>     | <span data-ttu-id="9b6d6-152">型</span><span class="sxs-lookup"><span data-stu-id="9b6d6-152">Type</span></span>   |<span data-ttu-id="9b6d6-153">説明</span><span class="sxs-lookup"><span data-stu-id="9b6d6-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b6d6-154">assistantName</span><span class="sxs-lookup"><span data-stu-id="9b6d6-154">assistantName</span></span>|<span data-ttu-id="9b6d6-155">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-155">String</span></span>|<span data-ttu-id="9b6d6-156">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-156">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="9b6d6-157">birthday</span><span class="sxs-lookup"><span data-stu-id="9b6d6-157">birthday</span></span>|<span data-ttu-id="9b6d6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b6d6-158">DateTimeOffset</span></span>|<span data-ttu-id="9b6d6-p102">連絡先の誕生日です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p102">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9b6d6-162">businessAddress</span><span class="sxs-lookup"><span data-stu-id="9b6d6-162">businessAddress</span></span>|[<span data-ttu-id="9b6d6-163">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="9b6d6-163">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="9b6d6-164">連絡先の勤務先の住所。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-164">The contact's business address.</span></span>|
|<span data-ttu-id="9b6d6-165">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="9b6d6-165">businessHomePage</span></span>|<span data-ttu-id="9b6d6-166">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-166">String</span></span>|<span data-ttu-id="9b6d6-167">連絡先の勤務先のホーム ページ。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-167">The business home page of the contact.</span></span>|
|<span data-ttu-id="9b6d6-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="9b6d6-168">businessPhones</span></span>|<span data-ttu-id="9b6d6-169">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9b6d6-169">String collection</span></span>|<span data-ttu-id="9b6d6-170">連絡先の勤務先の電話番号。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-170">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="9b6d6-171">categories</span><span class="sxs-lookup"><span data-stu-id="9b6d6-171">categories</span></span>|<span data-ttu-id="9b6d6-172">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9b6d6-172">String collection</span></span>|<span data-ttu-id="9b6d6-173">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-173">The categories associated with the contact.</span></span>|
|<span data-ttu-id="9b6d6-174">changeKey</span><span class="sxs-lookup"><span data-stu-id="9b6d6-174">changeKey</span></span>|<span data-ttu-id="9b6d6-175">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-175">String</span></span>|<span data-ttu-id="9b6d6-p103">連絡先のバージョンを識別します。連絡先を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p103">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="9b6d6-179">children</span><span class="sxs-lookup"><span data-stu-id="9b6d6-179">children</span></span>|<span data-ttu-id="9b6d6-180">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9b6d6-180">String collection</span></span>|<span data-ttu-id="9b6d6-181">連絡先の子供の名前。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-181">The names of the contact's children.</span></span>|
|<span data-ttu-id="9b6d6-182">companyName</span><span class="sxs-lookup"><span data-stu-id="9b6d6-182">companyName</span></span>|<span data-ttu-id="9b6d6-183">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-183">String</span></span>|<span data-ttu-id="9b6d6-184">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-184">The name of the contact's company.</span></span>|
|<span data-ttu-id="9b6d6-185">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b6d6-185">createdDateTime</span></span>|<span data-ttu-id="9b6d6-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b6d6-186">DateTimeOffset</span></span>|<span data-ttu-id="9b6d6-p104">連絡先が作成された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p104">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9b6d6-190">department</span><span class="sxs-lookup"><span data-stu-id="9b6d6-190">department</span></span>|<span data-ttu-id="9b6d6-191">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-191">String</span></span>|<span data-ttu-id="9b6d6-192">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-192">The contact's department.</span></span>|
|<span data-ttu-id="9b6d6-193">displayName</span><span class="sxs-lookup"><span data-stu-id="9b6d6-193">displayName</span></span>|<span data-ttu-id="9b6d6-194">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-194">String</span></span>|<span data-ttu-id="9b6d6-195">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-195">The contact's display name.</span></span> <span data-ttu-id="9b6d6-196">[作成](../api/user_post_contacts.md)または[更新](../api/contact_update.md)操作では、表示名を指定できます。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-196">You can specify the display name in a [create](../api/user_post_contacts.md) or [update](../api/contact_update.md) operation.</span></span> <span data-ttu-id="9b6d6-197">その他のプロパティを後で更新プログラムが原因で、自動的に生成された値を指定した表示名の値を上書きすることに注意します。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-197">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="9b6d6-198">既存の値を保持するには、必ず、[更新](../api/contact_update.md)操作の表示名としてです。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-198">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact_update.md) operation.</span></span>|
|<span data-ttu-id="9b6d6-199">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="9b6d6-199">emailAddresses</span></span>|<span data-ttu-id="9b6d6-200">[EmailAddress](emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="9b6d6-200">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="9b6d6-201">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-201">The contact's email addresses.</span></span>|
|<span data-ttu-id="9b6d6-202">fileAs</span><span class="sxs-lookup"><span data-stu-id="9b6d6-202">fileAs</span></span>|<span data-ttu-id="9b6d6-203">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-203">String</span></span>|<span data-ttu-id="9b6d6-204">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-204">The name the contact is filed under.</span></span>|
|<span data-ttu-id="9b6d6-205">generation</span><span class="sxs-lookup"><span data-stu-id="9b6d6-205">generation</span></span>|<span data-ttu-id="9b6d6-206">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-206">String</span></span>|<span data-ttu-id="9b6d6-207">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-207">The contact's generation.</span></span>|
|<span data-ttu-id="9b6d6-208">givenName</span><span class="sxs-lookup"><span data-stu-id="9b6d6-208">givenName</span></span>|<span data-ttu-id="9b6d6-209">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-209">String</span></span>|<span data-ttu-id="9b6d6-210">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-210">The contact's given name.</span></span>|
|<span data-ttu-id="9b6d6-211">homeAddress</span><span class="sxs-lookup"><span data-stu-id="9b6d6-211">homeAddress</span></span>|[<span data-ttu-id="9b6d6-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="9b6d6-212">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="9b6d6-213">連絡先の自宅住所。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-213">The contact's home address.</span></span>|
|<span data-ttu-id="9b6d6-214">homePhones</span><span class="sxs-lookup"><span data-stu-id="9b6d6-214">homePhones</span></span>|<span data-ttu-id="9b6d6-215">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9b6d6-215">String collection</span></span>|<span data-ttu-id="9b6d6-216">連絡先の自宅の電話番号。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-216">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="9b6d6-217">id</span><span class="sxs-lookup"><span data-stu-id="9b6d6-217">id</span></span>|<span data-ttu-id="9b6d6-218">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-218">String</span></span>|<span data-ttu-id="9b6d6-p106">連絡先の一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p106">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="9b6d6-221">imAddresses</span><span class="sxs-lookup"><span data-stu-id="9b6d6-221">imAddresses</span></span>|<span data-ttu-id="9b6d6-222">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9b6d6-222">String collection</span></span>|<span data-ttu-id="9b6d6-223">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-223">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="9b6d6-224">initials</span><span class="sxs-lookup"><span data-stu-id="9b6d6-224">initials</span></span>|<span data-ttu-id="9b6d6-225">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-225">String</span></span>|<span data-ttu-id="9b6d6-226">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-226">The contact's initials.</span></span>|
|<span data-ttu-id="9b6d6-227">jobTitle</span><span class="sxs-lookup"><span data-stu-id="9b6d6-227">jobTitle</span></span>|<span data-ttu-id="9b6d6-228">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-228">String</span></span>|<span data-ttu-id="9b6d6-229">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-229">The contact’s job title.</span></span>|
|<span data-ttu-id="9b6d6-230">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b6d6-230">lastModifiedDateTime</span></span>|<span data-ttu-id="9b6d6-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b6d6-231">DateTimeOffset</span></span>|<span data-ttu-id="9b6d6-p107">連絡先が変更された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p107">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9b6d6-235">manager</span><span class="sxs-lookup"><span data-stu-id="9b6d6-235">manager</span></span>|<span data-ttu-id="9b6d6-236">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-236">String</span></span>|<span data-ttu-id="9b6d6-237">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-237">The name of the contact's manager.</span></span>
|<span data-ttu-id="9b6d6-238">middleName</span><span class="sxs-lookup"><span data-stu-id="9b6d6-238">middleName</span></span>|<span data-ttu-id="9b6d6-239">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-239">String</span></span>|<span data-ttu-id="9b6d6-240">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-240">The contact's middle name.</span></span>|
|<span data-ttu-id="9b6d6-241">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="9b6d6-241">mobilePhone</span></span>|<span data-ttu-id="9b6d6-242">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-242">String</span></span>|<span data-ttu-id="9b6d6-243">連絡先の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-243">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="9b6d6-244">nickName</span><span class="sxs-lookup"><span data-stu-id="9b6d6-244">nickName</span></span>|<span data-ttu-id="9b6d6-245">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-245">String</span></span>|<span data-ttu-id="9b6d6-246">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-246">The contact's nickname.</span></span>|
|<span data-ttu-id="9b6d6-247">officeLocation</span><span class="sxs-lookup"><span data-stu-id="9b6d6-247">officeLocation</span></span>|<span data-ttu-id="9b6d6-248">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-248">String</span></span>|<span data-ttu-id="9b6d6-249">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-249">The location of the contact's office.</span></span>|
|<span data-ttu-id="9b6d6-250">otherAddress</span><span class="sxs-lookup"><span data-stu-id="9b6d6-250">otherAddress</span></span>|[<span data-ttu-id="9b6d6-251">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="9b6d6-251">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="9b6d6-252">連絡先の別の住所。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-252">Other addresses for the contact.</span></span>|
|<span data-ttu-id="9b6d6-253">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="9b6d6-253">parentFolderId</span></span>|<span data-ttu-id="9b6d6-254">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-254">String</span></span>|<span data-ttu-id="9b6d6-255">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-255">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="9b6d6-256">personalNotes</span><span class="sxs-lookup"><span data-stu-id="9b6d6-256">personalNotes</span></span>|<span data-ttu-id="9b6d6-257">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-257">String</span></span>|<span data-ttu-id="9b6d6-258">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-258">The user's notes about the contact.</span></span>|
|<span data-ttu-id="9b6d6-259">profession</span><span class="sxs-lookup"><span data-stu-id="9b6d6-259">profession</span></span>|<span data-ttu-id="9b6d6-260">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-260">String</span></span>|<span data-ttu-id="9b6d6-261">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-261">The contact's profession.</span></span>|
|<span data-ttu-id="9b6d6-262">spouseName</span><span class="sxs-lookup"><span data-stu-id="9b6d6-262">spouseName</span></span>|<span data-ttu-id="9b6d6-263">String</span><span class="sxs-lookup"><span data-stu-id="9b6d6-263">String</span></span>|<span data-ttu-id="9b6d6-264">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-264">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="9b6d6-265">姓</span><span class="sxs-lookup"><span data-stu-id="9b6d6-265">surname</span></span>|<span data-ttu-id="9b6d6-266">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-266">String</span></span>|<span data-ttu-id="9b6d6-267">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-267">The contact's surname.</span></span>|
|<span data-ttu-id="9b6d6-268">タイトル</span><span class="sxs-lookup"><span data-stu-id="9b6d6-268">title</span></span>|<span data-ttu-id="9b6d6-269">String</span><span class="sxs-lookup"><span data-stu-id="9b6d6-269">String</span></span>|<span data-ttu-id="9b6d6-270">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-270">The contact's title.</span></span>|
|<span data-ttu-id="9b6d6-271">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="9b6d6-271">yomiCompanyName</span></span>|<span data-ttu-id="9b6d6-272">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-272">String</span></span>|<span data-ttu-id="9b6d6-273">連絡先の会社名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-273">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="9b6d6-274">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="9b6d6-274">yomiGivenName</span></span>|<span data-ttu-id="9b6d6-275">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-275">String</span></span>|<span data-ttu-id="9b6d6-276">連絡先の名 (ファースト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-276">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="9b6d6-277">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="9b6d6-277">yomiSurname</span></span>|<span data-ttu-id="9b6d6-278">文字列</span><span class="sxs-lookup"><span data-stu-id="9b6d6-278">String</span></span>|<span data-ttu-id="9b6d6-279">連絡先の姓 (ラスト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-279">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b6d6-280">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b6d6-280">Relationships</span></span>
| <span data-ttu-id="9b6d6-281">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b6d6-281">Relationship</span></span> | <span data-ttu-id="9b6d6-282">型</span><span class="sxs-lookup"><span data-stu-id="9b6d6-282">Type</span></span>   |<span data-ttu-id="9b6d6-283">説明</span><span class="sxs-lookup"><span data-stu-id="9b6d6-283">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b6d6-284">extensions</span><span class="sxs-lookup"><span data-stu-id="9b6d6-284">extensions</span></span>|<span data-ttu-id="9b6d6-285">[extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9b6d6-285">[extension](extension.md) collection</span></span>|<span data-ttu-id="9b6d6-p108">連絡先に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p108">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9b6d6-289">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9b6d6-289">multiValueExtendedProperties</span></span>|<span data-ttu-id="9b6d6-290">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="9b6d6-290">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="9b6d6-p109">連絡先に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p109">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9b6d6-294">photo</span><span class="sxs-lookup"><span data-stu-id="9b6d6-294">photo</span></span>|[<span data-ttu-id="9b6d6-295">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9b6d6-295">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="9b6d6-p110">連絡先の写真 (オプション)。連絡先の写真を取得また設定することができます。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p110">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="9b6d6-298">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9b6d6-298">singleValueExtendedProperties</span></span>|<span data-ttu-id="9b6d6-299">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="9b6d6-299">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="9b6d6-p111">連絡先に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9b6d6-p111">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b6d6-303">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b6d6-303">JSON representation</span></span>

<span data-ttu-id="9b6d6-304">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9b6d6-304">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="9b6d6-305">関連項目</span><span class="sxs-lookup"><span data-stu-id="9b6d6-305">See also</span></span>

- [<span data-ttu-id="9b6d6-306">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-306">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="9b6d6-307">フォルダー内のメッセージへの増分変更を取得する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-307">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="9b6d6-308">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-308">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="9b6d6-309">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="9b6d6-309">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="9b6d6-310">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="9b6d6-310">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
