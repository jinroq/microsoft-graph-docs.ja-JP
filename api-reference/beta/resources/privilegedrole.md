---
title: privilegedRole リソースの種類
description: 次のように、Azure AD 管理者の役割を表します:**グローバル ・ アドミニストレーター、課金管理者、サービス管理者、ユーザー管理者、管理者のパスワード**などです。
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513747"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="a85a9-103">privilegedRole リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a85a9-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a85a9-104">次のように、Azure AD 管理者の役割を表します:**グローバル ・ アドミニストレーター、課金管理者、サービス管理者、ユーザー管理者、管理者のパスワード**などです。</span><span class="sxs-lookup"><span data-stu-id="a85a9-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="a85a9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a85a9-105">Methods</span></span>

| <span data-ttu-id="a85a9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a85a9-106">Method</span></span>           | <span data-ttu-id="a85a9-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a85a9-107">Return Type</span></span>    |<span data-ttu-id="a85a9-108">説明</span><span class="sxs-lookup"><span data-stu-id="a85a9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a85a9-109">PrivilegedRole オブジェクトのリスト</span><span class="sxs-lookup"><span data-stu-id="a85a9-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="a85a9-110">[privilegedRole](privilegedrole.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a85a9-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="a85a9-111">PrivilegedRole のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a85a9-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="a85a9-112">PrivilegedRole を取得します。</span><span class="sxs-lookup"><span data-stu-id="a85a9-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="a85a9-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="a85a9-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="a85a9-114">PrivilegedRole オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a85a9-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="a85a9-115">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="a85a9-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="a85a9-116">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a85a9-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="a85a9-117">このロールの割り当てオブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a85a9-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="a85a9-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="a85a9-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="a85a9-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a85a9-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="a85a9-120">割り当て済みのロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="a85a9-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="a85a9-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="a85a9-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="a85a9-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a85a9-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="a85a9-123">割り当て済みのロールを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="a85a9-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="a85a9-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a85a9-124">Properties</span></span>
| <span data-ttu-id="a85a9-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a85a9-125">Property</span></span>     | <span data-ttu-id="a85a9-126">型</span><span class="sxs-lookup"><span data-stu-id="a85a9-126">Type</span></span>   |<span data-ttu-id="a85a9-127">説明</span><span class="sxs-lookup"><span data-stu-id="a85a9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a85a9-128">id</span><span class="sxs-lookup"><span data-stu-id="a85a9-128">id</span></span>|<span data-ttu-id="a85a9-129">文字列</span><span class="sxs-lookup"><span data-stu-id="a85a9-129">string</span></span>|<span data-ttu-id="a85a9-130">管理者の役割の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="a85a9-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="a85a9-131">GUID の文字列し、特定の役割の Azure AD からロール テンプレートの id と同じ値を持ちます。</span><span class="sxs-lookup"><span data-stu-id="a85a9-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="a85a9-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a85a9-132">Read-only.</span></span>|
|<span data-ttu-id="a85a9-133">name</span><span class="sxs-lookup"><span data-stu-id="a85a9-133">name</span></span>|<span data-ttu-id="a85a9-134">string</span><span class="sxs-lookup"><span data-stu-id="a85a9-134">string</span></span>|<span data-ttu-id="a85a9-135">ロール名です。</span><span class="sxs-lookup"><span data-stu-id="a85a9-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a85a9-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a85a9-136">Relationships</span></span>
| <span data-ttu-id="a85a9-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a85a9-137">Relationship</span></span> | <span data-ttu-id="a85a9-138">型</span><span class="sxs-lookup"><span data-stu-id="a85a9-138">Type</span></span>   |<span data-ttu-id="a85a9-139">説明</span><span class="sxs-lookup"><span data-stu-id="a85a9-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a85a9-140">assignments</span><span class="sxs-lookup"><span data-stu-id="a85a9-140">assignments</span></span>|<span data-ttu-id="a85a9-141">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a85a9-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="a85a9-142">このロールの割り当て。</span><span class="sxs-lookup"><span data-stu-id="a85a9-142">The assignments for this role.</span></span> <span data-ttu-id="a85a9-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a85a9-143">Read-only.</span></span> <span data-ttu-id="a85a9-144">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a85a9-144">Nullable.</span></span>|
|<span data-ttu-id="a85a9-145">設定</span><span class="sxs-lookup"><span data-stu-id="a85a9-145">settings</span></span>|[<span data-ttu-id="a85a9-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="a85a9-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="a85a9-147">このロールの設定をします。</span><span class="sxs-lookup"><span data-stu-id="a85a9-147">The settings for this role.</span></span> <span data-ttu-id="a85a9-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a85a9-148">Read-only.</span></span> <span data-ttu-id="a85a9-149">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a85a9-149">Nullable.</span></span>|
|<span data-ttu-id="a85a9-150">Summary</span><span class="sxs-lookup"><span data-stu-id="a85a9-150">summary</span></span>|[<span data-ttu-id="a85a9-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="a85a9-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="a85a9-152">この役割の概要情報です。</span><span class="sxs-lookup"><span data-stu-id="a85a9-152">The summary information for this role.</span></span> <span data-ttu-id="a85a9-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a85a9-153">Read-only.</span></span> <span data-ttu-id="a85a9-154">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a85a9-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a85a9-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a85a9-155">JSON representation</span></span>

<span data-ttu-id="a85a9-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a85a9-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
