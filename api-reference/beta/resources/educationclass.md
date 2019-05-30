---
title: educationClass リソース タイプ
description: '学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: dfce83c99ec886a01c2c52c3bae58c91b12fa0b0
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536171"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="625f8-106">educationClass リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="625f8-106">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="625f8-107">学校内のクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="625f8-107">Represents a class within a school.</span></span> <span data-ttu-id="625f8-108">**educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。</span><span class="sxs-lookup"><span data-stu-id="625f8-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="625f8-109">学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。</span><span class="sxs-lookup"><span data-stu-id="625f8-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="625f8-110">Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="625f8-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="625f8-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="625f8-111">Methods</span></span>

| <span data-ttu-id="625f8-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="625f8-112">Method</span></span>           | <span data-ttu-id="625f8-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="625f8-113">Return Type</span></span>    |<span data-ttu-id="625f8-114">説明</span><span class="sxs-lookup"><span data-stu-id="625f8-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="625f8-115">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="625f8-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="625f8-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="625f8-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="625f8-117">**educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="625f8-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="625f8-118">Add member</span><span class="sxs-lookup"><span data-stu-id="625f8-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="625f8-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="625f8-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="625f8-120">members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="625f8-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="625f8-121">List members</span><span class="sxs-lookup"><span data-stu-id="625f8-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="625f8-122">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="625f8-123">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="625f8-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="625f8-124">Remove student</span><span class="sxs-lookup"><span data-stu-id="625f8-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="625f8-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="625f8-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="625f8-126">members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="625f8-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="625f8-127">List schools</span><span class="sxs-lookup"><span data-stu-id="625f8-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="625f8-128">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="625f8-129">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="625f8-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="625f8-130">Add teacher</span><span class="sxs-lookup"><span data-stu-id="625f8-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="625f8-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="625f8-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="625f8-132">teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="625f8-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="625f8-133">List teachers</span><span class="sxs-lookup"><span data-stu-id="625f8-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="625f8-134">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="625f8-135">クラスの教師一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="625f8-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="625f8-136">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="625f8-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="625f8-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="625f8-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="625f8-138">teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="625f8-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="625f8-139">EducationAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="625f8-139">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="625f8-140">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="625f8-140">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="625f8-141">Assignments コレクションへの投稿によって新しい**educationAssignment**を作成します。</span><span class="sxs-lookup"><span data-stu-id="625f8-141">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="625f8-142">割り当てを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="625f8-142">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="625f8-143">[educationAssignment](../resources/educationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-143">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="625f8-144">**EducationAssignment**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="625f8-144">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="625f8-145">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="625f8-145">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="625f8-146">group</span><span class="sxs-lookup"><span data-stu-id="625f8-146">group</span></span>](group.md)| <span data-ttu-id="625f8-147">この **educationClass** に対応する Office 365 **group**を取得します。</span><span class="sxs-lookup"><span data-stu-id="625f8-147">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="625f8-148">EducationCategory を作成する</span><span class="sxs-lookup"><span data-stu-id="625f8-148">Create educationCategory</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="625f8-149">educationCategory</span><span class="sxs-lookup"><span data-stu-id="625f8-149">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="625f8-150">このクラスの新しい**educationCategory**を作成します。</span><span class="sxs-lookup"><span data-stu-id="625f8-150">Create a new **educationCategory** for this class.</span></span>|
|[<span data-ttu-id="625f8-151">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="625f8-151">List categories</span></span>](../api/educationclass-list-categories.md) | <span data-ttu-id="625f8-152">[educationCategory](educationcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-152">[educationCategory](educationcategory.md) collection</span></span> | <span data-ttu-id="625f8-153">このクラスに属する**educationCategory**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="625f8-153">Get a list of **educationCategory** objects belonging to this class.</span></span>|
|[<span data-ttu-id="625f8-154">Update</span><span class="sxs-lookup"><span data-stu-id="625f8-154">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="625f8-155">educationClass</span><span class="sxs-lookup"><span data-stu-id="625f8-155">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="625f8-156">**educationClass** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="625f8-156">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="625f8-157">Delete</span><span class="sxs-lookup"><span data-stu-id="625f8-157">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="625f8-158">None</span><span class="sxs-lookup"><span data-stu-id="625f8-158">None</span></span> |<span data-ttu-id="625f8-159">**educationClass** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="625f8-159">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="625f8-160">プロパティ</span><span class="sxs-lookup"><span data-stu-id="625f8-160">Properties</span></span>
| <span data-ttu-id="625f8-161">プロパティ</span><span class="sxs-lookup"><span data-stu-id="625f8-161">Property</span></span>     | <span data-ttu-id="625f8-162">型</span><span class="sxs-lookup"><span data-stu-id="625f8-162">Type</span></span>   |<span data-ttu-id="625f8-163">説明</span><span class="sxs-lookup"><span data-stu-id="625f8-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="625f8-164">id</span><span class="sxs-lookup"><span data-stu-id="625f8-164">id</span></span>| <span data-ttu-id="625f8-165">文字列</span><span class="sxs-lookup"><span data-stu-id="625f8-165">String</span></span>| <span data-ttu-id="625f8-166">クラスの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="625f8-166">Unique identifier for the class.</span></span>|
|<span data-ttu-id="625f8-167">description</span><span class="sxs-lookup"><span data-stu-id="625f8-167">description</span></span>|<span data-ttu-id="625f8-168">String</span><span class="sxs-lookup"><span data-stu-id="625f8-168">String</span></span>| <span data-ttu-id="625f8-169">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="625f8-169">Description of the class.</span></span>|
|<span data-ttu-id="625f8-170">displayName</span><span class="sxs-lookup"><span data-stu-id="625f8-170">displayName</span></span>|<span data-ttu-id="625f8-171">文字列</span><span class="sxs-lookup"><span data-stu-id="625f8-171">String</span></span>| <span data-ttu-id="625f8-172">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="625f8-172">Name of the class.</span></span>|
|<span data-ttu-id="625f8-173">mailNickname</span><span class="sxs-lookup"><span data-stu-id="625f8-173">mailNickname</span></span>|<span data-ttu-id="625f8-174">String</span><span class="sxs-lookup"><span data-stu-id="625f8-174">String</span></span>| <span data-ttu-id="625f8-175">すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。</span><span class="sxs-lookup"><span data-stu-id="625f8-175">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="625f8-176">createdBy</span><span class="sxs-lookup"><span data-stu-id="625f8-176">createdBy</span></span>|[<span data-ttu-id="625f8-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="625f8-177">identitySet</span></span>](identityset.md)| <span data-ttu-id="625f8-178">クラスを作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="625f8-178">Entity who created the class</span></span> |
|<span data-ttu-id="625f8-179">classCode</span><span class="sxs-lookup"><span data-stu-id="625f8-179">classCode</span></span>|<span data-ttu-id="625f8-180">String</span><span class="sxs-lookup"><span data-stu-id="625f8-180">String</span></span>| <span data-ttu-id="625f8-181">クラスを識別するために学校が使用するクラス コード。</span><span class="sxs-lookup"><span data-stu-id="625f8-181">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="625f8-182">externalId</span><span class="sxs-lookup"><span data-stu-id="625f8-182">externalId</span></span>|<span data-ttu-id="625f8-183">String</span><span class="sxs-lookup"><span data-stu-id="625f8-183">String</span></span>| <span data-ttu-id="625f8-184">同期システムからのクラスの ID。</span><span class="sxs-lookup"><span data-stu-id="625f8-184">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="625f8-185">externalName</span><span class="sxs-lookup"><span data-stu-id="625f8-185">externalName</span></span>|<span data-ttu-id="625f8-186">String</span><span class="sxs-lookup"><span data-stu-id="625f8-186">String</span></span>|<span data-ttu-id="625f8-187">同期システムからのクラスの名前。</span><span class="sxs-lookup"><span data-stu-id="625f8-187">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="625f8-188">externalSource</span><span class="sxs-lookup"><span data-stu-id="625f8-188">externalSource</span></span>|<span data-ttu-id="625f8-189">string</span><span class="sxs-lookup"><span data-stu-id="625f8-189">string</span></span>| <span data-ttu-id="625f8-190">このクラスの作成方法。</span><span class="sxs-lookup"><span data-stu-id="625f8-190">How this class was created.</span></span> <span data-ttu-id="625f8-191">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="625f8-191">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="625f8-192">term</span><span class="sxs-lookup"><span data-stu-id="625f8-192">term</span></span>|[<span data-ttu-id="625f8-193">educationTerm</span><span class="sxs-lookup"><span data-stu-id="625f8-193">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="625f8-194">このクラスの学期。</span><span class="sxs-lookup"><span data-stu-id="625f8-194">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="625f8-195">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="625f8-195">Relationships</span></span>
| <span data-ttu-id="625f8-196">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="625f8-196">Relationship</span></span> | <span data-ttu-id="625f8-197">型</span><span class="sxs-lookup"><span data-stu-id="625f8-197">Type</span></span>   |<span data-ttu-id="625f8-198">説明</span><span class="sxs-lookup"><span data-stu-id="625f8-198">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="625f8-199">members</span><span class="sxs-lookup"><span data-stu-id="625f8-199">members</span></span>|<span data-ttu-id="625f8-200">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-200">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="625f8-201">クラスのすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="625f8-201">All users in the class.</span></span> <span data-ttu-id="625f8-202">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="625f8-202">Nullable.</span></span>|
|<span data-ttu-id="625f8-203">schools</span><span class="sxs-lookup"><span data-stu-id="625f8-203">schools</span></span>|<span data-ttu-id="625f8-204">[educationSchool](../resources/educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-204">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="625f8-205">このクラスに関連付けられているすべての学校。</span><span class="sxs-lookup"><span data-stu-id="625f8-205">All schools that this class is associated with.</span></span> <span data-ttu-id="625f8-206">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="625f8-206">Nullable.</span></span>|
|<span data-ttu-id="625f8-207">teachers</span><span class="sxs-lookup"><span data-stu-id="625f8-207">teachers</span></span>|<span data-ttu-id="625f8-208">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-208">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="625f8-209">このクラスのすべての教師。</span><span class="sxs-lookup"><span data-stu-id="625f8-209">All teachers in the class.</span></span> <span data-ttu-id="625f8-210">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="625f8-210">Nullable.</span></span>|
|<span data-ttu-id="625f8-211">assignments</span><span class="sxs-lookup"><span data-stu-id="625f8-211">assignments</span></span>|<span data-ttu-id="625f8-212">[educationAssignment](../resources/educationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-212">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="625f8-213">このクラスに関連付けられているすべての割り当て。</span><span class="sxs-lookup"><span data-stu-id="625f8-213">All assignments associated with this class.</span></span> <span data-ttu-id="625f8-214">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="625f8-214">Nullable.</span></span>|
|<span data-ttu-id="625f8-215">categories</span><span class="sxs-lookup"><span data-stu-id="625f8-215">categories</span></span>|<span data-ttu-id="625f8-216">[educationCategory](../resources/educationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="625f8-216">[educationCategory](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="625f8-217">このクラスに関連付けられているすべてのカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="625f8-217">All categories associated with this class.</span></span> <span data-ttu-id="625f8-218">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="625f8-218">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="625f8-219">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="625f8-219">JSON representation</span></span>

<span data-ttu-id="625f8-220">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="625f8-220">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "suppressions": []
}
-->
