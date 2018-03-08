# <a name="educationschool-resource-type"></a><span data-ttu-id="cf17e-101">educationSchool リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf17e-101">educationSchool resource type</span></span>

<span data-ttu-id="cf17e-102">学校を表すリソースで、その学校のクラス、教師、学生を管理するために使用します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-102">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="cf17e-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf17e-103">Methods</span></span>

| <span data-ttu-id="cf17e-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf17e-104">Method</span></span>           | <span data-ttu-id="cf17e-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cf17e-105">Return Type</span></span>    |<span data-ttu-id="cf17e-106">説明</span><span class="sxs-lookup"><span data-stu-id="cf17e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf17e-107">Get</span><span class="sxs-lookup"><span data-stu-id="cf17e-107">Get</span></span>](../api/educationschool_get.md) | [<span data-ttu-id="cf17e-108">educationSchool</span><span class="sxs-lookup"><span data-stu-id="cf17e-108">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="cf17e-109">**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cf17e-109">Read properties and relationships of the **enrollmentTroubleshootingEvent** object.</span></span>|
|[<span data-ttu-id="cf17e-110">Add class</span><span class="sxs-lookup"><span data-stu-id="cf17e-110">Add class</span></span>](../api/educationschool_post_classes.md) |[<span data-ttu-id="cf17e-111">educationClass</span><span class="sxs-lookup"><span data-stu-id="cf17e-111">educationClass</span></span>](educationclass.md)| <span data-ttu-id="cf17e-112">classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-112">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="cf17e-113">List classes</span><span class="sxs-lookup"><span data-stu-id="cf17e-113">List classes</span></span>](../api/educationschool_list_classes.md) |<span data-ttu-id="cf17e-114">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cf17e-114">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="cf17e-115">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-115">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="cf17e-116">Remove class</span><span class="sxs-lookup"><span data-stu-id="cf17e-116">Remove class</span></span>](../api/educationschool_delete_classes.md) |[<span data-ttu-id="cf17e-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="cf17e-117">educationClass</span></span>](educationclass.md)| <span data-ttu-id="cf17e-118">classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-118">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="cf17e-119">Add user</span><span class="sxs-lookup"><span data-stu-id="cf17e-119">Add user</span></span>](../api/educationschool_post_users.md) |[<span data-ttu-id="cf17e-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="cf17e-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="cf17e-121">**users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-121">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="cf17e-122">List users</span><span class="sxs-lookup"><span data-stu-id="cf17e-122">List users</span></span>](../api/educationschool_list_users.md) |<span data-ttu-id="cf17e-123">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cf17e-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="cf17e-124">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-124">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="cf17e-125">Remove user</span><span class="sxs-lookup"><span data-stu-id="cf17e-125">Remove user</span></span>](../api/educationschool_delete_users.md) |[<span data-ttu-id="cf17e-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="cf17e-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="cf17e-127">**users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-127">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="cf17e-128">Update</span><span class="sxs-lookup"><span data-stu-id="cf17e-128">Update</span></span>](../api/educationschool_update.md) | [<span data-ttu-id="cf17e-129">educationSchool</span><span class="sxs-lookup"><span data-stu-id="cf17e-129">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="cf17e-130">**educationSchool** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-130">Update an **event** object.</span></span> |
|[<span data-ttu-id="cf17e-131">Delete</span><span class="sxs-lookup"><span data-stu-id="cf17e-131">Delete</span></span>](../api/educationschool_delete.md) | <span data-ttu-id="cf17e-132">なし</span><span class="sxs-lookup"><span data-stu-id="cf17e-132">None</span></span> |<span data-ttu-id="cf17e-133">**educationSchool** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-133">Delete an **event** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cf17e-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf17e-134">Properties</span></span>
| <span data-ttu-id="cf17e-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf17e-135">Property</span></span>     | <span data-ttu-id="cf17e-136">型</span><span class="sxs-lookup"><span data-stu-id="cf17e-136">Type</span></span>   |<span data-ttu-id="cf17e-137">説明</span><span class="sxs-lookup"><span data-stu-id="cf17e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf17e-138">id</span><span class="sxs-lookup"><span data-stu-id="cf17e-138">id</span></span>|<span data-ttu-id="cf17e-139">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-139">String</span></span>|<span data-ttu-id="cf17e-140">この学校の GUID。</span><span class="sxs-lookup"><span data-stu-id="cf17e-140">GUID of this school.</span></span>|
|<span data-ttu-id="cf17e-141">displayName</span><span class="sxs-lookup"><span data-stu-id="cf17e-141">displayName</span></span>| <span data-ttu-id="cf17e-142">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-142">String</span></span>| <span data-ttu-id="cf17e-143">学校の表示名。</span><span class="sxs-lookup"><span data-stu-id="cf17e-143">Display name of the item</span></span>| 
|<span data-ttu-id="cf17e-144">description</span><span class="sxs-lookup"><span data-stu-id="cf17e-144">description</span></span>| <span data-ttu-id="cf17e-145">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-145">String</span></span> | <span data-ttu-id="cf17e-146">学校の説明。</span><span class="sxs-lookup"><span data-stu-id="cf17e-146">Description of the school.</span></span>| 
|<span data-ttu-id="cf17e-147">status</span><span class="sxs-lookup"><span data-stu-id="cf17e-147">status</span></span>| <span data-ttu-id="cf17e-148">string</span><span class="sxs-lookup"><span data-stu-id="cf17e-148">string</span></span>| <span data-ttu-id="cf17e-149">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="cf17e-149">Read-only.</span></span> <span data-ttu-id="cf17e-150">使用可能な値: `inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="cf17e-150">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="cf17e-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="cf17e-151">externalSource</span></span>| <span data-ttu-id="cf17e-152">string</span><span class="sxs-lookup"><span data-stu-id="cf17e-152">string</span></span>| <span data-ttu-id="cf17e-153">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="cf17e-153">Read-only.</span></span>  <span data-ttu-id="cf17e-154">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="cf17e-154">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="cf17e-155">principalEmail</span><span class="sxs-lookup"><span data-stu-id="cf17e-155">principalEmail</span></span>| <span data-ttu-id="cf17e-156">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-156">String</span></span>| <span data-ttu-id="cf17e-157">プリンシパルの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="cf17e-157">Email address of the principal.</span></span>|
|<span data-ttu-id="cf17e-158">principalName</span><span class="sxs-lookup"><span data-stu-id="cf17e-158">PrincipalName</span></span>| <span data-ttu-id="cf17e-159">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-159">String</span></span> | <span data-ttu-id="cf17e-160">プリンシパルの名前。</span><span class="sxs-lookup"><span data-stu-id="cf17e-160">Name of the principal.</span></span>|
|<span data-ttu-id="cf17e-161">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="cf17e-161">externalPrincipalId</span></span>| <span data-ttu-id="cf17e-162">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-162">String</span></span> | <span data-ttu-id="cf17e-163">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="cf17e-163">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="cf17e-164">highestGrade</span><span class="sxs-lookup"><span data-stu-id="cf17e-164">highestGrade</span></span>|<span data-ttu-id="cf17e-165">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-165">String</span></span>| <span data-ttu-id="cf17e-166">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="cf17e-166">Highest grade taught.</span></span> |
|<span data-ttu-id="cf17e-167">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="cf17e-167">lowestGrade</span></span>|<span data-ttu-id="cf17e-168">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-168">String</span></span>| <span data-ttu-id="cf17e-169">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="cf17e-169">Lowest grade taught.</span></span> |
|<span data-ttu-id="cf17e-170">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="cf17e-170">schoolNumber</span></span>|<span data-ttu-id="cf17e-171">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-171">String</span></span>| <span data-ttu-id="cf17e-172">学校番号。</span><span class="sxs-lookup"><span data-stu-id="cf17e-172">School Number.</span></span>|
|<span data-ttu-id="cf17e-173">externalId</span><span class="sxs-lookup"><span data-stu-id="cf17e-173">externalId</span></span>|<span data-ttu-id="cf17e-174">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-174">String</span></span>| <span data-ttu-id="cf17e-175">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="cf17e-175">ID of school in syncing system.</span></span> |
|<span data-ttu-id="cf17e-176">phone</span><span class="sxs-lookup"><span data-stu-id="cf17e-176">Phone</span></span>|<span data-ttu-id="cf17e-177">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-177">String</span></span>| <span data-ttu-id="cf17e-178">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="cf17e-178">Phone number of school.</span></span> |
|<span data-ttu-id="cf17e-179">fax</span><span class="sxs-lookup"><span data-stu-id="cf17e-179">fax</span></span>|<span data-ttu-id="cf17e-180">String</span><span class="sxs-lookup"><span data-stu-id="cf17e-180">String</span></span>| <span data-ttu-id="cf17e-181">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="cf17e-181">Fax number of school.</span></span> |
|<span data-ttu-id="cf17e-182">address</span><span class="sxs-lookup"><span data-stu-id="cf17e-182">address</span></span>|[<span data-ttu-id="cf17e-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="cf17e-183">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="cf17e-184">学校の住所。</span><span class="sxs-lookup"><span data-stu-id="cf17e-184">Address of the school.</span></span>|
|<span data-ttu-id="cf17e-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="cf17e-185">createdBy</span></span>|[<span data-ttu-id="cf17e-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="cf17e-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="cf17e-187">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="cf17e-187">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="cf17e-188">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cf17e-188">Relationships</span></span>
| <span data-ttu-id="cf17e-189">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cf17e-189">Relationship</span></span> | <span data-ttu-id="cf17e-190">型</span><span class="sxs-lookup"><span data-stu-id="cf17e-190">Type</span></span>   |<span data-ttu-id="cf17e-191">説明</span><span class="sxs-lookup"><span data-stu-id="cf17e-191">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf17e-192">classes</span><span class="sxs-lookup"><span data-stu-id="cf17e-192">Classes</span></span>|<span data-ttu-id="cf17e-193">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cf17e-193">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="cf17e-194">学校で授業しているクラス。</span><span class="sxs-lookup"><span data-stu-id="cf17e-194">Classes taught at the school.</span></span> <span data-ttu-id="cf17e-195">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cf17e-195">Nullable.</span></span>|
|<span data-ttu-id="cf17e-196">users</span><span class="sxs-lookup"><span data-stu-id="cf17e-196">users</span></span>|<span data-ttu-id="cf17e-197">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cf17e-197">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="cf17e-198">学校のユーザー。</span><span class="sxs-lookup"><span data-stu-id="cf17e-198">Users in the school.</span></span> <span data-ttu-id="cf17e-199">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cf17e-199">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf17e-200">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf17e-200">JSON representation</span></span>

<span data-ttu-id="cf17e-201">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf17e-201">The following is a JSON representation of the resource.</span></span>

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
