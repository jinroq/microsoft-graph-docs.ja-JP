---
title: educationSchool リソースの種類
description: '学校。 **educationSchool**リソースは現在、administrativeUnit リソースに対応しており、同じ ID を共有しています。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542943"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="74982-104">educationSchool リソースの種類</span><span class="sxs-lookup"><span data-stu-id="74982-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74982-105">学校。</span><span class="sxs-lookup"><span data-stu-id="74982-105">A school.</span></span> <span data-ttu-id="74982-106">**educationSchool**リソースは現在、 [administrativeUnit](administrativeunit.md)リソースに対応しており、同じ ID を共有しています。</span><span class="sxs-lookup"><span data-stu-id="74982-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="74982-107">このリソースは[educationOrganization](educationorganization.md)のサブタイプです。</span><span class="sxs-lookup"><span data-stu-id="74982-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="74982-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="74982-108">Methods</span></span>

| <span data-ttu-id="74982-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="74982-109">Method</span></span>           | <span data-ttu-id="74982-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="74982-110">Return Type</span></span>    |<span data-ttu-id="74982-111">説明</span><span class="sxs-lookup"><span data-stu-id="74982-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74982-112">Get</span><span class="sxs-lookup"><span data-stu-id="74982-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="74982-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="74982-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="74982-114">**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="74982-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="74982-115">Add class</span><span class="sxs-lookup"><span data-stu-id="74982-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="74982-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="74982-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="74982-117">classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。</span><span class="sxs-lookup"><span data-stu-id="74982-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="74982-118">List classes</span><span class="sxs-lookup"><span data-stu-id="74982-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="74982-119">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="74982-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="74982-120">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="74982-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="74982-121">Remove class</span><span class="sxs-lookup"><span data-stu-id="74982-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="74982-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="74982-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="74982-123">classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。</span><span class="sxs-lookup"><span data-stu-id="74982-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="74982-124">Add user</span><span class="sxs-lookup"><span data-stu-id="74982-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="74982-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="74982-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="74982-126">**users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="74982-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="74982-127">List users</span><span class="sxs-lookup"><span data-stu-id="74982-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="74982-128">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="74982-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="74982-129">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="74982-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="74982-130">Remove user</span><span class="sxs-lookup"><span data-stu-id="74982-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="74982-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="74982-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="74982-132">**users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="74982-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="74982-133">administrativeUnit を取得する</span><span class="sxs-lookup"><span data-stu-id="74982-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="74982-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="74982-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="74982-135">この**educationSchool**に対応する**administrativeUnit**を取得します。</span><span class="sxs-lookup"><span data-stu-id="74982-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="74982-136">Update</span><span class="sxs-lookup"><span data-stu-id="74982-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="74982-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="74982-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="74982-138">**educationSchool** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="74982-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="74982-139">削除</span><span class="sxs-lookup"><span data-stu-id="74982-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="74982-140">なし</span><span class="sxs-lookup"><span data-stu-id="74982-140">None</span></span> |<span data-ttu-id="74982-141">**educationSchool** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="74982-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="74982-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74982-142">Properties</span></span>
| <span data-ttu-id="74982-143">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74982-143">Property</span></span>     | <span data-ttu-id="74982-144">型</span><span class="sxs-lookup"><span data-stu-id="74982-144">Type</span></span>   |<span data-ttu-id="74982-145">説明</span><span class="sxs-lookup"><span data-stu-id="74982-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74982-146">id</span><span class="sxs-lookup"><span data-stu-id="74982-146">id</span></span>|<span data-ttu-id="74982-147">String</span><span class="sxs-lookup"><span data-stu-id="74982-147">String</span></span>|<span data-ttu-id="74982-148">この学校の GUID。</span><span class="sxs-lookup"><span data-stu-id="74982-148">GUID of this school.</span></span>|
|<span data-ttu-id="74982-149">displayName</span><span class="sxs-lookup"><span data-stu-id="74982-149">displayName</span></span>| <span data-ttu-id="74982-150">文字列</span><span class="sxs-lookup"><span data-stu-id="74982-150">String</span></span>| <span data-ttu-id="74982-151">学校の表示名。</span><span class="sxs-lookup"><span data-stu-id="74982-151">Display name of the school.</span></span>| 
|<span data-ttu-id="74982-152">description</span><span class="sxs-lookup"><span data-stu-id="74982-152">description</span></span>| <span data-ttu-id="74982-153">String</span><span class="sxs-lookup"><span data-stu-id="74982-153">String</span></span> | <span data-ttu-id="74982-154">学校の説明。</span><span class="sxs-lookup"><span data-stu-id="74982-154">Description of the school.</span></span>| 
|<span data-ttu-id="74982-155">status</span><span class="sxs-lookup"><span data-stu-id="74982-155">status</span></span>| <span data-ttu-id="74982-156">string</span><span class="sxs-lookup"><span data-stu-id="74982-156">string</span></span>| <span data-ttu-id="74982-157">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="74982-157">Read-Only.</span></span> <span data-ttu-id="74982-158">使用可能な値: `inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="74982-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="74982-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="74982-159">externalSource</span></span>| <span data-ttu-id="74982-160">string</span><span class="sxs-lookup"><span data-stu-id="74982-160">string</span></span>| <span data-ttu-id="74982-161">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="74982-161">Read-Only.</span></span>  <span data-ttu-id="74982-162">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="74982-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="74982-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="74982-163">principalEmail</span></span>| <span data-ttu-id="74982-164">String</span><span class="sxs-lookup"><span data-stu-id="74982-164">String</span></span>| <span data-ttu-id="74982-165">プリンシパルの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="74982-165">Email address of the principal.</span></span>|
|<span data-ttu-id="74982-166">principalName</span><span class="sxs-lookup"><span data-stu-id="74982-166">principalName</span></span>| <span data-ttu-id="74982-167">String</span><span class="sxs-lookup"><span data-stu-id="74982-167">String</span></span> | <span data-ttu-id="74982-168">プリンシパルの名前。</span><span class="sxs-lookup"><span data-stu-id="74982-168">Name of the principal.</span></span>|
|<span data-ttu-id="74982-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="74982-169">externalPrincipalId</span></span>| <span data-ttu-id="74982-170">String</span><span class="sxs-lookup"><span data-stu-id="74982-170">String</span></span> | <span data-ttu-id="74982-171">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="74982-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="74982-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="74982-172">highestGrade</span></span>|<span data-ttu-id="74982-173">String</span><span class="sxs-lookup"><span data-stu-id="74982-173">String</span></span>| <span data-ttu-id="74982-174">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="74982-174">Highest grade taught.</span></span> |
|<span data-ttu-id="74982-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="74982-175">lowestGrade</span></span>|<span data-ttu-id="74982-176">String</span><span class="sxs-lookup"><span data-stu-id="74982-176">String</span></span>| <span data-ttu-id="74982-177">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="74982-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="74982-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="74982-178">schoolNumber</span></span>|<span data-ttu-id="74982-179">String</span><span class="sxs-lookup"><span data-stu-id="74982-179">String</span></span>| <span data-ttu-id="74982-180">学校番号。</span><span class="sxs-lookup"><span data-stu-id="74982-180">School Number.</span></span>|
|<span data-ttu-id="74982-181">externalId</span><span class="sxs-lookup"><span data-stu-id="74982-181">externalId</span></span>|<span data-ttu-id="74982-182">String</span><span class="sxs-lookup"><span data-stu-id="74982-182">String</span></span>| <span data-ttu-id="74982-183">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="74982-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="74982-184">phone</span><span class="sxs-lookup"><span data-stu-id="74982-184">phone</span></span>|<span data-ttu-id="74982-185">String</span><span class="sxs-lookup"><span data-stu-id="74982-185">String</span></span>| <span data-ttu-id="74982-186">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="74982-186">Phone number of school.</span></span> |
|<span data-ttu-id="74982-187">fax</span><span class="sxs-lookup"><span data-stu-id="74982-187">fax</span></span>|<span data-ttu-id="74982-188">String</span><span class="sxs-lookup"><span data-stu-id="74982-188">String</span></span>| <span data-ttu-id="74982-189">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="74982-189">Fax number of school.</span></span> |
|<span data-ttu-id="74982-190">address</span><span class="sxs-lookup"><span data-stu-id="74982-190">address</span></span>|[<span data-ttu-id="74982-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="74982-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="74982-192">学校の住所。</span><span class="sxs-lookup"><span data-stu-id="74982-192">Address of the school.</span></span>|
|<span data-ttu-id="74982-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="74982-193">createdBy</span></span>|[<span data-ttu-id="74982-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="74982-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="74982-195">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="74982-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="74982-196">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="74982-196">Relationships</span></span>
| <span data-ttu-id="74982-197">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="74982-197">Relationship</span></span> | <span data-ttu-id="74982-198">型</span><span class="sxs-lookup"><span data-stu-id="74982-198">Type</span></span>   |<span data-ttu-id="74982-199">説明</span><span class="sxs-lookup"><span data-stu-id="74982-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74982-200">classes</span><span class="sxs-lookup"><span data-stu-id="74982-200">classes</span></span>|<span data-ttu-id="74982-201">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="74982-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="74982-202">学校で授業しているクラス。</span><span class="sxs-lookup"><span data-stu-id="74982-202">Classes taught at the school.</span></span> <span data-ttu-id="74982-203">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="74982-203">Nullable.</span></span>|
|<span data-ttu-id="74982-204">users</span><span class="sxs-lookup"><span data-stu-id="74982-204">users</span></span>|<span data-ttu-id="74982-205">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="74982-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="74982-206">学校のユーザー。</span><span class="sxs-lookup"><span data-stu-id="74982-206">Users in the school.</span></span> <span data-ttu-id="74982-207">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="74982-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74982-208">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74982-208">JSON representation</span></span>

<span data-ttu-id="74982-209">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74982-209">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationschool.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
