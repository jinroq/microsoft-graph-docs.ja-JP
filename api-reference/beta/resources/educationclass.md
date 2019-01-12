---
title: educationClass リソース タイプ
description: '学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f651e695ddf0b7139a31d077dcf021fced91293a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962920"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="c2d86-106">educationClass リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c2d86-106">educationClass resource type</span></span>

> <span data-ttu-id="c2d86-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c2d86-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2d86-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2d86-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2d86-109">学校内のクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-109">Represents a class within a school.</span></span> <span data-ttu-id="c2d86-110">**educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-110">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="c2d86-111">学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。</span><span class="sxs-lookup"><span data-stu-id="c2d86-111">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="c2d86-112">Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c2d86-112">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="c2d86-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="c2d86-113">Methods</span></span>

| <span data-ttu-id="c2d86-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="c2d86-114">Method</span></span>           | <span data-ttu-id="c2d86-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c2d86-115">Return Type</span></span>    |<span data-ttu-id="c2d86-116">説明</span><span class="sxs-lookup"><span data-stu-id="c2d86-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2d86-117">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="c2d86-117">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="c2d86-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="c2d86-118">educationClass</span></span>](educationclass.md) |<span data-ttu-id="c2d86-119">**educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c2d86-119">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="c2d86-120">Add member</span><span class="sxs-lookup"><span data-stu-id="c2d86-120">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="c2d86-121">educationUser</span><span class="sxs-lookup"><span data-stu-id="c2d86-121">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c2d86-122">members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-122">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="c2d86-123">List members</span><span class="sxs-lookup"><span data-stu-id="c2d86-123">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="c2d86-124">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c2d86-124">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="c2d86-125">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-125">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="c2d86-126">Remove student</span><span class="sxs-lookup"><span data-stu-id="c2d86-126">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="c2d86-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="c2d86-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c2d86-128">members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-128">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="c2d86-129">List schools</span><span class="sxs-lookup"><span data-stu-id="c2d86-129">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="c2d86-130">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c2d86-130">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="c2d86-131">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-131">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="c2d86-132">Add teacher</span><span class="sxs-lookup"><span data-stu-id="c2d86-132">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="c2d86-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="c2d86-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c2d86-134">teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-134">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="c2d86-135">List teachers</span><span class="sxs-lookup"><span data-stu-id="c2d86-135">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="c2d86-136">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c2d86-136">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="c2d86-137">クラスの教師一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-137">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="c2d86-138">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="c2d86-138">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="c2d86-139">educationUser</span><span class="sxs-lookup"><span data-stu-id="c2d86-139">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c2d86-140">teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-140">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="c2d86-141">EducationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-141">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="c2d86-142">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2d86-142">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="c2d86-143">割り当てのコレクションへの投稿には、新しい**educationAssignment**を作成します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-143">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="c2d86-144">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="c2d86-144">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="c2d86-145">[educationAssignment](../resources/educationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c2d86-145">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="c2d86-146">**EducationAssignment**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-146">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="c2d86-147">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="c2d86-147">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="c2d86-148">group</span><span class="sxs-lookup"><span data-stu-id="c2d86-148">group</span></span>](group.md)| <span data-ttu-id="c2d86-149">この **educationClass** に対応する Office 365 **group**を取得します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-149">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="c2d86-150">Update</span><span class="sxs-lookup"><span data-stu-id="c2d86-150">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="c2d86-151">educationClass</span><span class="sxs-lookup"><span data-stu-id="c2d86-151">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="c2d86-152">**educationClass** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-152">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="c2d86-153">Delete</span><span class="sxs-lookup"><span data-stu-id="c2d86-153">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="c2d86-154">なし</span><span class="sxs-lookup"><span data-stu-id="c2d86-154">None</span></span> |<span data-ttu-id="c2d86-155">**educationClass** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-155">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c2d86-156">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2d86-156">Properties</span></span>
| <span data-ttu-id="c2d86-157">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2d86-157">Property</span></span>     | <span data-ttu-id="c2d86-158">種類</span><span class="sxs-lookup"><span data-stu-id="c2d86-158">Type</span></span>   |<span data-ttu-id="c2d86-159">説明</span><span class="sxs-lookup"><span data-stu-id="c2d86-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2d86-160">ID</span><span class="sxs-lookup"><span data-stu-id="c2d86-160">id</span></span>| <span data-ttu-id="c2d86-161">String</span><span class="sxs-lookup"><span data-stu-id="c2d86-161">String</span></span>| <span data-ttu-id="c2d86-162">クラスの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="c2d86-162">Unique identifier for the class.</span></span>|
|<span data-ttu-id="c2d86-163">説明</span><span class="sxs-lookup"><span data-stu-id="c2d86-163">description</span></span>|<span data-ttu-id="c2d86-164">String</span><span class="sxs-lookup"><span data-stu-id="c2d86-164">String</span></span>| <span data-ttu-id="c2d86-165">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="c2d86-165">Description of the class.</span></span>|
|<span data-ttu-id="c2d86-166">displayName</span><span class="sxs-lookup"><span data-stu-id="c2d86-166">displayName</span></span>|<span data-ttu-id="c2d86-167">String</span><span class="sxs-lookup"><span data-stu-id="c2d86-167">String</span></span>| <span data-ttu-id="c2d86-168">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="c2d86-168">Name of the class.</span></span>|
|<span data-ttu-id="c2d86-169">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c2d86-169">mailNickname</span></span>|<span data-ttu-id="c2d86-170">String</span><span class="sxs-lookup"><span data-stu-id="c2d86-170">String</span></span>| <span data-ttu-id="c2d86-171">すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。</span><span class="sxs-lookup"><span data-stu-id="c2d86-171">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="c2d86-172">createdBy</span><span class="sxs-lookup"><span data-stu-id="c2d86-172">createdBy</span></span>|[<span data-ttu-id="c2d86-173">identitySet</span><span class="sxs-lookup"><span data-stu-id="c2d86-173">identitySet</span></span>](identityset.md)| <span data-ttu-id="c2d86-174">クラスを作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="c2d86-174">Entity who created the class</span></span> |
|<span data-ttu-id="c2d86-175">classCode</span><span class="sxs-lookup"><span data-stu-id="c2d86-175">classCode</span></span>|<span data-ttu-id="c2d86-176">String</span><span class="sxs-lookup"><span data-stu-id="c2d86-176">String</span></span>| <span data-ttu-id="c2d86-177">クラスを識別するために学校が使用するクラス コード。</span><span class="sxs-lookup"><span data-stu-id="c2d86-177">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="c2d86-178">externalId</span><span class="sxs-lookup"><span data-stu-id="c2d86-178">externalId</span></span>|<span data-ttu-id="c2d86-179">String</span><span class="sxs-lookup"><span data-stu-id="c2d86-179">String</span></span>| <span data-ttu-id="c2d86-180">同期システムからのクラスの ID。</span><span class="sxs-lookup"><span data-stu-id="c2d86-180">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="c2d86-181">externalName</span><span class="sxs-lookup"><span data-stu-id="c2d86-181">externalName</span></span>|<span data-ttu-id="c2d86-182">String</span><span class="sxs-lookup"><span data-stu-id="c2d86-182">String</span></span>|<span data-ttu-id="c2d86-183">同期システムからのクラスの名前。</span><span class="sxs-lookup"><span data-stu-id="c2d86-183">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="c2d86-184">externalSource</span><span class="sxs-lookup"><span data-stu-id="c2d86-184">externalSource</span></span>|<span data-ttu-id="c2d86-185">文字列</span><span class="sxs-lookup"><span data-stu-id="c2d86-185">string</span></span>| <span data-ttu-id="c2d86-186">このクラスの作成方法。</span><span class="sxs-lookup"><span data-stu-id="c2d86-186">How this class was created.</span></span> <span data-ttu-id="c2d86-187">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c2d86-187">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c2d86-188">term</span><span class="sxs-lookup"><span data-stu-id="c2d86-188">term</span></span>|[<span data-ttu-id="c2d86-189">educationTerm</span><span class="sxs-lookup"><span data-stu-id="c2d86-189">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="c2d86-190">このクラスの学期。</span><span class="sxs-lookup"><span data-stu-id="c2d86-190">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c2d86-191">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c2d86-191">Relationships</span></span>
| <span data-ttu-id="c2d86-192">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c2d86-192">Relationship</span></span> | <span data-ttu-id="c2d86-193">型</span><span class="sxs-lookup"><span data-stu-id="c2d86-193">Type</span></span>   |<span data-ttu-id="c2d86-194">説明</span><span class="sxs-lookup"><span data-stu-id="c2d86-194">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2d86-195">members</span><span class="sxs-lookup"><span data-stu-id="c2d86-195">members</span></span>|<span data-ttu-id="c2d86-196">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c2d86-196">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="c2d86-197">クラスのすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="c2d86-197">All users in the class.</span></span> <span data-ttu-id="c2d86-198">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c2d86-198">Nullable.</span></span>|
|<span data-ttu-id="c2d86-199">schools</span><span class="sxs-lookup"><span data-stu-id="c2d86-199">schools</span></span>|<span data-ttu-id="c2d86-200">[educationSchool](../resources/educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c2d86-200">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="c2d86-201">このクラスに関連付けられているすべての学校。</span><span class="sxs-lookup"><span data-stu-id="c2d86-201">All schools that this class is associated with.</span></span> <span data-ttu-id="c2d86-202">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c2d86-202">Nullable.</span></span>|
|<span data-ttu-id="c2d86-203">teachers</span><span class="sxs-lookup"><span data-stu-id="c2d86-203">teachers</span></span>|<span data-ttu-id="c2d86-204">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c2d86-204">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="c2d86-205">このクラスのすべての教師。</span><span class="sxs-lookup"><span data-stu-id="c2d86-205">All teachers in the class.</span></span> <span data-ttu-id="c2d86-206">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c2d86-206">Nullable.</span></span>|
|<span data-ttu-id="c2d86-207">assignments</span><span class="sxs-lookup"><span data-stu-id="c2d86-207">assignments</span></span>|<span data-ttu-id="c2d86-208">[educationAssignment](../resources/educationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c2d86-208">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="c2d86-209">このクラスに関連付けられているすべての割り当て。</span><span class="sxs-lookup"><span data-stu-id="c2d86-209">All assignments associated with this class.</span></span> <span data-ttu-id="c2d86-210">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c2d86-210">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2d86-211">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c2d86-211">JSON representation</span></span>

<span data-ttu-id="c2d86-212">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2d86-212">The following is a JSON representation of the resource.</span></span>

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
  "term": {"@odata.type": "microsoft.graph.education.term"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
