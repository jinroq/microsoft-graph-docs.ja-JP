# <a name="educationschool-resource-type"></a><span data-ttu-id="51acd-101">educationSchool リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="51acd-101">educationSchool resource type</span></span>

<span data-ttu-id="51acd-102">学校。</span><span class="sxs-lookup"><span data-stu-id="51acd-102">A school entity.</span></span> <span data-ttu-id="51acd-103">現時点で、**educationSchool** リソースは [administrativeUnit](../../beta/resources/administrativeunit.md) リソースと一致していて、同じ ID を共有しています。</span><span class="sxs-lookup"><span data-stu-id="51acd-103">The **educationSchool** resource currently corresponds to an [administrativeUnit](../../beta/resources/administrativeunit.md) resource and shares the same ID.</span></span>  

><span data-ttu-id="51acd-104">**注:** 現在の **administrativeUnit** リソースと **educationOrganization** リソースはベータ版です。</span><span class="sxs-lookup"><span data-stu-id="51acd-104">**Note:**  The **administrativeUnit** and **educationOrganization** resources are currently in beta.</span></span> <span data-ttu-id="51acd-105">これらのリソースを使用する場合は、定期的に[変更ログ](../../../concepts/changelog.md)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="51acd-105">If you're using these resources, be sure to review the [Changelog](../../../concepts/changelog.md) periodically.</span></span> <span data-ttu-id="51acd-106">Microsoft Graph API リソースが v1.0 エンドポイントにリリースされるときに、これについて変更ログに記載する予定です。</span><span class="sxs-lookup"><span data-stu-id="51acd-106">When Microsoft Graph API resources are released to the v1.0  endpoint, we'll note this in the Changelog.</span></span> <span data-ttu-id="51acd-107">アプリで **administrativeUnit** リソースまたは **educationOrganization** リソースを使用する場合は、次のコード ブロックに示すように、ベース要求 URL を宣言する必要があります。</span><span class="sxs-lookup"><span data-stu-id="51acd-107">If your app consumes the **administrativeUnit** or **educationOrganization** resources, you will need to declare base request URLs as shown in the the following code block.</span></span>  
  ```JavaScript
  var v1BaseUrl = “https://graph.microsoft.com/v1.0/education”;
  var betaBaseUrl = “https://graph.microsoft.com/beta/education”;  // for administrativeUnit and educationOrganization
  ```

<span data-ttu-id="51acd-108">このリソースは、[educationOrganization](../../beta/resources/educationorganization.md) のサブタイプです。</span><span class="sxs-lookup"><span data-stu-id="51acd-108">This resource is a subtype of [educationOrganization](../../beta/resources/educationorganization.md).</span></span>


## <a name="methods"></a><span data-ttu-id="51acd-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="51acd-109">Methods</span></span>

