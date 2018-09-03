# <a name="contact-resource-type"></a><span data-ttu-id="b0b5f-101">contact リソース型</span><span class="sxs-lookup"><span data-stu-id="b0b5f-101">contact resource type</span></span>

<span data-ttu-id="b0b5f-p101">連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p101">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="b0b5f-104">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-104">This resource supports:</span></span>

- <span data-ttu-id="b0b5f-105">[拡張機能](../../../concepts/extensibility_overview.md)を使用して、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-105">Adding your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="b0b5f-106">[デルタ](../api/contact_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-106">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="b0b5f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0b5f-107">Methods</span></span>

| <span data-ttu-id="b0b5f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0b5f-108">Method</span></span>       | <span data-ttu-id="b0b5f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b0b5f-109">Return Type</span></span>  |<span data-ttu-id="b0b5f-110">説明</span><span class="sxs-lookup"><span data-stu-id="b0b5f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0b5f-111">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-111">Get contact</span></span>](../api/contact_get.md) | [<span data-ttu-id="b0b5f-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="b0b5f-112">contact</span></span>](contact.md) |<span data-ttu-id="b0b5f-113">連絡先オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-113">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="b0b5f-114">作成</span><span class="sxs-lookup"><span data-stu-id="b0b5f-114">Create</span></span>](../api/user_post_contacts.md) | [<span data-ttu-id="b0b5f-115">連絡先</span><span class="sxs-lookup"><span data-stu-id="b0b5f-115">contact</span></span>](contact.md) |<span data-ttu-id="b0b5f-116">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-116">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="b0b5f-117">更新する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-117">Update</span></span>](../api/contact_update.md) | [<span data-ttu-id="b0b5f-118">連絡先</span><span class="sxs-lookup"><span data-stu-id="b0b5f-118">contact</span></span>](contact.md) |<span data-ttu-id="b0b5f-119">連絡先オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-119">Update contact object.</span></span> |
|[<span data-ttu-id="b0b5f-120">削除</span><span class="sxs-lookup"><span data-stu-id="b0b5f-120">Delete</span></span>](../api/contact_delete.md) | <span data-ttu-id="b0b5f-121">なし</span><span class="sxs-lookup"><span data-stu-id="b0b5f-121">None</span></span> |<span data-ttu-id="b0b5f-122">連絡先オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-122">Delete contact object.</span></span> |
|[<span data-ttu-id="b0b5f-123">デルタ</span><span class="sxs-lookup"><span data-stu-id="b0b5f-123">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="b0b5f-124">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-124">[contact](contact.md) collection</span></span>| <span data-ttu-id="b0b5f-125">指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-125">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="b0b5f-126">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="b0b5f-126">**Open extensions**</span></span>| | |
|[<span data-ttu-id="b0b5f-127">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-127">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="b0b5f-128">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b0b5f-128">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="b0b5f-129">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-129">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="b0b5f-130">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-130">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="b0b5f-131">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-131">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="b0b5f-132">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-132">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="b0b5f-133">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="b0b5f-133">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="b0b5f-134">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-134">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="b0b5f-135">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-135">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="b0b5f-136">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="b0b5f-136">**Extended properties**</span></span>| | |
|[<span data-ttu-id="b0b5f-137">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-137">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="b0b5f-138">連絡先</span><span class="sxs-lookup"><span data-stu-id="b0b5f-138">contact</span></span>](contact.md)  |<span data-ttu-id="b0b5f-139">新規または既存の連絡先に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-139">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="b0b5f-140">単一値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-140">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="b0b5f-141">連絡先</span><span class="sxs-lookup"><span data-stu-id="b0b5f-141">contact</span></span>](contact.md) | <span data-ttu-id="b0b5f-142">または `$filter` を使用して、単一値の拡張プロパティを含む連絡先を取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="b0b5f-142">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b0b5f-143">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-143">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="b0b5f-144">連絡先</span><span class="sxs-lookup"><span data-stu-id="b0b5f-144">contact</span></span>](contact.md) | <span data-ttu-id="b0b5f-145">新規または既存の連絡先に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-145">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="b0b5f-146">複数値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-146">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="b0b5f-147">連絡先</span><span class="sxs-lookup"><span data-stu-id="b0b5f-147">contact</span></span>](contact.md) | <span data-ttu-id="b0b5f-148">を使用して、複数値の拡張プロパティを含む連絡先を取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="b0b5f-148">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0b5f-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0b5f-149">Properties</span></span>
| <span data-ttu-id="b0b5f-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0b5f-150">Property</span></span>     | <span data-ttu-id="b0b5f-151">タイプ</span><span class="sxs-lookup"><span data-stu-id="b0b5f-151">Type</span></span>   |<span data-ttu-id="b0b5f-152">説明</span><span class="sxs-lookup"><span data-stu-id="b0b5f-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0b5f-153">assistantName</span><span class="sxs-lookup"><span data-stu-id="b0b5f-153">assistantName</span></span>|<span data-ttu-id="b0b5f-154">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-154">String</span></span>|<span data-ttu-id="b0b5f-155">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-155">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="b0b5f-156">誕生日</span><span class="sxs-lookup"><span data-stu-id="b0b5f-156">birthday</span></span>|<span data-ttu-id="b0b5f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0b5f-157">DateTimeOffset</span></span>|<span data-ttu-id="b0b5f-p102">連絡先の誕生日です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p102">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b0b5f-161">businessAddress</span><span class="sxs-lookup"><span data-stu-id="b0b5f-161">businessAddress</span></span>|[<span data-ttu-id="b0b5f-162">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b0b5f-162">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="b0b5f-163">連絡先の勤務先の住所。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-163">The contact's business address.</span></span>|
|<span data-ttu-id="b0b5f-164">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="b0b5f-164">businessHomePage</span></span>|<span data-ttu-id="b0b5f-165">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-165">String</span></span>|<span data-ttu-id="b0b5f-166">連絡先の勤務先のホーム ページ。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-166">The business home page of the contact.</span></span>|
|<span data-ttu-id="b0b5f-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="b0b5f-167">businessPhones</span></span>|<span data-ttu-id="b0b5f-168">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-168">String collection</span></span>|<span data-ttu-id="b0b5f-169">連絡先の勤務先の電話番号。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-169">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="b0b5f-170">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="b0b5f-170">categories</span></span>|<span data-ttu-id="b0b5f-171">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-171">String collection</span></span>|<span data-ttu-id="b0b5f-172">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-172">The categories associated with the contact.</span></span>|
|<span data-ttu-id="b0b5f-173">changeKey</span><span class="sxs-lookup"><span data-stu-id="b0b5f-173">changeKey</span></span>|<span data-ttu-id="b0b5f-174">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-174">String</span></span>|<span data-ttu-id="b0b5f-p103">連絡先のバージョンを識別します。連絡先を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p103">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="b0b5f-178">子</span><span class="sxs-lookup"><span data-stu-id="b0b5f-178">children</span></span>|<span data-ttu-id="b0b5f-179">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-179">String collection</span></span>|<span data-ttu-id="b0b5f-180">連絡先の子供の名前。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-180">The names of the contact's children.</span></span>|
|<span data-ttu-id="b0b5f-181">companyName</span><span class="sxs-lookup"><span data-stu-id="b0b5f-181">companyName</span></span>|<span data-ttu-id="b0b5f-182">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-182">String</span></span>|<span data-ttu-id="b0b5f-183">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-183">The name of the contact's company.</span></span>|
|<span data-ttu-id="b0b5f-184">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0b5f-184">createdDateTime</span></span>|<span data-ttu-id="b0b5f-185">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0b5f-185">DateTimeOffset</span></span>|<span data-ttu-id="b0b5f-p104">連絡先が作成された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p104">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b0b5f-189">部署</span><span class="sxs-lookup"><span data-stu-id="b0b5f-189">department</span></span>|<span data-ttu-id="b0b5f-190">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-190">String</span></span>|<span data-ttu-id="b0b5f-191">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-191">The contact's department.</span></span>|
|<span data-ttu-id="b0b5f-192">displayName</span><span class="sxs-lookup"><span data-stu-id="b0b5f-192">displayName</span></span>|<span data-ttu-id="b0b5f-193">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-193">String</span></span>|<span data-ttu-id="b0b5f-194">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-194">The contact's display name.</span></span>|
|<span data-ttu-id="b0b5f-195">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="b0b5f-195">emailAddresses</span></span>|<span data-ttu-id="b0b5f-196">[EmailAddress](emailaddress.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-196">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="b0b5f-197">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-197">The contact's email addresses.</span></span>|
|<span data-ttu-id="b0b5f-198">フラグ</span><span class="sxs-lookup"><span data-stu-id="b0b5f-198">flag</span></span>|[<span data-ttu-id="b0b5f-199">FollowupFlag</span><span class="sxs-lookup"><span data-stu-id="b0b5f-199">FollowupFlag</span></span>](followupflag.md)|<span data-ttu-id="b0b5f-200">メッセージのステータス、開始日、期限、または完了日を示すフラグ値。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-200">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="b0b5f-201">fileAs</span><span class="sxs-lookup"><span data-stu-id="b0b5f-201">fileAs</span></span>|<span data-ttu-id="b0b5f-202">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-202">String</span></span>|<span data-ttu-id="b0b5f-203">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-203">The name the contact is filed under.</span></span>|
|<span data-ttu-id="b0b5f-204">生成</span><span class="sxs-lookup"><span data-stu-id="b0b5f-204">generation</span></span>|<span data-ttu-id="b0b5f-205">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-205">String</span></span>|<span data-ttu-id="b0b5f-206">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-206">The contact's generation.</span></span>|
|<span data-ttu-id="b0b5f-207">givenName</span><span class="sxs-lookup"><span data-stu-id="b0b5f-207">givenName</span></span>|<span data-ttu-id="b0b5f-208">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-208">String</span></span>|<span data-ttu-id="b0b5f-209">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-209">The contact's given name.</span></span>|
|<span data-ttu-id="b0b5f-210">homeAddress</span><span class="sxs-lookup"><span data-stu-id="b0b5f-210">homeAddress</span></span>|[<span data-ttu-id="b0b5f-211">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b0b5f-211">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="b0b5f-212">連絡先の自宅住所。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-212">The contact's home address.</span></span>|
|<span data-ttu-id="b0b5f-213">homePhones</span><span class="sxs-lookup"><span data-stu-id="b0b5f-213">homePhones</span></span>|<span data-ttu-id="b0b5f-214">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-214">String collection</span></span>|<span data-ttu-id="b0b5f-215">連絡先の自宅の電話番号。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-215">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="b0b5f-216">ID</span><span class="sxs-lookup"><span data-stu-id="b0b5f-216">id</span></span>|<span data-ttu-id="b0b5f-217">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-217">String</span></span>|<span data-ttu-id="b0b5f-p105">連絡先の一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p105">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="b0b5f-220">imAddresses</span><span class="sxs-lookup"><span data-stu-id="b0b5f-220">imAddresses</span></span>|<span data-ttu-id="b0b5f-221">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-221">String collection</span></span>|<span data-ttu-id="b0b5f-222">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-222">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="b0b5f-223">イニシャル</span><span class="sxs-lookup"><span data-stu-id="b0b5f-223">initials</span></span>|<span data-ttu-id="b0b5f-224">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-224">String</span></span>|<span data-ttu-id="b0b5f-225">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-225">The contact's initials.</span></span>|
|<span data-ttu-id="b0b5f-226">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b0b5f-226">jobTitle</span></span>|<span data-ttu-id="b0b5f-227">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-227">String</span></span>|<span data-ttu-id="b0b5f-228">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-228">The contact’s job title.</span></span>|
|<span data-ttu-id="b0b5f-229">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0b5f-229">lastModifiedDateTime</span></span>|<span data-ttu-id="b0b5f-230">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0b5f-230">DateTimeOffset</span></span>|<span data-ttu-id="b0b5f-p106">連絡先が変更された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p106">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b0b5f-234">マネージャー</span><span class="sxs-lookup"><span data-stu-id="b0b5f-234">manager</span></span>|<span data-ttu-id="b0b5f-235">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-235">String</span></span>|<span data-ttu-id="b0b5f-236">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-236">The name of the contact's manager.</span></span>
|<span data-ttu-id="b0b5f-237">middleName</span><span class="sxs-lookup"><span data-stu-id="b0b5f-237">middleName</span></span>|<span data-ttu-id="b0b5f-238">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-238">String</span></span>|<span data-ttu-id="b0b5f-239">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-239">The contact's middle name.</span></span>|
|<span data-ttu-id="b0b5f-240">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b0b5f-240">mobilePhone</span></span>|<span data-ttu-id="b0b5f-241">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-241">String</span></span>|<span data-ttu-id="b0b5f-242">連絡先の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-242">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="b0b5f-243">nickName</span><span class="sxs-lookup"><span data-stu-id="b0b5f-243">nickName</span></span>|<span data-ttu-id="b0b5f-244">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-244">String</span></span>|<span data-ttu-id="b0b5f-245">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-245">The contact's nickname.</span></span>|
|<span data-ttu-id="b0b5f-246">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b0b5f-246">officeLocation</span></span>|<span data-ttu-id="b0b5f-247">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-247">String</span></span>|<span data-ttu-id="b0b5f-248">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-248">The location of the contact's office.</span></span>|
|<span data-ttu-id="b0b5f-249">otherAddress</span><span class="sxs-lookup"><span data-stu-id="b0b5f-249">otherAddress</span></span>|[<span data-ttu-id="b0b5f-250">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b0b5f-250">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="b0b5f-251">連絡先の別の住所。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-251">Other addresses for the contact.</span></span>|
|<span data-ttu-id="b0b5f-252">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b0b5f-252">parentFolderId</span></span>|<span data-ttu-id="b0b5f-253">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-253">String</span></span>|<span data-ttu-id="b0b5f-254">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-254">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="b0b5f-255">personalNotes</span><span class="sxs-lookup"><span data-stu-id="b0b5f-255">personalNotes</span></span>|<span data-ttu-id="b0b5f-256">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-256">String</span></span>|<span data-ttu-id="b0b5f-257">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-257">The user's notes about the contact.</span></span>|
|<span data-ttu-id="b0b5f-258">職業</span><span class="sxs-lookup"><span data-stu-id="b0b5f-258">profession</span></span>|<span data-ttu-id="b0b5f-259">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-259">String</span></span>|<span data-ttu-id="b0b5f-260">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-260">The contact's profession.</span></span>|
|<span data-ttu-id="b0b5f-261">spouseName</span><span class="sxs-lookup"><span data-stu-id="b0b5f-261">spouseName</span></span>|<span data-ttu-id="b0b5f-262">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-262">String</span></span>|<span data-ttu-id="b0b5f-263">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-263">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="b0b5f-264">姓</span><span class="sxs-lookup"><span data-stu-id="b0b5f-264">surname</span></span>|<span data-ttu-id="b0b5f-265">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-265">String</span></span>|<span data-ttu-id="b0b5f-266">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-266">The contact's surname.</span></span>|
|<span data-ttu-id="b0b5f-267">タイトル</span><span class="sxs-lookup"><span data-stu-id="b0b5f-267">title</span></span>|<span data-ttu-id="b0b5f-268">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-268">String</span></span>|<span data-ttu-id="b0b5f-269">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-269">The contact's title.</span></span>|
|<span data-ttu-id="b0b5f-270">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="b0b5f-270">yomiCompanyName</span></span>|<span data-ttu-id="b0b5f-271">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-271">String</span></span>|<span data-ttu-id="b0b5f-272">連絡先の会社名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-272">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="b0b5f-273">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="b0b5f-273">yomiGivenName</span></span>|<span data-ttu-id="b0b5f-274">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-274">String</span></span>|<span data-ttu-id="b0b5f-275">連絡先の名 (ファースト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-275">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="b0b5f-276">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="b0b5f-276">yomiSurname</span></span>|<span data-ttu-id="b0b5f-277">文字列</span><span class="sxs-lookup"><span data-stu-id="b0b5f-277">String</span></span>|<span data-ttu-id="b0b5f-278">連絡先の姓 (ラスト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-278">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0b5f-279">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b0b5f-279">Relationships</span></span>
| <span data-ttu-id="b0b5f-280">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b0b5f-280">Relationship</span></span> | <span data-ttu-id="b0b5f-281">型</span><span class="sxs-lookup"><span data-stu-id="b0b5f-281">Type</span></span>   |<span data-ttu-id="b0b5f-282">説明</span><span class="sxs-lookup"><span data-stu-id="b0b5f-282">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0b5f-283">拡張機能</span><span class="sxs-lookup"><span data-stu-id="b0b5f-283">extensions</span></span>|<span data-ttu-id="b0b5f-284">[extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-284">[extension](extension.md) collection</span></span>|<span data-ttu-id="b0b5f-p107">連絡先に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p107">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b0b5f-288">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b0b5f-288">multiValueExtendedProperties</span></span>|<span data-ttu-id="b0b5f-289">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-289">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b0b5f-p108">連絡先に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p108">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b0b5f-293">写真</span><span class="sxs-lookup"><span data-stu-id="b0b5f-293">photo</span></span>|[<span data-ttu-id="b0b5f-294">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="b0b5f-294">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="b0b5f-p109">連絡先の写真 (オプション)。連絡先の写真を取得また設定することができます。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p109">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="b0b5f-297">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b0b5f-297">singleValueExtendedProperties</span></span>|<span data-ttu-id="b0b5f-298">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b5f-298">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b0b5f-p110">連絡先に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b0b5f-p110">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0b5f-302">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0b5f-302">JSON representation</span></span>

<span data-ttu-id="b0b5f-303">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b0b5f-303">Here is a JSON representation of the resource</span></span>

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
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
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

## <a name="see-also"></a><span data-ttu-id="b0b5f-304">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0b5f-304">See also</span></span>

- [<span data-ttu-id="b0b5f-305">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-305">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="b0b5f-306">フォルダー内のメッセージへの増分変更を取得する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-306">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="b0b5f-307">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-307">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="b0b5f-308">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="b0b5f-308">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="b0b5f-309">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="b0b5f-309">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
