---
title: educationClass リソース タイプ
description: '学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。  '
localization_priority: Normal
ms.openlocfilehash: 1c657a1eba131a9bcfa8dd4f84e2ba2141a4750a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866788"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="714a8-106">educationClass リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="714a8-106">educationClass resource type</span></span>

> <span data-ttu-id="714a8-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="714a8-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="714a8-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="714a8-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="714a8-109">学校内のクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="714a8-109">Represents a class within a school.</span></span> <span data-ttu-id="714a8-110">**educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。</span><span class="sxs-lookup"><span data-stu-id="714a8-110">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="714a8-111">学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。</span><span class="sxs-lookup"><span data-stu-id="714a8-111">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="714a8-112">Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="714a8-112">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="714a8-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="714a8-113">Methods</span></span>

| <span data-ttu-id="714a8-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="714a8-114">Method</span></span>           | <span data-ttu-id="714a8-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="714a8-115">Return Type</span></span>    |<span data-ttu-id="714a8-116">説明</span><span class="sxs-lookup"><span data-stu-id="714a8-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="714a8-117">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="714a8-117">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="714a8-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="714a8-118">educationClass</span></span>](educationclass.md) |<span data-ttu-id="714a8-119">**educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="714a8-119">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="714a8-120">Add member</span><span class="sxs-lookup"><span data-stu-id="714a8-120">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="714a8-121">educationUser</span><span class="sxs-lookup"><span data-stu-id="714a8-121">educationUser</span></span>](educationuser.md)| <span data-ttu-id="714a8-122">members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="714a8-122">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="714a8-123">List members</span><span class="sxs-lookup"><span data-stu-id="714a8-123">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="714a8-124">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="714a8-124">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="714a8-125">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="714a8-125">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="714a8-126">Remove student</span><span class="sxs-lookup"><span data-stu-id="714a8-126">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="714a8-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="714a8-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="714a8-128">members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="714a8-128">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="714a8-129">List schools</span><span class="sxs-lookup"><span data-stu-id="714a8-129">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="714a8-130">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="714a8-130">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="714a8-131">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="714a8-131">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="714a8-132">Add teacher</span><span class="sxs-lookup"><span data-stu-id="714a8-132">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="714a8-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="714a8-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="714a8-134">teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="714a8-134">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="714a8-135">List teachers</span><span class="sxs-lookup"><span data-stu-id="714a8-135">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="714a8-136">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="714a8-136">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="714a8-137">クラスの教師一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="714a8-137">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="714a8-138">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="714a8-138">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="714a8-139">educationUser</span><span class="sxs-lookup"><span data-stu-id="714a8-139">educationUser</span></span>](educationuser.md)| <span data-ttu-id="714a8-140">teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="714a8-140">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="714a8-141">EducationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="714a8-141">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="714a8-142">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="714a8-142">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="714a8-143">割り当てのコレクションへの投稿には、新しい**educationAssignment**を作成します。</span><span class="sxs-lookup"><span data-stu-id="714a8-143">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="714a8-144">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="714a8-144">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="714a8-145">[educationAssignment](../resources/educationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="714a8-145">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="714a8-146">**EducationAssignment**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="714a8-146">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="714a8-147">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="714a8-147">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="714a8-148">group</span><span class="sxs-lookup"><span data-stu-id="714a8-148">group</span></span>](group.md)| <span data-ttu-id="714a8-149">この **educationClass** に対応する Office 365 **group**を取得します。</span><span class="sxs-lookup"><span data-stu-id="714a8-149">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="714a8-150">Update</span><span class="sxs-lookup"><span data-stu-id="714a8-150">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="714a8-151">educationClass</span><span class="sxs-lookup"><span data-stu-id="714a8-151">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="714a8-152">**educationClass** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="714a8-152">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="714a8-153">Delete</span><span class="sxs-lookup"><span data-stu-id="714a8-153">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="714a8-154">なし</span><span class="sxs-lookup"><span data-stu-id="714a8-154">None</span></span> |<span data-ttu-id="714a8-155">**educationClass** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="714a8-155">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="714a8-156">プロパティ</span><span class="sxs-lookup"><span data-stu-id="714a8-156">Properties</span></span>
| <span data-ttu-id="714a8-157">プロパティ</span><span class="sxs-lookup"><span data-stu-id="714a8-157">Property</span></span>     | <span data-ttu-id="714a8-158">種類</span><span class="sxs-lookup"><span data-stu-id="714a8-158">Type</span></span>   |<span data-ttu-id="714a8-159">説明</span><span class="sxs-lookup"><span data-stu-id="714a8-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="714a8-160">ID</span><span class="sxs-lookup"><span data-stu-id="714a8-160">id</span></span>| <span data-ttu-id="714a8-161">String</span><span class="sxs-lookup"><span data-stu-id="714a8-161">String</span></span>| <span data-ttu-id="714a8-162">クラスの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="714a8-162">Unique identifier for the class.</span></span>|
|<span data-ttu-id="714a8-163">説明</span><span class="sxs-lookup"><span data-stu-id="714a8-163">description</span></span>|<span data-ttu-id="714a8-164">String</span><span class="sxs-lookup"><span data-stu-id="714a8-164">String</span></span>| <span data-ttu-id="714a8-165">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="714a8-165">Description of the class.</span></span>|
|<span data-ttu-id="714a8-166">displayName</span><span class="sxs-lookup"><span data-stu-id="714a8-166">displayName</span></span>|<span data-ttu-id="714a8-167">String</span><span class="sxs-lookup"><span data-stu-id="714a8-167">String</span></span>| <span data-ttu-id="714a8-168">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="714a8-168">Name of the class.</span></span>|
|<span data-ttu-id="714a8-169">mailNickname</span><span class="sxs-lookup"><span data-stu-id="714a8-169">mailNickname</span></span>|<span data-ttu-id="714a8-170">String</span><span class="sxs-lookup"><span data-stu-id="714a8-170">String</span></span>| <span data-ttu-id="714a8-171">すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。</span><span class="sxs-lookup"><span data-stu-id="714a8-171">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="714a8-172">createdBy</span><span class="sxs-lookup"><span data-stu-id="714a8-172">createdBy</span></span>|[<span data-ttu-id="714a8-173">identitySet</span><span class="sxs-lookup"><span data-stu-id="714a8-173">identitySet</span></span>](identityset.md)| <span data-ttu-id="714a8-174">クラスを作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="714a8-174">Entity who created the class</span></span> |
|<span data-ttu-id="714a8-175">classCode</span><span class="sxs-lookup"><span data-stu-id="714a8-175">classCode</span></span>|<span data-ttu-id="714a8-176">String</span><span class="sxs-lookup"><span data-stu-id="714a8-176">String</span></span>| <span data-ttu-id="714a8-177">クラスを識別するために学校が使用するクラス コード。</span><span class="sxs-lookup"><span data-stu-id="714a8-177">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="714a8-178">externalId</span><span class="sxs-lookup"><span data-stu-id="714a8-178">externalId</span></span>|<span data-ttu-id="714a8-179">String</span><span class="sxs-lookup"><span data-stu-id="714a8-179">String</span></span>| <span data-ttu-id="714a8-180">同期システムからのクラスの ID。</span><span class="sxs-lookup"><span data-stu-id="714a8-180">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="714a8-181">externalName</span><span class="sxs-lookup"><span data-stu-id="714a8-181">externalName</span></span>|<span data-ttu-id="714a8-182">String</span><span class="sxs-lookup"><span data-stu-id="714a8-182">String</span></span>|<span data-ttu-id="714a8-183">同期システムからのクラスの名前。</span><span class="sxs-lookup"><span data-stu-id="714a8-183">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="714a8-184">externalSource</span><span class="sxs-lookup"><span data-stu-id="714a8-184">externalSource</span></span>|<span data-ttu-id="714a8-185">文字列</span><span class="sxs-lookup"><span data-stu-id="714a8-185">string</span></span>| <span data-ttu-id="714a8-186">このクラスの作成方法。</span><span class="sxs-lookup"><span data-stu-id="714a8-186">How this class was created.</span></span> <span data-ttu-id="714a8-187">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="714a8-187">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="714a8-188">term</span><span class="sxs-lookup"><span data-stu-id="714a8-188">term</span></span>|[<span data-ttu-id="714a8-189">educationTerm</span><span class="sxs-lookup"><span data-stu-id="714a8-189">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="714a8-190">このクラスの学期。</span><span class="sxs-lookup"><span data-stu-id="714a8-190">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="714a8-191">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="714a8-191">Relationships</span></span>
| <span data-ttu-id="714a8-192">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="714a8-192">Relationship</span></span> | <span data-ttu-id="714a8-193">型</span><span class="sxs-lookup"><span data-stu-id="714a8-193">Type</span></span>   |<span data-ttu-id="714a8-194">説明</span><span class="sxs-lookup"><span data-stu-id="714a8-194">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="714a8-195">members</span><span class="sxs-lookup"><span data-stu-id="714a8-195">members</span></span>|<span data-ttu-id="714a8-196">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="714a8-196">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="714a8-197">クラスのすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="714a8-197">All users in the class.</span></span> <span data-ttu-id="714a8-198">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="714a8-198">Nullable.</span></span>|
|<span data-ttu-id="714a8-199">schools</span><span class="sxs-lookup"><span data-stu-id="714a8-199">schools</span></span>|<span data-ttu-id="714a8-200">[educationSchool](../resources/educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="714a8-200">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="714a8-201">このクラスに関連付けられているすべての学校。</span><span class="sxs-lookup"><span data-stu-id="714a8-201">All schools that this class is associated with.</span></span> <span data-ttu-id="714a8-202">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="714a8-202">Nullable.</span></span>|
|<span data-ttu-id="714a8-203">teachers</span><span class="sxs-lookup"><span data-stu-id="714a8-203">teachers</span></span>|<span data-ttu-id="714a8-204">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="714a8-204">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="714a8-205">このクラスのすべての教師。</span><span class="sxs-lookup"><span data-stu-id="714a8-205">All teachers in the class.</span></span> <span data-ttu-id="714a8-206">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="714a8-206">Nullable.</span></span>|
|<span data-ttu-id="714a8-207">assignments</span><span class="sxs-lookup"><span data-stu-id="714a8-207">assignments</span></span>|<span data-ttu-id="714a8-208">[educationAssignment](../resources/educationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="714a8-208">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="714a8-209">このクラスに関連付けられているすべての割り当て。</span><span class="sxs-lookup"><span data-stu-id="714a8-209">All assignments associated with this class.</span></span> <span data-ttu-id="714a8-210">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="714a8-210">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="714a8-211">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="714a8-211">JSON representation</span></span>

<span data-ttu-id="714a8-212">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="714a8-212">The following is a JSON representation of the resource.</span></span>

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