| <span data-ttu-id="51acd-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="51acd-110">Method</span></span>           | <span data-ttu-id="51acd-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="51acd-111">Return Type</span></span>    |<span data-ttu-id="51acd-112">説明</span><span class="sxs-lookup"><span data-stu-id="51acd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51acd-113">Get</span><span class="sxs-lookup"><span data-stu-id="51acd-113">Get</span></span>](../api/educationschool_get.md) | [<span data-ttu-id="51acd-114">educationSchool</span><span class="sxs-lookup"><span data-stu-id="51acd-114">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="51acd-115">**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="51acd-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="51acd-116">Add class</span><span class="sxs-lookup"><span data-stu-id="51acd-116">Add class</span></span>](../api/educationschool_post_classes.md) |[<span data-ttu-id="51acd-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="51acd-117">educationClass</span></span>](educationclass.md)| <span data-ttu-id="51acd-118">classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。</span><span class="sxs-lookup"><span data-stu-id="51acd-118">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="51acd-119">List classes</span><span class="sxs-lookup"><span data-stu-id="51acd-119">List classes</span></span>](../api/educationschool_list_classes.md) |<span data-ttu-id="51acd-120">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51acd-120">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="51acd-121">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="51acd-121">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="51acd-122">Remove class</span><span class="sxs-lookup"><span data-stu-id="51acd-122">Remove class</span></span>](../api/educationschool_delete_classes.md) |[<span data-ttu-id="51acd-123">educationClass</span><span class="sxs-lookup"><span data-stu-id="51acd-123">educationClass</span></span>](educationclass.md)| <span data-ttu-id="51acd-124">classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。</span><span class="sxs-lookup"><span data-stu-id="51acd-124">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="51acd-125">Add user</span><span class="sxs-lookup"><span data-stu-id="51acd-125">Add user</span></span>](../api/educationschool_post_users.md) |[<span data-ttu-id="51acd-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="51acd-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="51acd-127">**users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="51acd-127">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="51acd-128">List users</span><span class="sxs-lookup"><span data-stu-id="51acd-128">List users</span></span>](../api/educationschool_list_users.md) |<span data-ttu-id="51acd-129">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51acd-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="51acd-130">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="51acd-130">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="51acd-131">Remove user</span><span class="sxs-lookup"><span data-stu-id="51acd-131">Remove user</span></span>](../api/educationschool_delete_users.md) |[<span data-ttu-id="51acd-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="51acd-132">educationUser</span></span>](educationuser.md)| <span data-ttu-id="51acd-133">**users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="51acd-133">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="51acd-134">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="51acd-134">Get administrativeUnit</span></span>](../api/educationschool_get_administrativeunit.md) |[<span data-ttu-id="51acd-135">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="51acd-135">administrativeUnit</span></span>](../../beta/resources/administrativeunit.md)| <span data-ttu-id="51acd-136">この **educationSchool** に対応する **administrativeUnit** を取得します。</span><span class="sxs-lookup"><span data-stu-id="51acd-136">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="51acd-137">Update</span><span class="sxs-lookup"><span data-stu-id="51acd-137">Update</span></span>](../api/educationschool_update.md) | [<span data-ttu-id="51acd-138">educationSchool</span><span class="sxs-lookup"><span data-stu-id="51acd-138">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="51acd-139">**educationSchool** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="51acd-139">Update an **event** object.</span></span> |
|[<span data-ttu-id="51acd-140">Delete</span><span class="sxs-lookup"><span data-stu-id="51acd-140">Delete</span></span>](../api/educationschool_delete.md) | <span data-ttu-id="51acd-141">なし</span><span class="sxs-lookup"><span data-stu-id="51acd-141">None</span></span> |<span data-ttu-id="51acd-142">**educationSchool** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="51acd-142">Delete an **event** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="51acd-143">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51acd-143">Properties</span></span>
| <span data-ttu-id="51acd-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51acd-144">Property</span></span>     | <span data-ttu-id="51acd-145">型</span><span class="sxs-lookup"><span data-stu-id="51acd-145">Type</span></span>   |<span data-ttu-id="51acd-146">説明</span><span class="sxs-lookup"><span data-stu-id="51acd-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51acd-147">id</span><span class="sxs-lookup"><span data-stu-id="51acd-147">id</span></span>|<span data-ttu-id="51acd-148">String</span><span class="sxs-lookup"><span data-stu-id="51acd-148">String</span></span>|<span data-ttu-id="51acd-149">この学校の GUID。</span><span class="sxs-lookup"><span data-stu-id="51acd-149">GUID of this school.</span></span>|
|<span data-ttu-id="51acd-150">displayName</span><span class="sxs-lookup"><span data-stu-id="51acd-150">displayName</span></span>| <span data-ttu-id="51acd-151">String</span><span class="sxs-lookup"><span data-stu-id="51acd-151">String</span></span>| <span data-ttu-id="51acd-152">学校の表示名。</span><span class="sxs-lookup"><span data-stu-id="51acd-152">Display name of the item</span></span>| 
|<span data-ttu-id="51acd-153">description</span><span class="sxs-lookup"><span data-stu-id="51acd-153">description</span></span>| <span data-ttu-id="51acd-154">String</span><span class="sxs-lookup"><span data-stu-id="51acd-154">String</span></span> | <span data-ttu-id="51acd-155">学校の説明。</span><span class="sxs-lookup"><span data-stu-id="51acd-155">Description of the school.</span></span>| 
|<span data-ttu-id="51acd-156">status</span><span class="sxs-lookup"><span data-stu-id="51acd-156">status</span></span>| <span data-ttu-id="51acd-157">string</span><span class="sxs-lookup"><span data-stu-id="51acd-157">string</span></span>| <span data-ttu-id="51acd-158">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="51acd-158">Read-only.</span></span> <span data-ttu-id="51acd-159">使用可能な値: `inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="51acd-159">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="51acd-160">externalSource</span><span class="sxs-lookup"><span data-stu-id="51acd-160">externalSource</span></span>| <span data-ttu-id="51acd-161">string</span><span class="sxs-lookup"><span data-stu-id="51acd-161">string</span></span>| <span data-ttu-id="51acd-162">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="51acd-162">Read-only.</span></span>  <span data-ttu-id="51acd-163">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="51acd-163">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="51acd-164">principalEmail</span><span class="sxs-lookup"><span data-stu-id="51acd-164">principalEmail</span></span>| <span data-ttu-id="51acd-165">String</span><span class="sxs-lookup"><span data-stu-id="51acd-165">String</span></span>| <span data-ttu-id="51acd-166">プリンシパルの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="51acd-166">Email address of the principal.</span></span>|
|<span data-ttu-id="51acd-167">principalName</span><span class="sxs-lookup"><span data-stu-id="51acd-167">PrincipalName</span></span>| <span data-ttu-id="51acd-168">String</span><span class="sxs-lookup"><span data-stu-id="51acd-168">String</span></span> | <span data-ttu-id="51acd-169">プリンシパルの名前。</span><span class="sxs-lookup"><span data-stu-id="51acd-169">Name of the principal.</span></span>|
|<span data-ttu-id="51acd-170">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="51acd-170">externalPrincipalId</span></span>| <span data-ttu-id="51acd-171">String</span><span class="sxs-lookup"><span data-stu-id="51acd-171">String</span></span> | <span data-ttu-id="51acd-172">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="51acd-172">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="51acd-173">highestGrade</span><span class="sxs-lookup"><span data-stu-id="51acd-173">highestGrade</span></span>|<span data-ttu-id="51acd-174">String</span><span class="sxs-lookup"><span data-stu-id="51acd-174">String</span></span>| <span data-ttu-id="51acd-175">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="51acd-175">Highest grade taught.</span></span> |
|<span data-ttu-id="51acd-176">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="51acd-176">lowestGrade</span></span>|<span data-ttu-id="51acd-177">String</span><span class="sxs-lookup"><span data-stu-id="51acd-177">String</span></span>| <span data-ttu-id="51acd-178">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="51acd-178">Lowest grade taught.</span></span> |
|<span data-ttu-id="51acd-179">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="51acd-179">schoolNumber</span></span>|<span data-ttu-id="51acd-180">String</span><span class="sxs-lookup"><span data-stu-id="51acd-180">String</span></span>| <span data-ttu-id="51acd-181">学校番号。</span><span class="sxs-lookup"><span data-stu-id="51acd-181">School Number.</span></span>|
|<span data-ttu-id="51acd-182">externalId</span><span class="sxs-lookup"><span data-stu-id="51acd-182">externalId</span></span>|<span data-ttu-id="51acd-183">String</span><span class="sxs-lookup"><span data-stu-id="51acd-183">String</span></span>| <span data-ttu-id="51acd-184">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="51acd-184">ID of school in syncing system.</span></span> |
|<span data-ttu-id="51acd-185">phone</span><span class="sxs-lookup"><span data-stu-id="51acd-185">Phone</span></span>|<span data-ttu-id="51acd-186">String</span><span class="sxs-lookup"><span data-stu-id="51acd-186">String</span></span>| <span data-ttu-id="51acd-187">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="51acd-187">Phone number of school.</span></span> |
|<span data-ttu-id="51acd-188">fax</span><span class="sxs-lookup"><span data-stu-id="51acd-188">fax</span></span>|<span data-ttu-id="51acd-189">String</span><span class="sxs-lookup"><span data-stu-id="51acd-189">String</span></span>| <span data-ttu-id="51acd-190">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="51acd-190">Fax number of school.</span></span> |
|<span data-ttu-id="51acd-191">address</span><span class="sxs-lookup"><span data-stu-id="51acd-191">address</span></span>|[<span data-ttu-id="51acd-192">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="51acd-192">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="51acd-193">学校の住所。</span><span class="sxs-lookup"><span data-stu-id="51acd-193">Address of the school.</span></span>|
|<span data-ttu-id="51acd-194">createdBy</span><span class="sxs-lookup"><span data-stu-id="51acd-194">createdBy</span></span>|[<span data-ttu-id="51acd-195">identitySet</span><span class="sxs-lookup"><span data-stu-id="51acd-195">identitySet</span></span>](identityset.md)|<span data-ttu-id="51acd-196">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="51acd-196">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="51acd-197">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="51acd-197">Relationships</span></span>
| <span data-ttu-id="51acd-198">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="51acd-198">Relationship</span></span> | <span data-ttu-id="51acd-199">型</span><span class="sxs-lookup"><span data-stu-id="51acd-199">Type</span></span>   |<span data-ttu-id="51acd-200">説明</span><span class="sxs-lookup"><span data-stu-id="51acd-200">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51acd-201">classes</span><span class="sxs-lookup"><span data-stu-id="51acd-201">Classes</span></span>|<span data-ttu-id="51acd-202">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51acd-202">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="51acd-203">学校で授業しているクラス。</span><span class="sxs-lookup"><span data-stu-id="51acd-203">Classes taught at the school.</span></span> <span data-ttu-id="51acd-204">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="51acd-204">Nullable.</span></span>|
|<span data-ttu-id="51acd-205">users</span><span class="sxs-lookup"><span data-stu-id="51acd-205">users</span></span>|<span data-ttu-id="51acd-206">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51acd-206">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="51acd-207">学校のユーザー。</span><span class="sxs-lookup"><span data-stu-id="51acd-207">Users in the school.</span></span> <span data-ttu-id="51acd-208">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="51acd-208">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51acd-209">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51acd-209">JSON representation</span></span>

<span data-ttu-id="51acd-210">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="51acd-210">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
