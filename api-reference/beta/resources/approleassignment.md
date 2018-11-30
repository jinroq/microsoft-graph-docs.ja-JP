---
title: appRoleAssignment リソースの種類
description: ユーザーまたはグループがアプリケーションに割り当てられるときの記録に使用します。 この例では、ロールの割り当てと、アプリケーション タイルは、ユーザーのアプリケーションのアクセス パネルを表示します。 このエンティティは、特定のロールで、リソース アプリケーションに別の (サービスの主体としてモデル化された) アプリケーションのアクセス権を付与するも使用できます。 ことができます作成、読み取り、更新、およびロールの割り当てを削除します。
ms.openlocfilehash: 97155bde12735ebd8a7674e0dbf20dae30e53f14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067936"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="8f468-106">appRoleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f468-106">appRoleAssignment resource type</span></span>

> <span data-ttu-id="8f468-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8f468-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f468-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f468-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f468-109">ユーザーまたはグループがアプリケーションに割り当てられるときの記録に使用します。</span><span class="sxs-lookup"><span data-stu-id="8f468-109">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="8f468-110">この例では、ロールの割り当てと、アプリケーション タイルは、ユーザーのアプリケーションのアクセス パネルを表示します。</span><span class="sxs-lookup"><span data-stu-id="8f468-110">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="8f468-111">このエンティティは、特定のロールで、リソース アプリケーションに別の (サービスの主体としてモデル化された) アプリケーションのアクセス権を付与するも使用できます。</span><span class="sxs-lookup"><span data-stu-id="8f468-111">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="8f468-112">ことができます作成、読み取り、更新、およびロールの割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="8f468-112">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f468-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f468-113">JSON representation</span></span>

<span data-ttu-id="8f468-114">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8f468-114">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8f468-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f468-115">Properties</span></span>
| <span data-ttu-id="8f468-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f468-116">Property</span></span>     | <span data-ttu-id="8f468-117">型</span><span class="sxs-lookup"><span data-stu-id="8f468-117">Type</span></span>   |<span data-ttu-id="8f468-118">説明</span><span class="sxs-lookup"><span data-stu-id="8f468-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f468-119">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="8f468-119">creationTimestamp</span></span>|<span data-ttu-id="8f468-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f468-120">DateTimeOffset</span></span>|<span data-ttu-id="8f468-121">交付が作成された時刻。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。</span><span class="sxs-lookup"><span data-stu-id="8f468-121">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f468-122">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8f468-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8f468-123">ID</span><span class="sxs-lookup"><span data-stu-id="8f468-123">id</span></span>|<span data-ttu-id="8f468-124">Guid</span><span class="sxs-lookup"><span data-stu-id="8f468-124">Guid</span></span>|<span data-ttu-id="8f468-125">プリンシパルに割り当てられたロールの id です。</span><span class="sxs-lookup"><span data-stu-id="8f468-125">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="8f468-126">この役割は、 **appRoles**プロパティにターゲットのリソース アプリケーション**引数 resourceId**で宣言されなければなりません。</span><span class="sxs-lookup"><span data-stu-id="8f468-126">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="8f468-127">リソースですべてのアクセス許可が宣言されていない場合は、デフォルトの id (GUID は 0) を指定してください。</span><span class="sxs-lookup"><span data-stu-id="8f468-127">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="8f468-128">キー。</span><span class="sxs-lookup"><span data-stu-id="8f468-128">Key.</span></span> <span data-ttu-id="8f468-129">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="8f468-129">Not nullable.</span></span> |
|<span data-ttu-id="8f468-130">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="8f468-130">principalDisplayName</span></span>|<span data-ttu-id="8f468-131">String</span><span class="sxs-lookup"><span data-stu-id="8f468-131">String</span></span>|<span data-ttu-id="8f468-132">アクセス権を与えられたプリンシパルの表示名。</span><span class="sxs-lookup"><span data-stu-id="8f468-132">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="8f468-133">principalId</span><span class="sxs-lookup"><span data-stu-id="8f468-133">principalId</span></span>|<span data-ttu-id="8f468-134">Guid</span><span class="sxs-lookup"><span data-stu-id="8f468-134">Guid</span></span>|<span data-ttu-id="8f468-135">アクセスを付与されているプリンシパルの一意の識別子 (**id**) です。</span><span class="sxs-lookup"><span data-stu-id="8f468-135">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="8f468-136">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="8f468-136">Required on create.</span></span>            |
|<span data-ttu-id="8f468-137">principalType</span><span class="sxs-lookup"><span data-stu-id="8f468-137">principalType</span></span>|<span data-ttu-id="8f468-138">String</span><span class="sxs-lookup"><span data-stu-id="8f468-138">String</span></span>|<span data-ttu-id="8f468-139">プリンシパルの種類。</span><span class="sxs-lookup"><span data-stu-id="8f468-139">The type of principal.</span></span>  <span data-ttu-id="8f468-140">「ユーザー」、「グループ」または"ServicePrincipal"指定できます。</span><span class="sxs-lookup"><span data-stu-id="8f468-140">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="8f468-141">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8f468-141">resourceDisplayName</span></span>|<span data-ttu-id="8f468-142">String</span><span class="sxs-lookup"><span data-stu-id="8f468-142">String</span></span>|<span data-ttu-id="8f468-143">割り当てが作成するリソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="8f468-143">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="8f468-144">resourceId</span><span class="sxs-lookup"><span data-stu-id="8f468-144">resourceId</span></span>|<span data-ttu-id="8f468-145">Guid</span><span class="sxs-lookup"><span data-stu-id="8f468-145">Guid</span></span>|<span data-ttu-id="8f468-146">割り当てが作成する対象のリソース (サービス主体) の一意の識別子 (**id**) です。</span><span class="sxs-lookup"><span data-stu-id="8f468-146">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f468-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8f468-147">Relationships</span></span>
<span data-ttu-id="8f468-148">なし</span><span class="sxs-lookup"><span data-stu-id="8f468-148">None</span></span>


## <a name="methods"></a><span data-ttu-id="8f468-149">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f468-149">Methods</span></span>

| <span data-ttu-id="8f468-150">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f468-150">Method</span></span>           | <span data-ttu-id="8f468-151">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8f468-151">Return Type</span></span>    |<span data-ttu-id="8f468-152">説明</span><span class="sxs-lookup"><span data-stu-id="8f468-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f468-153">AppRoleAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="8f468-153">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="8f468-154">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8f468-154">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="8f468-155">AppRoleAssignment オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f468-155">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="8f468-156">Update</span><span class="sxs-lookup"><span data-stu-id="8f468-156">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="8f468-157">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8f468-157">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="8f468-158">AppRoleAssignment オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="8f468-158">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="8f468-159">削除</span><span class="sxs-lookup"><span data-stu-id="8f468-159">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="8f468-160">なし</span><span class="sxs-lookup"><span data-stu-id="8f468-160">None</span></span> |<span data-ttu-id="8f468-161">AppRoleAssignment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="8f468-161">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->