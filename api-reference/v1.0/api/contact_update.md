# <a name="update-contact"></a><span data-ttu-id="db524-101">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="db524-101">Update contact</span></span>

<span data-ttu-id="db524-102">連絡先オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="db524-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="db524-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db524-103">Permissions</span></span>
<span data-ttu-id="db524-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db524-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="db524-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db524-106">Permission type</span></span>      | <span data-ttu-id="db524-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db524-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db524-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db524-108">Delegated (work or school account)</span></span> | <span data-ttu-id="db524-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db524-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="db524-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db524-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db524-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db524-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="db524-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db524-112">Application</span></span> | <span data-ttu-id="db524-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db524-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="db524-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db524-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="db524-115">ユーザーの既定 [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="db524-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="db524-116">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="db524-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="db524-p102">[contactFolder](../resources/mailfolder.md) の子フォルダー内に含まれる [連絡先](../resources/contact.md)。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="db524-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="db524-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db524-119">Request headers</span></span>
| <span data-ttu-id="db524-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db524-120">Header</span></span>       | <span data-ttu-id="db524-121">値</span><span class="sxs-lookup"><span data-stu-id="db524-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db524-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db524-122">Authorization</span></span>  | <span data-ttu-id="db524-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="db524-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="db524-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db524-125">Content-Type</span></span>  | <span data-ttu-id="db524-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="db524-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db524-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="db524-128">Request body</span></span>
<span data-ttu-id="db524-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="db524-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="db524-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db524-132">Property</span></span>     | <span data-ttu-id="db524-133">型</span><span class="sxs-lookup"><span data-stu-id="db524-133">Type</span></span>   |<span data-ttu-id="db524-134">説明</span><span class="sxs-lookup"><span data-stu-id="db524-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db524-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="db524-135">assistantName</span></span>|<span data-ttu-id="db524-136">String</span><span class="sxs-lookup"><span data-stu-id="db524-136">String</span></span>|<span data-ttu-id="db524-137">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="db524-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="db524-138">birthday</span><span class="sxs-lookup"><span data-stu-id="db524-138">birthday</span></span>|<span data-ttu-id="db524-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db524-139">DateTimeOffset</span></span>|<span data-ttu-id="db524-140">連絡先の誕生日です。</span><span class="sxs-lookup"><span data-stu-id="db524-140">The contact's birthday.</span></span>|
|<span data-ttu-id="db524-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="db524-141">businessAddress</span></span>|[<span data-ttu-id="db524-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="db524-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="db524-143">連絡先の勤務先の住所。</span><span class="sxs-lookup"><span data-stu-id="db524-143">The contact's business address.</span></span>|
|<span data-ttu-id="db524-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="db524-144">businessHomePage</span></span>|<span data-ttu-id="db524-145">String</span><span class="sxs-lookup"><span data-stu-id="db524-145">String</span></span>|<span data-ttu-id="db524-146">連絡先の勤務先のホーム ページ。</span><span class="sxs-lookup"><span data-stu-id="db524-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="db524-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="db524-147">businessPhones</span></span>|<span data-ttu-id="db524-148">String</span><span class="sxs-lookup"><span data-stu-id="db524-148">String</span></span>|<span data-ttu-id="db524-149">連絡先の勤務先の電話番号。</span><span class="sxs-lookup"><span data-stu-id="db524-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="db524-150">categories</span><span class="sxs-lookup"><span data-stu-id="db524-150">categories</span></span>|<span data-ttu-id="db524-151">String</span><span class="sxs-lookup"><span data-stu-id="db524-151">String</span></span>|<span data-ttu-id="db524-152">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="db524-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="db524-153">children</span><span class="sxs-lookup"><span data-stu-id="db524-153">children</span></span>|<span data-ttu-id="db524-154">String</span><span class="sxs-lookup"><span data-stu-id="db524-154">String</span></span>|<span data-ttu-id="db524-155">連絡先の子供の名前。</span><span class="sxs-lookup"><span data-stu-id="db524-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="db524-156">companyName</span><span class="sxs-lookup"><span data-stu-id="db524-156">companyName</span></span>|<span data-ttu-id="db524-157">String</span><span class="sxs-lookup"><span data-stu-id="db524-157">String</span></span>|<span data-ttu-id="db524-158">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="db524-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="db524-159">department</span><span class="sxs-lookup"><span data-stu-id="db524-159">department</span></span>|<span data-ttu-id="db524-160">String</span><span class="sxs-lookup"><span data-stu-id="db524-160">String</span></span>|<span data-ttu-id="db524-161">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="db524-161">The contact's department.</span></span>|
|<span data-ttu-id="db524-162">displayName</span><span class="sxs-lookup"><span data-stu-id="db524-162">displayName</span></span>|<span data-ttu-id="db524-163">String</span><span class="sxs-lookup"><span data-stu-id="db524-163">String</span></span>|<span data-ttu-id="db524-164">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="db524-164">The contact's display name.</span></span>|
|<span data-ttu-id="db524-165">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="db524-165">emailAddresses</span></span>|<span data-ttu-id="db524-166">[EmailAddress](../resources/emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="db524-166">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="db524-167">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="db524-167">The contact's email addresses.</span></span>|
|<span data-ttu-id="db524-168">fileAs</span><span class="sxs-lookup"><span data-stu-id="db524-168">fileAs</span></span>|<span data-ttu-id="db524-169">String</span><span class="sxs-lookup"><span data-stu-id="db524-169">String</span></span>|<span data-ttu-id="db524-170">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="db524-170">The name the contact is filed under.</span></span>|
|<span data-ttu-id="db524-171">generation</span><span class="sxs-lookup"><span data-stu-id="db524-171">generation</span></span>|<span data-ttu-id="db524-172">String</span><span class="sxs-lookup"><span data-stu-id="db524-172">String</span></span>|<span data-ttu-id="db524-173">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="db524-173">The contact's generation.</span></span>|
|<span data-ttu-id="db524-174">givenName</span><span class="sxs-lookup"><span data-stu-id="db524-174">givenName</span></span>|<span data-ttu-id="db524-175">String</span><span class="sxs-lookup"><span data-stu-id="db524-175">String</span></span>|<span data-ttu-id="db524-176">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="db524-176">The contact's given name.</span></span>|
|<span data-ttu-id="db524-177">homeAddress</span><span class="sxs-lookup"><span data-stu-id="db524-177">homeAddress</span></span>|[<span data-ttu-id="db524-178">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="db524-178">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="db524-179">連絡先の自宅住所。</span><span class="sxs-lookup"><span data-stu-id="db524-179">The contact's home address.</span></span>|
|<span data-ttu-id="db524-180">homePhones</span><span class="sxs-lookup"><span data-stu-id="db524-180">homePhones</span></span>|<span data-ttu-id="db524-181">String collection</span><span class="sxs-lookup"><span data-stu-id="db524-181">String collection</span></span>|<span data-ttu-id="db524-182">連絡先の自宅の電話番号。</span><span class="sxs-lookup"><span data-stu-id="db524-182">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="db524-183">imAddresses</span><span class="sxs-lookup"><span data-stu-id="db524-183">imAddresses</span></span>|<span data-ttu-id="db524-184">String</span><span class="sxs-lookup"><span data-stu-id="db524-184">String</span></span>|<span data-ttu-id="db524-185">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="db524-185">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="db524-186">initials</span><span class="sxs-lookup"><span data-stu-id="db524-186">initials</span></span>|<span data-ttu-id="db524-187">String</span><span class="sxs-lookup"><span data-stu-id="db524-187">String</span></span>|<span data-ttu-id="db524-188">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="db524-188">The contact's initials.</span></span>|
|<span data-ttu-id="db524-189">jobTitle</span><span class="sxs-lookup"><span data-stu-id="db524-189">jobTitle</span></span>|<span data-ttu-id="db524-190">String</span><span class="sxs-lookup"><span data-stu-id="db524-190">String</span></span>|<span data-ttu-id="db524-191">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="db524-191">The contact’s job title.</span></span>|
|<span data-ttu-id="db524-192">manager</span><span class="sxs-lookup"><span data-stu-id="db524-192">manager</span></span>|<span data-ttu-id="db524-193">String</span><span class="sxs-lookup"><span data-stu-id="db524-193">String</span></span>|<span data-ttu-id="db524-194">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="db524-194">The name of the contact's manager.</span></span>
|<span data-ttu-id="db524-195">middleName</span><span class="sxs-lookup"><span data-stu-id="db524-195">middleName</span></span>|<span data-ttu-id="db524-196">String</span><span class="sxs-lookup"><span data-stu-id="db524-196">String</span></span>|<span data-ttu-id="db524-197">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="db524-197">The contact's middle name.</span></span>|
|<span data-ttu-id="db524-198">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="db524-198">mobilePhone</span></span>|<span data-ttu-id="db524-199">String</span><span class="sxs-lookup"><span data-stu-id="db524-199">String</span></span>|<span data-ttu-id="db524-200">連絡先の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="db524-200">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="db524-201">nickName</span><span class="sxs-lookup"><span data-stu-id="db524-201">nickName</span></span>|<span data-ttu-id="db524-202">String</span><span class="sxs-lookup"><span data-stu-id="db524-202">String</span></span>|<span data-ttu-id="db524-203">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="db524-203">The contact's nickname.</span></span>|
|<span data-ttu-id="db524-204">officeLocation</span><span class="sxs-lookup"><span data-stu-id="db524-204">officeLocation</span></span>|<span data-ttu-id="db524-205">String</span><span class="sxs-lookup"><span data-stu-id="db524-205">String</span></span>|<span data-ttu-id="db524-206">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="db524-206">The location of the contact's office.</span></span>|
|<span data-ttu-id="db524-207">otherAddress</span><span class="sxs-lookup"><span data-stu-id="db524-207">otherAddress</span></span>|[<span data-ttu-id="db524-208">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="db524-208">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="db524-209">連絡先の別の住所。</span><span class="sxs-lookup"><span data-stu-id="db524-209">Other addresses for the contact.</span></span>|
|<span data-ttu-id="db524-210">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="db524-210">parentFolderId</span></span>|<span data-ttu-id="db524-211">String</span><span class="sxs-lookup"><span data-stu-id="db524-211">String</span></span>|<span data-ttu-id="db524-212">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="db524-212">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="db524-213">personalNotes</span><span class="sxs-lookup"><span data-stu-id="db524-213">personalNotes</span></span>|<span data-ttu-id="db524-214">String</span><span class="sxs-lookup"><span data-stu-id="db524-214">String</span></span>|<span data-ttu-id="db524-215">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="db524-215">The user's notes about the contact.</span></span>|
|<span data-ttu-id="db524-216">profession</span><span class="sxs-lookup"><span data-stu-id="db524-216">profession</span></span>|<span data-ttu-id="db524-217">String</span><span class="sxs-lookup"><span data-stu-id="db524-217">String</span></span>|<span data-ttu-id="db524-218">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="db524-218">The contact's profession.</span></span>|
|<span data-ttu-id="db524-219">spouseName</span><span class="sxs-lookup"><span data-stu-id="db524-219">spouseName</span></span>|<span data-ttu-id="db524-220">String</span><span class="sxs-lookup"><span data-stu-id="db524-220">String</span></span>|<span data-ttu-id="db524-221">連絡先の配偶者の名前。</span><span class="sxs-lookup"><span data-stu-id="db524-221">The name of the contact's spouse.</span></span>|
|<span data-ttu-id="db524-222">surname</span><span class="sxs-lookup"><span data-stu-id="db524-222">surname</span></span>|<span data-ttu-id="db524-223">String</span><span class="sxs-lookup"><span data-stu-id="db524-223">String</span></span>|<span data-ttu-id="db524-224">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="db524-224">The contact's surname.</span></span>|
|<span data-ttu-id="db524-225">title</span><span class="sxs-lookup"><span data-stu-id="db524-225">title</span></span>|<span data-ttu-id="db524-226">String</span><span class="sxs-lookup"><span data-stu-id="db524-226">String</span></span>|<span data-ttu-id="db524-227">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="db524-227">The contact's title.</span></span>|
|<span data-ttu-id="db524-228">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="db524-228">yomiCompanyName</span></span>|<span data-ttu-id="db524-229">String</span><span class="sxs-lookup"><span data-stu-id="db524-229">String</span></span>|<span data-ttu-id="db524-p106">連絡先の会社名の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="db524-p106">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="db524-232">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="db524-232">yomiGivenName</span></span>|<span data-ttu-id="db524-233">String</span><span class="sxs-lookup"><span data-stu-id="db524-233">String</span></span>|<span data-ttu-id="db524-p107">連絡先の名 (ファースト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="db524-p107">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="db524-236">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="db524-236">yomiSurname</span></span>|<span data-ttu-id="db524-237">String</span><span class="sxs-lookup"><span data-stu-id="db524-237">String</span></span>|<span data-ttu-id="db524-p108">連絡先の姓 (ラスト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="db524-p108">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="db524-240">応答</span><span class="sxs-lookup"><span data-stu-id="db524-240">Response</span></span>

<span data-ttu-id="db524-241">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="db524-241">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db524-242">例</span><span class="sxs-lookup"><span data-stu-id="db524-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db524-243">要求</span><span class="sxs-lookup"><span data-stu-id="db524-243">Request</span></span>
<span data-ttu-id="db524-244">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db524-244">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="db524-245">応答</span><span class="sxs-lookup"><span data-stu-id="db524-245">Response</span></span>
<span data-ttu-id="db524-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="db524-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "http://www.contoso.com",
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
