---
title: appRoleAssignment リソースの種類
description: ユーザーまたはグループがアプリケーションに割り当てられるときの記録に使用します。 この例では、ロールの割り当てにより、アプリケーション タイルが、ユーザー アプリケーションのアクセス パネル上に表示されます。 特定のロールで、リソース アプリケーションに別の (サービス プリンシパルとしてモデル化された) アプリケーションのアクセス権を付与する場合にも、このエンティティを使用できます。 ロールの割り当ての作成、読み取り、更新、削除ができます。
localization_priority: Priority
ms.openlocfilehash: 6255642f47f0e1454fb64440d4938605a2de5df4
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640435"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="96511-106">appRoleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96511-106">appRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96511-107">ユーザーまたはグループがアプリケーションに割り当てられるときの記録に使用します。</span><span class="sxs-lookup"><span data-stu-id="96511-107">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="96511-108">この例では、ロールの割り当てにより、アプリケーション タイルが、ユーザー アプリケーションのアクセス パネル上に表示されます。</span><span class="sxs-lookup"><span data-stu-id="96511-108">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="96511-109">特定のロールで、リソース アプリケーションに別の (サービス プリンシパルとしてモデル化された) アプリケーションのアクセス権を付与する場合にも、このエンティティを使用できます。</span><span class="sxs-lookup"><span data-stu-id="96511-109">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="96511-110">ロールの割り当ての作成、読み取り、更新、削除ができます。</span><span class="sxs-lookup"><span data-stu-id="96511-110">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="96511-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96511-111">JSON representation</span></span>

<span data-ttu-id="96511-112">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="96511-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a><span data-ttu-id="96511-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96511-113">Properties</span></span>
| <span data-ttu-id="96511-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96511-114">Property</span></span>     | <span data-ttu-id="96511-115">型</span><span class="sxs-lookup"><span data-stu-id="96511-115">Type</span></span>   |<span data-ttu-id="96511-116">説明</span><span class="sxs-lookup"><span data-stu-id="96511-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96511-117">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="96511-117">creationTimestamp</span></span>|<span data-ttu-id="96511-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96511-118">DateTimeOffset</span></span>|<span data-ttu-id="96511-119">許可が出された時間です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="96511-119">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96511-120">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96511-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="96511-121">id</span><span class="sxs-lookup"><span data-stu-id="96511-121">id</span></span>|<span data-ttu-id="96511-122">Guid</span><span class="sxs-lookup"><span data-stu-id="96511-122">Guid</span></span>|<span data-ttu-id="96511-123">プリンシパルに割り当てられたロール ID です。</span><span class="sxs-lookup"><span data-stu-id="96511-123">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="96511-124">このロールは、**appRoles** プロパティのターゲット リソース アプリケーション **resourceId** によって宣言される必要があります。</span><span class="sxs-lookup"><span data-stu-id="96511-124">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="96511-125">リソースがアクセス許可を宣言していない場合は、既存の ID (ゼロ GUID) を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="96511-125">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="96511-126">キー。</span><span class="sxs-lookup"><span data-stu-id="96511-126">Key.</span></span> <span data-ttu-id="96511-127">null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="96511-127">Not nullable.</span></span> |
|<span data-ttu-id="96511-128">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="96511-128">principalDisplayName</span></span>|<span data-ttu-id="96511-129">String</span><span class="sxs-lookup"><span data-stu-id="96511-129">String</span></span>|<span data-ttu-id="96511-130">アクセス権が付与されているプリンシパルの表示名。</span><span class="sxs-lookup"><span data-stu-id="96511-130">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="96511-131">principalId</span><span class="sxs-lookup"><span data-stu-id="96511-131">principalId</span></span>|<span data-ttu-id="96511-132">Guid</span><span class="sxs-lookup"><span data-stu-id="96511-132">Guid</span></span>|<span data-ttu-id="96511-133">アクセス権が付与されているプリンシパルの一意の識別子 (**id**) です。</span><span class="sxs-lookup"><span data-stu-id="96511-133">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="96511-134">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="96511-134">Required on create.</span></span>            |
|<span data-ttu-id="96511-135">principalType</span><span class="sxs-lookup"><span data-stu-id="96511-135">principalType</span></span>|<span data-ttu-id="96511-136">String</span><span class="sxs-lookup"><span data-stu-id="96511-136">String</span></span>|<span data-ttu-id="96511-137">プリンシパルの種類。</span><span class="sxs-lookup"><span data-stu-id="96511-137">The type of principal.</span></span>  <span data-ttu-id="96511-138">"User"、"Group"、"ServicePrincipal" のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="96511-138">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="96511-139">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="96511-139">resourceDisplayName</span></span>|<span data-ttu-id="96511-140">String</span><span class="sxs-lookup"><span data-stu-id="96511-140">String</span></span>|<span data-ttu-id="96511-141">割り当てが作成されたリソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="96511-141">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="96511-142">resourceId</span><span class="sxs-lookup"><span data-stu-id="96511-142">resourceId</span></span>|<span data-ttu-id="96511-143">Guid</span><span class="sxs-lookup"><span data-stu-id="96511-143">Guid</span></span>|<span data-ttu-id="96511-144">割り当てが作成されたターゲット リソース (サービス プリンシパル) の一意の識別子 (**id**) です。</span><span class="sxs-lookup"><span data-stu-id="96511-144">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96511-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96511-145">Relationships</span></span>
<span data-ttu-id="96511-146">なし</span><span class="sxs-lookup"><span data-stu-id="96511-146">None</span></span>


## <a name="methods"></a><span data-ttu-id="96511-147">メソッド</span><span class="sxs-lookup"><span data-stu-id="96511-147">Methods</span></span>

| <span data-ttu-id="96511-148">メソッド</span><span class="sxs-lookup"><span data-stu-id="96511-148">Method</span></span>           | <span data-ttu-id="96511-149">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="96511-149">Return Type</span></span>    |<span data-ttu-id="96511-150">説明</span><span class="sxs-lookup"><span data-stu-id="96511-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96511-151">appRoleAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="96511-151">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="96511-152">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="96511-152">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="96511-153">appRoleAssignment オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="96511-153">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="96511-154">更新する</span><span class="sxs-lookup"><span data-stu-id="96511-154">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="96511-155">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="96511-155">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="96511-156">appRoleAssignment オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="96511-156">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="96511-157">削除する</span><span class="sxs-lookup"><span data-stu-id="96511-157">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="96511-158">なし</span><span class="sxs-lookup"><span data-stu-id="96511-158">None</span></span> |<span data-ttu-id="96511-159">appRoleAssignment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="96511-159">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
