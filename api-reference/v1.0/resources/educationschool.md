---
title: educationSchool リソースの種類
description: '学校を表すリソースで、その学校のクラス、教師、学生を管理するために使用します。  '
localization_priority: Normal
ms.openlocfilehash: b957355bc132fd0b90c4bf623e68619d7ebcd0ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877022"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="ab920-103">educationSchool リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab920-103">educationSchool resource type</span></span>

<span data-ttu-id="ab920-104">学校を表すリソースで、その学校のクラス、教師、学生を管理するために使用します。</span><span class="sxs-lookup"><span data-stu-id="ab920-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="ab920-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab920-105">Methods</span></span>

| <span data-ttu-id="ab920-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab920-106">Method</span></span>           | <span data-ttu-id="ab920-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ab920-107">Return Type</span></span>    |<span data-ttu-id="ab920-108">説明</span><span class="sxs-lookup"><span data-stu-id="ab920-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab920-109">Get</span><span class="sxs-lookup"><span data-stu-id="ab920-109">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="ab920-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="ab920-110">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="ab920-111">**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ab920-111">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="ab920-112">Add class</span><span class="sxs-lookup"><span data-stu-id="ab920-112">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="ab920-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="ab920-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="ab920-114">classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。</span><span class="sxs-lookup"><span data-stu-id="ab920-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="ab920-115">List classes</span><span class="sxs-lookup"><span data-stu-id="ab920-115">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="ab920-116">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ab920-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="ab920-117">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ab920-117">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="ab920-118">Remove class</span><span class="sxs-lookup"><span data-stu-id="ab920-118">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="ab920-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="ab920-119">educationClass</span></span>](educationclass.md)| <span data-ttu-id="ab920-120">classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。</span><span class="sxs-lookup"><span data-stu-id="ab920-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="ab920-121">Add user</span><span class="sxs-lookup"><span data-stu-id="ab920-121">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="ab920-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="ab920-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ab920-123">**users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="ab920-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="ab920-124">List users</span><span class="sxs-lookup"><span data-stu-id="ab920-124">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="ab920-125">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ab920-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="ab920-126">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ab920-126">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="ab920-127">Remove user</span><span class="sxs-lookup"><span data-stu-id="ab920-127">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="ab920-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="ab920-128">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ab920-129">**users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="ab920-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="ab920-130">Update</span><span class="sxs-lookup"><span data-stu-id="ab920-130">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="ab920-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="ab920-131">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="ab920-132">**educationSchool** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab920-132">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="ab920-133">Delete</span><span class="sxs-lookup"><span data-stu-id="ab920-133">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="ab920-134">なし</span><span class="sxs-lookup"><span data-stu-id="ab920-134">None</span></span> |<span data-ttu-id="ab920-135">**educationSchool** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="ab920-135">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ab920-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab920-136">Properties</span></span>
| <span data-ttu-id="ab920-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab920-137">Property</span></span>     | <span data-ttu-id="ab920-138">種類</span><span class="sxs-lookup"><span data-stu-id="ab920-138">Type</span></span>   |<span data-ttu-id="ab920-139">説明</span><span class="sxs-lookup"><span data-stu-id="ab920-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab920-140">ID</span><span class="sxs-lookup"><span data-stu-id="ab920-140">id</span></span>|<span data-ttu-id="ab920-141">String</span><span class="sxs-lookup"><span data-stu-id="ab920-141">String</span></span>|<span data-ttu-id="ab920-142">この学校の GUID。</span><span class="sxs-lookup"><span data-stu-id="ab920-142">GUID of this school.</span></span>|
|<span data-ttu-id="ab920-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ab920-143">displayName</span></span>| <span data-ttu-id="ab920-144">String</span><span class="sxs-lookup"><span data-stu-id="ab920-144">String</span></span>| <span data-ttu-id="ab920-145">学校の表示名。</span><span class="sxs-lookup"><span data-stu-id="ab920-145">Display name of the school.</span></span>| 
|<span data-ttu-id="ab920-146">説明</span><span class="sxs-lookup"><span data-stu-id="ab920-146">description</span></span>| <span data-ttu-id="ab920-147">String</span><span class="sxs-lookup"><span data-stu-id="ab920-147">String</span></span> | <span data-ttu-id="ab920-148">学校の説明。</span><span class="sxs-lookup"><span data-stu-id="ab920-148">Description of the school.</span></span>| 
|<span data-ttu-id="ab920-149">status</span><span class="sxs-lookup"><span data-stu-id="ab920-149">status</span></span>| <span data-ttu-id="ab920-150">文字列</span><span class="sxs-lookup"><span data-stu-id="ab920-150">string</span></span>| <span data-ttu-id="ab920-151">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ab920-151">Read-Only.</span></span> <span data-ttu-id="ab920-152">可能な値: `inactive`、 `active`、 `expired`、 `deleteable`。</span><span class="sxs-lookup"><span data-stu-id="ab920-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="ab920-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="ab920-153">externalSource</span></span>| <span data-ttu-id="ab920-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="ab920-154">educationExternalSource</span></span>| <span data-ttu-id="ab920-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ab920-155">Read-Only.</span></span>  <span data-ttu-id="ab920-156">可能な値: `sis`、 `manual`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ab920-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ab920-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="ab920-157">principalEmail</span></span>| <span data-ttu-id="ab920-158">String</span><span class="sxs-lookup"><span data-stu-id="ab920-158">String</span></span>| <span data-ttu-id="ab920-159">プリンシパルの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="ab920-159">Email address of the principal.</span></span>|
|<span data-ttu-id="ab920-160">principalName</span><span class="sxs-lookup"><span data-stu-id="ab920-160">principalName</span></span>| <span data-ttu-id="ab920-161">String</span><span class="sxs-lookup"><span data-stu-id="ab920-161">String</span></span> | <span data-ttu-id="ab920-162">プリンシパルの名前。</span><span class="sxs-lookup"><span data-stu-id="ab920-162">Name of the principal.</span></span>|
|<span data-ttu-id="ab920-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="ab920-163">externalPrincipalId</span></span>| <span data-ttu-id="ab920-164">String</span><span class="sxs-lookup"><span data-stu-id="ab920-164">String</span></span> | <span data-ttu-id="ab920-165">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="ab920-165">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="ab920-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="ab920-166">highestGrade</span></span>|<span data-ttu-id="ab920-167">String</span><span class="sxs-lookup"><span data-stu-id="ab920-167">String</span></span>| <span data-ttu-id="ab920-168">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="ab920-168">Highest grade taught.</span></span> |
|<span data-ttu-id="ab920-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="ab920-169">lowestGrade</span></span>|<span data-ttu-id="ab920-170">String</span><span class="sxs-lookup"><span data-stu-id="ab920-170">String</span></span>| <span data-ttu-id="ab920-171">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="ab920-171">Lowest grade taught.</span></span> |
|<span data-ttu-id="ab920-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="ab920-172">schoolNumber</span></span>|<span data-ttu-id="ab920-173">String</span><span class="sxs-lookup"><span data-stu-id="ab920-173">String</span></span>| <span data-ttu-id="ab920-174">学校番号。</span><span class="sxs-lookup"><span data-stu-id="ab920-174">School Number.</span></span>|
|<span data-ttu-id="ab920-175">externalId</span><span class="sxs-lookup"><span data-stu-id="ab920-175">externalId</span></span>|<span data-ttu-id="ab920-176">String</span><span class="sxs-lookup"><span data-stu-id="ab920-176">String</span></span>| <span data-ttu-id="ab920-177">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="ab920-177">ID of school in syncing system.</span></span> |
|<span data-ttu-id="ab920-178">phone</span><span class="sxs-lookup"><span data-stu-id="ab920-178">phone</span></span>|<span data-ttu-id="ab920-179">String</span><span class="sxs-lookup"><span data-stu-id="ab920-179">String</span></span>| <span data-ttu-id="ab920-180">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="ab920-180">Phone number of school.</span></span> |
|<span data-ttu-id="ab920-181">fax</span><span class="sxs-lookup"><span data-stu-id="ab920-181">fax</span></span>|<span data-ttu-id="ab920-182">String</span><span class="sxs-lookup"><span data-stu-id="ab920-182">String</span></span>| <span data-ttu-id="ab920-183">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="ab920-183">Fax number of school.</span></span> |
|<span data-ttu-id="ab920-184">address</span><span class="sxs-lookup"><span data-stu-id="ab920-184">address</span></span>|[<span data-ttu-id="ab920-185">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="ab920-185">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="ab920-186">学校の住所。</span><span class="sxs-lookup"><span data-stu-id="ab920-186">Address of the school.</span></span>|
|<span data-ttu-id="ab920-187">createdBy</span><span class="sxs-lookup"><span data-stu-id="ab920-187">createdBy</span></span>|[<span data-ttu-id="ab920-188">identitySet</span><span class="sxs-lookup"><span data-stu-id="ab920-188">identitySet</span></span>](identityset.md)|<span data-ttu-id="ab920-189">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="ab920-189">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab920-190">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab920-190">Relationships</span></span>
| <span data-ttu-id="ab920-191">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab920-191">Relationship</span></span> | <span data-ttu-id="ab920-192">型</span><span class="sxs-lookup"><span data-stu-id="ab920-192">Type</span></span>   |<span data-ttu-id="ab920-193">説明</span><span class="sxs-lookup"><span data-stu-id="ab920-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab920-194">classes</span><span class="sxs-lookup"><span data-stu-id="ab920-194">classes</span></span>|<span data-ttu-id="ab920-195">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ab920-195">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="ab920-196">学校で授業しているクラス。</span><span class="sxs-lookup"><span data-stu-id="ab920-196">Classes taught at the school.</span></span> <span data-ttu-id="ab920-197">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ab920-197">Nullable.</span></span>|
|<span data-ttu-id="ab920-198">users</span><span class="sxs-lookup"><span data-stu-id="ab920-198">users</span></span>|<span data-ttu-id="ab920-199">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ab920-199">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="ab920-200">学校のユーザー。</span><span class="sxs-lookup"><span data-stu-id="ab920-200">Users in the school.</span></span> <span data-ttu-id="ab920-201">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ab920-201">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab920-202">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab920-202">JSON representation</span></span>

<span data-ttu-id="ab920-203">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab920-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
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
