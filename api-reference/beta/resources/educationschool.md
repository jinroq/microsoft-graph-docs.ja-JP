---
title: educationSchool リソースの種類
description: '学校。 現時点で、**educationSchool** リソースは administrativeUnit リソースと一致していて、同じ ID を共有しています。  '
localization_priority: Normal
ms.openlocfilehash: 20eacb87b68cbf490131b98a15d3ab3239d73478
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830451"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="2b17e-104">educationSchool リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b17e-104">educationSchool resource type</span></span>

> <span data-ttu-id="2b17e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b17e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b17e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b17e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b17e-107">学校。</span><span class="sxs-lookup"><span data-stu-id="2b17e-107">A school.</span></span> <span data-ttu-id="2b17e-108">現時点で、**educationSchool** リソースは [administrativeUnit](administrativeunit.md) リソースと一致していて、同じ ID を共有しています。</span><span class="sxs-lookup"><span data-stu-id="2b17e-108">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="2b17e-109">このリソースは、[educationOrganization](educationorganization.md) のサブタイプです。</span><span class="sxs-lookup"><span data-stu-id="2b17e-109">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="2b17e-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b17e-110">Methods</span></span>

| <span data-ttu-id="2b17e-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b17e-111">Method</span></span>           | <span data-ttu-id="2b17e-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2b17e-112">Return Type</span></span>    |<span data-ttu-id="2b17e-113">説明</span><span class="sxs-lookup"><span data-stu-id="2b17e-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b17e-114">Get</span><span class="sxs-lookup"><span data-stu-id="2b17e-114">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="2b17e-115">educationSchool</span><span class="sxs-lookup"><span data-stu-id="2b17e-115">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="2b17e-116">**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2b17e-116">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="2b17e-117">Add class</span><span class="sxs-lookup"><span data-stu-id="2b17e-117">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="2b17e-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="2b17e-118">educationClass</span></span>](educationclass.md)| <span data-ttu-id="2b17e-119">classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-119">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="2b17e-120">List classes</span><span class="sxs-lookup"><span data-stu-id="2b17e-120">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="2b17e-121">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2b17e-121">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="2b17e-122">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-122">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="2b17e-123">Remove class</span><span class="sxs-lookup"><span data-stu-id="2b17e-123">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="2b17e-124">educationClass</span><span class="sxs-lookup"><span data-stu-id="2b17e-124">educationClass</span></span>](educationclass.md)| <span data-ttu-id="2b17e-125">classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-125">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="2b17e-126">Add user</span><span class="sxs-lookup"><span data-stu-id="2b17e-126">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="2b17e-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="2b17e-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="2b17e-128">**users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-128">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="2b17e-129">List users</span><span class="sxs-lookup"><span data-stu-id="2b17e-129">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="2b17e-130">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2b17e-130">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="2b17e-131">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-131">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="2b17e-132">Remove user</span><span class="sxs-lookup"><span data-stu-id="2b17e-132">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="2b17e-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="2b17e-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="2b17e-134">**users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-134">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="2b17e-135">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2b17e-135">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="2b17e-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2b17e-136">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="2b17e-137">この **educationSchool** に対応する **administrativeUnit** を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-137">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="2b17e-138">Update</span><span class="sxs-lookup"><span data-stu-id="2b17e-138">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="2b17e-139">educationSchool</span><span class="sxs-lookup"><span data-stu-id="2b17e-139">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="2b17e-140">**educationSchool** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-140">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="2b17e-141">Delete</span><span class="sxs-lookup"><span data-stu-id="2b17e-141">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="2b17e-142">なし</span><span class="sxs-lookup"><span data-stu-id="2b17e-142">None</span></span> |<span data-ttu-id="2b17e-143">**educationSchool** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-143">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2b17e-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b17e-144">Properties</span></span>
| <span data-ttu-id="2b17e-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b17e-145">Property</span></span>     | <span data-ttu-id="2b17e-146">種類</span><span class="sxs-lookup"><span data-stu-id="2b17e-146">Type</span></span>   |<span data-ttu-id="2b17e-147">説明</span><span class="sxs-lookup"><span data-stu-id="2b17e-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b17e-148">ID</span><span class="sxs-lookup"><span data-stu-id="2b17e-148">id</span></span>|<span data-ttu-id="2b17e-149">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-149">String</span></span>|<span data-ttu-id="2b17e-150">この学校の GUID。</span><span class="sxs-lookup"><span data-stu-id="2b17e-150">GUID of this school.</span></span>|
|<span data-ttu-id="2b17e-151">displayName</span><span class="sxs-lookup"><span data-stu-id="2b17e-151">displayName</span></span>| <span data-ttu-id="2b17e-152">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-152">String</span></span>| <span data-ttu-id="2b17e-153">学校の表示名。</span><span class="sxs-lookup"><span data-stu-id="2b17e-153">Display name of the school.</span></span>| 
|<span data-ttu-id="2b17e-154">説明</span><span class="sxs-lookup"><span data-stu-id="2b17e-154">description</span></span>| <span data-ttu-id="2b17e-155">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-155">String</span></span> | <span data-ttu-id="2b17e-156">学校の説明。</span><span class="sxs-lookup"><span data-stu-id="2b17e-156">Description of the school.</span></span>| 
|<span data-ttu-id="2b17e-157">status</span><span class="sxs-lookup"><span data-stu-id="2b17e-157">status</span></span>| <span data-ttu-id="2b17e-158">文字列</span><span class="sxs-lookup"><span data-stu-id="2b17e-158">string</span></span>| <span data-ttu-id="2b17e-159">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="2b17e-159">Read-Only.</span></span> <span data-ttu-id="2b17e-160">使用可能な値: `inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="2b17e-160">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="2b17e-161">externalSource</span><span class="sxs-lookup"><span data-stu-id="2b17e-161">externalSource</span></span>| <span data-ttu-id="2b17e-162">文字列</span><span class="sxs-lookup"><span data-stu-id="2b17e-162">string</span></span>| <span data-ttu-id="2b17e-163">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="2b17e-163">Read-Only.</span></span>  <span data-ttu-id="2b17e-164">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2b17e-164">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2b17e-165">principalEmail</span><span class="sxs-lookup"><span data-stu-id="2b17e-165">principalEmail</span></span>| <span data-ttu-id="2b17e-166">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-166">String</span></span>| <span data-ttu-id="2b17e-167">プリンシパルの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="2b17e-167">Email address of the principal.</span></span>|
|<span data-ttu-id="2b17e-168">principalName</span><span class="sxs-lookup"><span data-stu-id="2b17e-168">principalName</span></span>| <span data-ttu-id="2b17e-169">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-169">String</span></span> | <span data-ttu-id="2b17e-170">プリンシパルの名前。</span><span class="sxs-lookup"><span data-stu-id="2b17e-170">Name of the principal.</span></span>|
|<span data-ttu-id="2b17e-171">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="2b17e-171">externalPrincipalId</span></span>| <span data-ttu-id="2b17e-172">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-172">String</span></span> | <span data-ttu-id="2b17e-173">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="2b17e-173">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="2b17e-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="2b17e-174">highestGrade</span></span>|<span data-ttu-id="2b17e-175">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-175">String</span></span>| <span data-ttu-id="2b17e-176">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="2b17e-176">Highest grade taught.</span></span> |
|<span data-ttu-id="2b17e-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="2b17e-177">lowestGrade</span></span>|<span data-ttu-id="2b17e-178">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-178">String</span></span>| <span data-ttu-id="2b17e-179">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="2b17e-179">Lowest grade taught.</span></span> |
|<span data-ttu-id="2b17e-180">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="2b17e-180">schoolNumber</span></span>|<span data-ttu-id="2b17e-181">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-181">String</span></span>| <span data-ttu-id="2b17e-182">学校番号。</span><span class="sxs-lookup"><span data-stu-id="2b17e-182">School Number.</span></span>|
|<span data-ttu-id="2b17e-183">externalId</span><span class="sxs-lookup"><span data-stu-id="2b17e-183">externalId</span></span>|<span data-ttu-id="2b17e-184">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-184">String</span></span>| <span data-ttu-id="2b17e-185">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="2b17e-185">ID of school in syncing system.</span></span> |
|<span data-ttu-id="2b17e-186">phone</span><span class="sxs-lookup"><span data-stu-id="2b17e-186">phone</span></span>|<span data-ttu-id="2b17e-187">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-187">String</span></span>| <span data-ttu-id="2b17e-188">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="2b17e-188">Phone number of school.</span></span> |
|<span data-ttu-id="2b17e-189">fax</span><span class="sxs-lookup"><span data-stu-id="2b17e-189">fax</span></span>|<span data-ttu-id="2b17e-190">String</span><span class="sxs-lookup"><span data-stu-id="2b17e-190">String</span></span>| <span data-ttu-id="2b17e-191">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="2b17e-191">Fax number of school.</span></span> |
|<span data-ttu-id="2b17e-192">address</span><span class="sxs-lookup"><span data-stu-id="2b17e-192">address</span></span>|[<span data-ttu-id="2b17e-193">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2b17e-193">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="2b17e-194">学校の住所。</span><span class="sxs-lookup"><span data-stu-id="2b17e-194">Address of the school.</span></span>|
|<span data-ttu-id="2b17e-195">createdBy</span><span class="sxs-lookup"><span data-stu-id="2b17e-195">createdBy</span></span>|[<span data-ttu-id="2b17e-196">identitySet</span><span class="sxs-lookup"><span data-stu-id="2b17e-196">identitySet</span></span>](identityset.md)|<span data-ttu-id="2b17e-197">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="2b17e-197">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2b17e-198">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b17e-198">Relationships</span></span>
| <span data-ttu-id="2b17e-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b17e-199">Relationship</span></span> | <span data-ttu-id="2b17e-200">型</span><span class="sxs-lookup"><span data-stu-id="2b17e-200">Type</span></span>   |<span data-ttu-id="2b17e-201">説明</span><span class="sxs-lookup"><span data-stu-id="2b17e-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b17e-202">classes</span><span class="sxs-lookup"><span data-stu-id="2b17e-202">classes</span></span>|<span data-ttu-id="2b17e-203">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2b17e-203">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="2b17e-204">学校で授業しているクラス。</span><span class="sxs-lookup"><span data-stu-id="2b17e-204">Classes taught at the school.</span></span> <span data-ttu-id="2b17e-205">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2b17e-205">Nullable.</span></span>|
|<span data-ttu-id="2b17e-206">users</span><span class="sxs-lookup"><span data-stu-id="2b17e-206">users</span></span>|<span data-ttu-id="2b17e-207">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2b17e-207">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="2b17e-208">学校のユーザー。</span><span class="sxs-lookup"><span data-stu-id="2b17e-208">Users in the school.</span></span> <span data-ttu-id="2b17e-209">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2b17e-209">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b17e-210">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b17e-210">JSON representation</span></span>

<span data-ttu-id="2b17e-211">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b17e-211">The following is a JSON representation of the resource.</span></span>

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
