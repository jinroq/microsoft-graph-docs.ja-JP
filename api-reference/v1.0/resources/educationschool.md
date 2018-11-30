---
title: educationSchool リソースの種類
description: '学校を表すリソースで、その学校のクラス、教師、学生を管理するために使用します。  '
ms.openlocfilehash: 8a87b3a0ceebf9a3dd66978da1bdde2d677ef63e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023924"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="499d9-103">educationSchool リソースの種類</span><span class="sxs-lookup"><span data-stu-id="499d9-103">educationSchool resource type</span></span>

<span data-ttu-id="499d9-104">学校を表すリソースで、その学校のクラス、教師、学生を管理するために使用します。</span><span class="sxs-lookup"><span data-stu-id="499d9-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="499d9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="499d9-105">Methods</span></span>

| <span data-ttu-id="499d9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="499d9-106">Method</span></span>           | <span data-ttu-id="499d9-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="499d9-107">Return Type</span></span>    |<span data-ttu-id="499d9-108">説明</span><span class="sxs-lookup"><span data-stu-id="499d9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="499d9-109">Get</span><span class="sxs-lookup"><span data-stu-id="499d9-109">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="499d9-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="499d9-110">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="499d9-111">**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="499d9-111">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="499d9-112">Add class</span><span class="sxs-lookup"><span data-stu-id="499d9-112">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="499d9-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="499d9-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="499d9-114">classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。</span><span class="sxs-lookup"><span data-stu-id="499d9-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="499d9-115">List classes</span><span class="sxs-lookup"><span data-stu-id="499d9-115">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="499d9-116">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="499d9-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="499d9-117">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="499d9-117">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="499d9-118">Remove class</span><span class="sxs-lookup"><span data-stu-id="499d9-118">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="499d9-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="499d9-119">educationClass</span></span>](educationclass.md)| <span data-ttu-id="499d9-120">classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。</span><span class="sxs-lookup"><span data-stu-id="499d9-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="499d9-121">Add user</span><span class="sxs-lookup"><span data-stu-id="499d9-121">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="499d9-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="499d9-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="499d9-123">**users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="499d9-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="499d9-124">List users</span><span class="sxs-lookup"><span data-stu-id="499d9-124">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="499d9-125">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="499d9-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="499d9-126">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="499d9-126">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="499d9-127">Remove user</span><span class="sxs-lookup"><span data-stu-id="499d9-127">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="499d9-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="499d9-128">educationUser</span></span>](educationuser.md)| <span data-ttu-id="499d9-129">**users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="499d9-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="499d9-130">Update</span><span class="sxs-lookup"><span data-stu-id="499d9-130">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="499d9-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="499d9-131">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="499d9-132">**educationSchool** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="499d9-132">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="499d9-133">Delete</span><span class="sxs-lookup"><span data-stu-id="499d9-133">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="499d9-134">なし</span><span class="sxs-lookup"><span data-stu-id="499d9-134">None</span></span> |<span data-ttu-id="499d9-135">**educationSchool** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="499d9-135">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="499d9-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="499d9-136">Properties</span></span>
| <span data-ttu-id="499d9-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="499d9-137">Property</span></span>     | <span data-ttu-id="499d9-138">型</span><span class="sxs-lookup"><span data-stu-id="499d9-138">Type</span></span>   |<span data-ttu-id="499d9-139">説明</span><span class="sxs-lookup"><span data-stu-id="499d9-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="499d9-140">id</span><span class="sxs-lookup"><span data-stu-id="499d9-140">id</span></span>|<span data-ttu-id="499d9-141">String</span><span class="sxs-lookup"><span data-stu-id="499d9-141">String</span></span>|<span data-ttu-id="499d9-142">この学校の GUID。</span><span class="sxs-lookup"><span data-stu-id="499d9-142">GUID of this school.</span></span>|
|<span data-ttu-id="499d9-143">displayName</span><span class="sxs-lookup"><span data-stu-id="499d9-143">displayName</span></span>| <span data-ttu-id="499d9-144">String</span><span class="sxs-lookup"><span data-stu-id="499d9-144">String</span></span>| <span data-ttu-id="499d9-145">学校の表示名。</span><span class="sxs-lookup"><span data-stu-id="499d9-145">Display name of the school.</span></span>| 
|<span data-ttu-id="499d9-146">説明</span><span class="sxs-lookup"><span data-stu-id="499d9-146">description</span></span>| <span data-ttu-id="499d9-147">String</span><span class="sxs-lookup"><span data-stu-id="499d9-147">String</span></span> | <span data-ttu-id="499d9-148">学校の説明。</span><span class="sxs-lookup"><span data-stu-id="499d9-148">Description of the school.</span></span>| 
|<span data-ttu-id="499d9-149">status</span><span class="sxs-lookup"><span data-stu-id="499d9-149">status</span></span>| <span data-ttu-id="499d9-150">文字列</span><span class="sxs-lookup"><span data-stu-id="499d9-150">string</span></span>| <span data-ttu-id="499d9-151">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="499d9-151">Read-Only.</span></span> <span data-ttu-id="499d9-152">可能な値: `inactive`、 `active`、 `expired`、 `deleteable`。</span><span class="sxs-lookup"><span data-stu-id="499d9-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="499d9-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="499d9-153">externalSource</span></span>| <span data-ttu-id="499d9-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="499d9-154">educationExternalSource</span></span>| <span data-ttu-id="499d9-155">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="499d9-155">Read-Only.</span></span>  <span data-ttu-id="499d9-156">可能な値: `sis`、 `manual`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="499d9-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="499d9-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="499d9-157">principalEmail</span></span>| <span data-ttu-id="499d9-158">String</span><span class="sxs-lookup"><span data-stu-id="499d9-158">String</span></span>| <span data-ttu-id="499d9-159">プリンシパルの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="499d9-159">Email address of the principal.</span></span>|
|<span data-ttu-id="499d9-160">principalName</span><span class="sxs-lookup"><span data-stu-id="499d9-160">principalName</span></span>| <span data-ttu-id="499d9-161">String</span><span class="sxs-lookup"><span data-stu-id="499d9-161">String</span></span> | <span data-ttu-id="499d9-162">プリンシパルの名前。</span><span class="sxs-lookup"><span data-stu-id="499d9-162">Name of the principal.</span></span>|
|<span data-ttu-id="499d9-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="499d9-163">externalPrincipalId</span></span>| <span data-ttu-id="499d9-164">String</span><span class="sxs-lookup"><span data-stu-id="499d9-164">String</span></span> | <span data-ttu-id="499d9-165">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="499d9-165">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="499d9-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="499d9-166">highestGrade</span></span>|<span data-ttu-id="499d9-167">String</span><span class="sxs-lookup"><span data-stu-id="499d9-167">String</span></span>| <span data-ttu-id="499d9-168">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="499d9-168">Highest grade taught.</span></span> |
|<span data-ttu-id="499d9-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="499d9-169">lowestGrade</span></span>|<span data-ttu-id="499d9-170">String</span><span class="sxs-lookup"><span data-stu-id="499d9-170">String</span></span>| <span data-ttu-id="499d9-171">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="499d9-171">Lowest grade taught.</span></span> |
|<span data-ttu-id="499d9-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="499d9-172">schoolNumber</span></span>|<span data-ttu-id="499d9-173">String</span><span class="sxs-lookup"><span data-stu-id="499d9-173">String</span></span>| <span data-ttu-id="499d9-174">学校番号。</span><span class="sxs-lookup"><span data-stu-id="499d9-174">School Number.</span></span>|
|<span data-ttu-id="499d9-175">externalId</span><span class="sxs-lookup"><span data-stu-id="499d9-175">externalId</span></span>|<span data-ttu-id="499d9-176">String</span><span class="sxs-lookup"><span data-stu-id="499d9-176">String</span></span>| <span data-ttu-id="499d9-177">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="499d9-177">ID of school in syncing system.</span></span> |
|<span data-ttu-id="499d9-178">phone</span><span class="sxs-lookup"><span data-stu-id="499d9-178">phone</span></span>|<span data-ttu-id="499d9-179">String</span><span class="sxs-lookup"><span data-stu-id="499d9-179">String</span></span>| <span data-ttu-id="499d9-180">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="499d9-180">Phone number of school.</span></span> |
|<span data-ttu-id="499d9-181">fax</span><span class="sxs-lookup"><span data-stu-id="499d9-181">fax</span></span>|<span data-ttu-id="499d9-182">String</span><span class="sxs-lookup"><span data-stu-id="499d9-182">String</span></span>| <span data-ttu-id="499d9-183">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="499d9-183">Fax number of school.</span></span> |
|<span data-ttu-id="499d9-184">address</span><span class="sxs-lookup"><span data-stu-id="499d9-184">address</span></span>|[<span data-ttu-id="499d9-185">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="499d9-185">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="499d9-186">学校の住所。</span><span class="sxs-lookup"><span data-stu-id="499d9-186">Address of the school.</span></span>|
|<span data-ttu-id="499d9-187">createdBy</span><span class="sxs-lookup"><span data-stu-id="499d9-187">createdBy</span></span>|[<span data-ttu-id="499d9-188">identitySet</span><span class="sxs-lookup"><span data-stu-id="499d9-188">identitySet</span></span>](identityset.md)|<span data-ttu-id="499d9-189">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="499d9-189">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="499d9-190">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="499d9-190">Relationships</span></span>
| <span data-ttu-id="499d9-191">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="499d9-191">Relationship</span></span> | <span data-ttu-id="499d9-192">型</span><span class="sxs-lookup"><span data-stu-id="499d9-192">Type</span></span>   |<span data-ttu-id="499d9-193">説明</span><span class="sxs-lookup"><span data-stu-id="499d9-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="499d9-194">classes</span><span class="sxs-lookup"><span data-stu-id="499d9-194">classes</span></span>|<span data-ttu-id="499d9-195">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="499d9-195">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="499d9-196">学校で授業しているクラス。</span><span class="sxs-lookup"><span data-stu-id="499d9-196">Classes taught at the school.</span></span> <span data-ttu-id="499d9-197">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="499d9-197">Nullable.</span></span>|
|<span data-ttu-id="499d9-198">users</span><span class="sxs-lookup"><span data-stu-id="499d9-198">users</span></span>|<span data-ttu-id="499d9-199">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="499d9-199">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="499d9-200">学校のユーザー。</span><span class="sxs-lookup"><span data-stu-id="499d9-200">Users in the school.</span></span> <span data-ttu-id="499d9-201">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="499d9-201">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="499d9-202">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="499d9-202">JSON representation</span></span>

<span data-ttu-id="499d9-203">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="499d9-203">The following is a JSON representation of the resource.</span></span>

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
