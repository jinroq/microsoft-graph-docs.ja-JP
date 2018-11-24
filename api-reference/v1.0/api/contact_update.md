# <a name="update-contact"></a><span data-ttu-id="94db5-101">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="94db5-101">Update contact</span></span>

<span data-ttu-id="94db5-102">連絡先オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="94db5-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94db5-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94db5-103">Permissions</span></span>
<span data-ttu-id="94db5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94db5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="94db5-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94db5-106">Permission type</span></span>      | <span data-ttu-id="94db5-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94db5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94db5-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94db5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="94db5-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94db5-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="94db5-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94db5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94db5-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94db5-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="94db5-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94db5-112">Application</span></span> | <span data-ttu-id="94db5-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94db5-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94db5-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94db5-114">HTTP request</span></span>
<span data-ttu-id="94db5-115"><!-- { "blockType": "ignored" } -->[連絡先](../resources/contact.md)ユーザーの既定の[contactFolder](../resources/contactfolder.md)からです。</span><span class="sxs-lookup"><span data-stu-id="94db5-115"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="94db5-116">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="94db5-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="94db5-p102">[contactFolder](../resources/mailfolder.md) の子フォルダー内に含まれる [連絡先](../resources/contact.md)。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="94db5-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="94db5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94db5-119">Request headers</span></span>
| <span data-ttu-id="94db5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94db5-120">Header</span></span>       | <span data-ttu-id="94db5-121">値</span><span class="sxs-lookup"><span data-stu-id="94db5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94db5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94db5-122">Authorization</span></span>  | <span data-ttu-id="94db5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94db5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94db5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94db5-125">Content-Type</span></span>  | <span data-ttu-id="94db5-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="94db5-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94db5-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="94db5-128">Request body</span></span>
<span data-ttu-id="94db5-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="94db5-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94db5-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94db5-132">Property</span></span>     | <span data-ttu-id="94db5-133">型</span><span class="sxs-lookup"><span data-stu-id="94db5-133">Type</span></span>   |<span data-ttu-id="94db5-134">説明</span><span class="sxs-lookup"><span data-stu-id="94db5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94db5-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="94db5-135">assistantName</span></span>|<span data-ttu-id="94db5-136">String</span><span class="sxs-lookup"><span data-stu-id="94db5-136">String</span></span>|<span data-ttu-id="94db5-137">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="94db5-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="94db5-138">birthday</span><span class="sxs-lookup"><span data-stu-id="94db5-138">birthday</span></span>|<span data-ttu-id="94db5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94db5-139">DateTimeOffset</span></span>|<span data-ttu-id="94db5-140">連絡先の誕生日です。</span><span class="sxs-lookup"><span data-stu-id="94db5-140">The contact's birthday.</span></span>|
|<span data-ttu-id="94db5-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="94db5-141">businessAddress</span></span>|[<span data-ttu-id="94db5-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="94db5-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="94db5-143">連絡先の勤務先の住所。</span><span class="sxs-lookup"><span data-stu-id="94db5-143">The contact's business address.</span></span>|
|<span data-ttu-id="94db5-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="94db5-144">businessHomePage</span></span>|<span data-ttu-id="94db5-145">String</span><span class="sxs-lookup"><span data-stu-id="94db5-145">String</span></span>|<span data-ttu-id="94db5-146">連絡先の勤務先のホーム ページ。</span><span class="sxs-lookup"><span data-stu-id="94db5-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="94db5-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="94db5-147">businessPhones</span></span>|<span data-ttu-id="94db5-148">String</span><span class="sxs-lookup"><span data-stu-id="94db5-148">String</span></span>|<span data-ttu-id="94db5-149">連絡先の勤務先の電話番号。</span><span class="sxs-lookup"><span data-stu-id="94db5-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="94db5-150">categories</span><span class="sxs-lookup"><span data-stu-id="94db5-150">categories</span></span>|<span data-ttu-id="94db5-151">String</span><span class="sxs-lookup"><span data-stu-id="94db5-151">String</span></span>|<span data-ttu-id="94db5-152">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="94db5-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="94db5-153">children</span><span class="sxs-lookup"><span data-stu-id="94db5-153">children</span></span>|<span data-ttu-id="94db5-154">String</span><span class="sxs-lookup"><span data-stu-id="94db5-154">String</span></span>|<span data-ttu-id="94db5-155">連絡先の子供の名前。</span><span class="sxs-lookup"><span data-stu-id="94db5-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="94db5-156">companyName</span><span class="sxs-lookup"><span data-stu-id="94db5-156">companyName</span></span>|<span data-ttu-id="94db5-157">String</span><span class="sxs-lookup"><span data-stu-id="94db5-157">String</span></span>|<span data-ttu-id="94db5-158">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="94db5-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="94db5-159">department</span><span class="sxs-lookup"><span data-stu-id="94db5-159">department</span></span>|<span data-ttu-id="94db5-160">String</span><span class="sxs-lookup"><span data-stu-id="94db5-160">String</span></span>|<span data-ttu-id="94db5-161">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="94db5-161">The contact's department.</span></span>|
|<span data-ttu-id="94db5-162">displayName</span><span class="sxs-lookup"><span data-stu-id="94db5-162">displayName</span></span>|<span data-ttu-id="94db5-163">String</span><span class="sxs-lookup"><span data-stu-id="94db5-163">String</span></span>|<span data-ttu-id="94db5-164">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="94db5-164">The contact's display name.</span></span> <span data-ttu-id="94db5-165">その他のプロパティを後で更新プログラムが原因で、自動的に生成された値を指定した表示名の値を上書きすることに注意します。</span><span class="sxs-lookup"><span data-stu-id="94db5-165">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="94db5-166">既存の値を保持するには、必ず、更新操作の表示名としてです。</span><span class="sxs-lookup"><span data-stu-id="94db5-166">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="94db5-167">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="94db5-167">emailAddresses</span></span>|<span data-ttu-id="94db5-168">[EmailAddress](../resources/emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="94db5-168">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="94db5-169">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="94db5-169">The contact's email addresses.</span></span>|
|<span data-ttu-id="94db5-170">fileAs</span><span class="sxs-lookup"><span data-stu-id="94db5-170">fileAs</span></span>|<span data-ttu-id="94db5-171">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-171">String</span></span>|<span data-ttu-id="94db5-172">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="94db5-172">The name the contact is filed under.</span></span>|
|<span data-ttu-id="94db5-173">generation</span><span class="sxs-lookup"><span data-stu-id="94db5-173">generation</span></span>|<span data-ttu-id="94db5-174">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-174">String</span></span>|<span data-ttu-id="94db5-175">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="94db5-175">The contact's generation.</span></span>|
|<span data-ttu-id="94db5-176">givenName</span><span class="sxs-lookup"><span data-stu-id="94db5-176">givenName</span></span>|<span data-ttu-id="94db5-177">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-177">String</span></span>|<span data-ttu-id="94db5-178">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="94db5-178">The contact's given name.</span></span>|
|<span data-ttu-id="94db5-179">homeAddress</span><span class="sxs-lookup"><span data-stu-id="94db5-179">homeAddress</span></span>|[<span data-ttu-id="94db5-180">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="94db5-180">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="94db5-181">連絡先の自宅住所。</span><span class="sxs-lookup"><span data-stu-id="94db5-181">The contact's home address.</span></span>|
|<span data-ttu-id="94db5-182">homePhones</span><span class="sxs-lookup"><span data-stu-id="94db5-182">homePhones</span></span>|<span data-ttu-id="94db5-183">String コレクション</span><span class="sxs-lookup"><span data-stu-id="94db5-183">String collection</span></span>|<span data-ttu-id="94db5-184">連絡先の自宅の電話番号。</span><span class="sxs-lookup"><span data-stu-id="94db5-184">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="94db5-185">imAddresses</span><span class="sxs-lookup"><span data-stu-id="94db5-185">imAddresses</span></span>|<span data-ttu-id="94db5-186">String</span><span class="sxs-lookup"><span data-stu-id="94db5-186">String</span></span>|<span data-ttu-id="94db5-187">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="94db5-187">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="94db5-188">initials</span><span class="sxs-lookup"><span data-stu-id="94db5-188">initials</span></span>|<span data-ttu-id="94db5-189">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-189">String</span></span>|<span data-ttu-id="94db5-190">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="94db5-190">The contact's initials.</span></span>|
|<span data-ttu-id="94db5-191">jobTitle</span><span class="sxs-lookup"><span data-stu-id="94db5-191">jobTitle</span></span>|<span data-ttu-id="94db5-192">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-192">String</span></span>|<span data-ttu-id="94db5-193">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="94db5-193">The contact’s job title.</span></span>|
|<span data-ttu-id="94db5-194">manager</span><span class="sxs-lookup"><span data-stu-id="94db5-194">manager</span></span>|<span data-ttu-id="94db5-195">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-195">String</span></span>|<span data-ttu-id="94db5-196">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="94db5-196">The name of the contact's manager.</span></span>
|<span data-ttu-id="94db5-197">middleName</span><span class="sxs-lookup"><span data-stu-id="94db5-197">middleName</span></span>|<span data-ttu-id="94db5-198">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-198">String</span></span>|<span data-ttu-id="94db5-199">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="94db5-199">The contact's middle name.</span></span>|
|<span data-ttu-id="94db5-200">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="94db5-200">mobilePhone</span></span>|<span data-ttu-id="94db5-201">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-201">String</span></span>|<span data-ttu-id="94db5-202">連絡先の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="94db5-202">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="94db5-203">nickName</span><span class="sxs-lookup"><span data-stu-id="94db5-203">nickName</span></span>|<span data-ttu-id="94db5-204">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-204">String</span></span>|<span data-ttu-id="94db5-205">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="94db5-205">The contact's nickname.</span></span>|
|<span data-ttu-id="94db5-206">officeLocation</span><span class="sxs-lookup"><span data-stu-id="94db5-206">officeLocation</span></span>|<span data-ttu-id="94db5-207">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-207">String</span></span>|<span data-ttu-id="94db5-208">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="94db5-208">The location of the contact's office.</span></span>|
|<span data-ttu-id="94db5-209">otherAddress</span><span class="sxs-lookup"><span data-stu-id="94db5-209">otherAddress</span></span>|[<span data-ttu-id="94db5-210">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="94db5-210">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="94db5-211">連絡先の別の住所。</span><span class="sxs-lookup"><span data-stu-id="94db5-211">Other addresses for the contact.</span></span>|
|<span data-ttu-id="94db5-212">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="94db5-212">parentFolderId</span></span>|<span data-ttu-id="94db5-213">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-213">String</span></span>|<span data-ttu-id="94db5-214">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="94db5-214">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="94db5-215">personalNotes</span><span class="sxs-lookup"><span data-stu-id="94db5-215">personalNotes</span></span>|<span data-ttu-id="94db5-216">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-216">String</span></span>|<span data-ttu-id="94db5-217">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="94db5-217">The user's notes about the contact.</span></span>|
|<span data-ttu-id="94db5-218">profession</span><span class="sxs-lookup"><span data-stu-id="94db5-218">profession</span></span>|<span data-ttu-id="94db5-219">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-219">String</span></span>|<span data-ttu-id="94db5-220">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="94db5-220">The contact's profession.</span></span>|
|<span data-ttu-id="94db5-221">spouseName</span><span class="sxs-lookup"><span data-stu-id="94db5-221">spouseName</span></span>|<span data-ttu-id="94db5-222">String</span><span class="sxs-lookup"><span data-stu-id="94db5-222">String</span></span>|<span data-ttu-id="94db5-223">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="94db5-223">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="94db5-224">姓</span><span class="sxs-lookup"><span data-stu-id="94db5-224">surname</span></span>|<span data-ttu-id="94db5-225">文字列</span><span class="sxs-lookup"><span data-stu-id="94db5-225">String</span></span>|<span data-ttu-id="94db5-226">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="94db5-226">The contact's surname.</span></span>|
|<span data-ttu-id="94db5-227">タイトル</span><span class="sxs-lookup"><span data-stu-id="94db5-227">title</span></span>|<span data-ttu-id="94db5-228">String</span><span class="sxs-lookup"><span data-stu-id="94db5-228">String</span></span>|<span data-ttu-id="94db5-229">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="94db5-229">The contact's title.</span></span>|
|<span data-ttu-id="94db5-230">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="94db5-230">yomiCompanyName</span></span>|<span data-ttu-id="94db5-231">String</span><span class="sxs-lookup"><span data-stu-id="94db5-231">String</span></span>|<span data-ttu-id="94db5-p107">連絡先の会社名の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="94db5-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="94db5-234">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="94db5-234">yomiGivenName</span></span>|<span data-ttu-id="94db5-235">String</span><span class="sxs-lookup"><span data-stu-id="94db5-235">String</span></span>|<span data-ttu-id="94db5-p108">連絡先の名 (ファースト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="94db5-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="94db5-238">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="94db5-238">yomiSurname</span></span>|<span data-ttu-id="94db5-239">String</span><span class="sxs-lookup"><span data-stu-id="94db5-239">String</span></span>|<span data-ttu-id="94db5-p109">連絡先の姓 (ラスト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="94db5-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="94db5-242">応答</span><span class="sxs-lookup"><span data-stu-id="94db5-242">Response</span></span>

<span data-ttu-id="94db5-243">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94db5-243">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94db5-244">例</span><span class="sxs-lookup"><span data-stu-id="94db5-244">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94db5-245">要求</span><span class="sxs-lookup"><span data-stu-id="94db5-245">Request</span></span>
<span data-ttu-id="94db5-246">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94db5-246">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contacts/{id}
Content-type: application/json
Content-length: 1977

{
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "birthday": "1974-07-22"
}
```
##### <a name="response"></a><span data-ttu-id="94db5-247">応答</span><span class="sxs-lookup"><span data-stu-id="94db5-247">Response</span></span>
<span data-ttu-id="94db5-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94db5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "https://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
