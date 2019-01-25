---
title: educationClass リソース タイプ
description: '学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5a4bbc0560f2a40b5a438ec8276bbcf984a22721
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526733"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="b37a3-106">educationClass リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="b37a3-106">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b37a3-107">学校内のクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-107">Represents a class within a school.</span></span> <span data-ttu-id="b37a3-108">**educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="b37a3-109">学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。</span><span class="sxs-lookup"><span data-stu-id="b37a3-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="b37a3-110">Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b37a3-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="b37a3-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="b37a3-111">Methods</span></span>

| <span data-ttu-id="b37a3-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="b37a3-112">Method</span></span>           | <span data-ttu-id="b37a3-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b37a3-113">Return Type</span></span>    |<span data-ttu-id="b37a3-114">説明</span><span class="sxs-lookup"><span data-stu-id="b37a3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b37a3-115">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="b37a3-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="b37a3-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="b37a3-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="b37a3-117">**educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b37a3-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="b37a3-118">Add member</span><span class="sxs-lookup"><span data-stu-id="b37a3-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="b37a3-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="b37a3-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b37a3-120">members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="b37a3-121">List members</span><span class="sxs-lookup"><span data-stu-id="b37a3-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="b37a3-122">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b37a3-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="b37a3-123">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="b37a3-124">Remove student</span><span class="sxs-lookup"><span data-stu-id="b37a3-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="b37a3-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="b37a3-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b37a3-126">members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="b37a3-127">List schools</span><span class="sxs-lookup"><span data-stu-id="b37a3-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="b37a3-128">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b37a3-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="b37a3-129">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="b37a3-130">Add teacher</span><span class="sxs-lookup"><span data-stu-id="b37a3-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="b37a3-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="b37a3-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b37a3-132">teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="b37a3-133">List teachers</span><span class="sxs-lookup"><span data-stu-id="b37a3-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="b37a3-134">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b37a3-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="b37a3-135">クラスの教師一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="b37a3-136">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="b37a3-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="b37a3-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="b37a3-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b37a3-138">teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="b37a3-139">EducationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-139">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="b37a3-140">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="b37a3-140">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="b37a3-141">割り当てのコレクションへの投稿には、新しい**educationAssignment**を作成します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-141">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="b37a3-142">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="b37a3-142">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="b37a3-143">[educationAssignment](../resources/educationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b37a3-143">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="b37a3-144">**EducationAssignment**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-144">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="b37a3-145">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="b37a3-145">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="b37a3-146">group</span><span class="sxs-lookup"><span data-stu-id="b37a3-146">group</span></span>](group.md)| <span data-ttu-id="b37a3-147">この **educationClass** に対応する Office 365 **group**を取得します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-147">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="b37a3-148">Update</span><span class="sxs-lookup"><span data-stu-id="b37a3-148">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="b37a3-149">educationClass</span><span class="sxs-lookup"><span data-stu-id="b37a3-149">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="b37a3-150">**educationClass** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-150">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="b37a3-151">Delete</span><span class="sxs-lookup"><span data-stu-id="b37a3-151">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="b37a3-152">なし</span><span class="sxs-lookup"><span data-stu-id="b37a3-152">None</span></span> |<span data-ttu-id="b37a3-153">**educationClass** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-153">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b37a3-154">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b37a3-154">Properties</span></span>
| <span data-ttu-id="b37a3-155">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b37a3-155">Property</span></span>     | <span data-ttu-id="b37a3-156">型</span><span class="sxs-lookup"><span data-stu-id="b37a3-156">Type</span></span>   |<span data-ttu-id="b37a3-157">説明</span><span class="sxs-lookup"><span data-stu-id="b37a3-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b37a3-158">id</span><span class="sxs-lookup"><span data-stu-id="b37a3-158">id</span></span>| <span data-ttu-id="b37a3-159">文字列</span><span class="sxs-lookup"><span data-stu-id="b37a3-159">String</span></span>| <span data-ttu-id="b37a3-160">クラスの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b37a3-160">Unique identifier for the class.</span></span>|
|<span data-ttu-id="b37a3-161">説明</span><span class="sxs-lookup"><span data-stu-id="b37a3-161">description</span></span>|<span data-ttu-id="b37a3-162">文字列</span><span class="sxs-lookup"><span data-stu-id="b37a3-162">String</span></span>| <span data-ttu-id="b37a3-163">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="b37a3-163">Description of the class.</span></span>|
|<span data-ttu-id="b37a3-164">displayName</span><span class="sxs-lookup"><span data-stu-id="b37a3-164">displayName</span></span>|<span data-ttu-id="b37a3-165">String</span><span class="sxs-lookup"><span data-stu-id="b37a3-165">String</span></span>| <span data-ttu-id="b37a3-166">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="b37a3-166">Name of the class.</span></span>|
|<span data-ttu-id="b37a3-167">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b37a3-167">mailNickname</span></span>|<span data-ttu-id="b37a3-168">String</span><span class="sxs-lookup"><span data-stu-id="b37a3-168">String</span></span>| <span data-ttu-id="b37a3-169">すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。</span><span class="sxs-lookup"><span data-stu-id="b37a3-169">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="b37a3-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="b37a3-170">createdBy</span></span>|[<span data-ttu-id="b37a3-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="b37a3-171">identitySet</span></span>](identityset.md)| <span data-ttu-id="b37a3-172">クラスを作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="b37a3-172">Entity who created the class</span></span> |
|<span data-ttu-id="b37a3-173">classCode</span><span class="sxs-lookup"><span data-stu-id="b37a3-173">classCode</span></span>|<span data-ttu-id="b37a3-174">String</span><span class="sxs-lookup"><span data-stu-id="b37a3-174">String</span></span>| <span data-ttu-id="b37a3-175">クラスを識別するために学校が使用するクラス コード。</span><span class="sxs-lookup"><span data-stu-id="b37a3-175">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="b37a3-176">externalId</span><span class="sxs-lookup"><span data-stu-id="b37a3-176">externalId</span></span>|<span data-ttu-id="b37a3-177">String</span><span class="sxs-lookup"><span data-stu-id="b37a3-177">String</span></span>| <span data-ttu-id="b37a3-178">同期システムからのクラスの ID。</span><span class="sxs-lookup"><span data-stu-id="b37a3-178">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="b37a3-179">externalName</span><span class="sxs-lookup"><span data-stu-id="b37a3-179">externalName</span></span>|<span data-ttu-id="b37a3-180">String</span><span class="sxs-lookup"><span data-stu-id="b37a3-180">String</span></span>|<span data-ttu-id="b37a3-181">同期システムからのクラスの名前。</span><span class="sxs-lookup"><span data-stu-id="b37a3-181">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="b37a3-182">externalSource</span><span class="sxs-lookup"><span data-stu-id="b37a3-182">externalSource</span></span>|<span data-ttu-id="b37a3-183">string</span><span class="sxs-lookup"><span data-stu-id="b37a3-183">string</span></span>| <span data-ttu-id="b37a3-184">このクラスの作成方法。</span><span class="sxs-lookup"><span data-stu-id="b37a3-184">How this class was created.</span></span> <span data-ttu-id="b37a3-185">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b37a3-185">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b37a3-186">term</span><span class="sxs-lookup"><span data-stu-id="b37a3-186">term</span></span>|[<span data-ttu-id="b37a3-187">educationTerm</span><span class="sxs-lookup"><span data-stu-id="b37a3-187">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="b37a3-188">このクラスの学期。</span><span class="sxs-lookup"><span data-stu-id="b37a3-188">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b37a3-189">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b37a3-189">Relationships</span></span>
| <span data-ttu-id="b37a3-190">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b37a3-190">Relationship</span></span> | <span data-ttu-id="b37a3-191">型</span><span class="sxs-lookup"><span data-stu-id="b37a3-191">Type</span></span>   |<span data-ttu-id="b37a3-192">説明</span><span class="sxs-lookup"><span data-stu-id="b37a3-192">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b37a3-193">members</span><span class="sxs-lookup"><span data-stu-id="b37a3-193">members</span></span>|<span data-ttu-id="b37a3-194">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b37a3-194">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="b37a3-195">クラスのすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="b37a3-195">All users in the class.</span></span> <span data-ttu-id="b37a3-196">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b37a3-196">Nullable.</span></span>|
|<span data-ttu-id="b37a3-197">schools</span><span class="sxs-lookup"><span data-stu-id="b37a3-197">schools</span></span>|<span data-ttu-id="b37a3-198">[educationSchool](../resources/educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b37a3-198">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="b37a3-199">このクラスに関連付けられているすべての学校。</span><span class="sxs-lookup"><span data-stu-id="b37a3-199">All schools that this class is associated with.</span></span> <span data-ttu-id="b37a3-200">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b37a3-200">Nullable.</span></span>|
|<span data-ttu-id="b37a3-201">teachers</span><span class="sxs-lookup"><span data-stu-id="b37a3-201">teachers</span></span>|<span data-ttu-id="b37a3-202">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b37a3-202">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="b37a3-203">このクラスのすべての教師。</span><span class="sxs-lookup"><span data-stu-id="b37a3-203">All teachers in the class.</span></span> <span data-ttu-id="b37a3-204">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b37a3-204">Nullable.</span></span>|
|<span data-ttu-id="b37a3-205">assignments</span><span class="sxs-lookup"><span data-stu-id="b37a3-205">assignments</span></span>|<span data-ttu-id="b37a3-206">[educationAssignment](../resources/educationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b37a3-206">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="b37a3-207">このクラスに関連付けられているすべての割り当て。</span><span class="sxs-lookup"><span data-stu-id="b37a3-207">All assignments associated with this class.</span></span> <span data-ttu-id="b37a3-208">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b37a3-208">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b37a3-209">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b37a3-209">JSON representation</span></span>

<span data-ttu-id="b37a3-210">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b37a3-210">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationclass.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
