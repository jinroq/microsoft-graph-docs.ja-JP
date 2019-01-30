---
title: directoryObject リソースの種類
description: Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87fb1c21e2fa1e9788890d97f6afbd0b494c555e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640568"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="27482-104">directoryObject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27482-104">directoryObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27482-p102">Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。</span><span class="sxs-lookup"><span data-stu-id="27482-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="27482-107">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="27482-107">This resource supports:</span></span>

- <span data-ttu-id="27482-108">[デルタ](../api/directoryobject-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="27482-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="27482-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="27482-109">Methods</span></span>

| <span data-ttu-id="27482-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="27482-110">Method</span></span>       | <span data-ttu-id="27482-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="27482-111">Return Type</span></span>  |<span data-ttu-id="27482-112">説明</span><span class="sxs-lookup"><span data-stu-id="27482-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27482-113">directoryObject を取得する</span><span class="sxs-lookup"><span data-stu-id="27482-113">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="27482-114">directoryObject</span><span class="sxs-lookup"><span data-stu-id="27482-114">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="27482-115">ディレクトリ オブジェクトのプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="27482-115">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="27482-116">Delete</span><span class="sxs-lookup"><span data-stu-id="27482-116">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="27482-117">なし</span><span class="sxs-lookup"><span data-stu-id="27482-117">None</span></span> |<span data-ttu-id="27482-118">ディレクトリ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="27482-118">Delete a directory object.</span></span> |
|[<span data-ttu-id="27482-119">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="27482-119">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="27482-120">String collection</span><span class="sxs-lookup"><span data-stu-id="27482-120">String collection</span></span>|<span data-ttu-id="27482-p103">グループの一覧内のメンバーシップを確認します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="27482-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="27482-123">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="27482-123">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="27482-124">String collection</span><span class="sxs-lookup"><span data-stu-id="27482-124">String collection</span></span>|<span data-ttu-id="27482-p104">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="27482-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="27482-127">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="27482-127">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="27482-128">String collection</span><span class="sxs-lookup"><span data-stu-id="27482-128">String collection</span></span>| <span data-ttu-id="27482-p105">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="27482-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="27482-131">getByIds</span><span class="sxs-lookup"><span data-stu-id="27482-131">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="27482-132">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="27482-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="27482-133">指定された一連の ID に基づいて、一連のディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="27482-133">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="27482-134">validateProperties</span><span class="sxs-lookup"><span data-stu-id="27482-134">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="27482-135">JSON</span><span class="sxs-lookup"><span data-stu-id="27482-135">JSON</span></span>| <span data-ttu-id="27482-136">名前付けポリシーに準拠した Office 365 グループの表示名またはメール ニックネームを検証します。</span><span class="sxs-lookup"><span data-stu-id="27482-136">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="27482-137">delta</span><span class="sxs-lookup"><span data-stu-id="27482-137">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="27482-138">directoryObject コレクション</span><span class="sxs-lookup"><span data-stu-id="27482-138">directoryObject collection</span></span>| <span data-ttu-id="27482-139">ディレクトリ オブジェクトの増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="27482-139">Get incremental changes for directory objects.</span></span> <span data-ttu-id="27482-140">派生した型によるフィルター処理をサポートします。</span><span class="sxs-lookup"><span data-stu-id="27482-140">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="27482-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27482-141">Properties</span></span>

| <span data-ttu-id="27482-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27482-142">Property</span></span>   | <span data-ttu-id="27482-143">型</span><span class="sxs-lookup"><span data-stu-id="27482-143">Type</span></span> |<span data-ttu-id="27482-144">説明</span><span class="sxs-lookup"><span data-stu-id="27482-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27482-145">id</span><span class="sxs-lookup"><span data-stu-id="27482-145">id</span></span>|<span data-ttu-id="27482-146">String</span><span class="sxs-lookup"><span data-stu-id="27482-146">String</span></span>|<span data-ttu-id="27482-147">オブジェクトの一意識別子である Guid。例: 12345678-9abc-def0-1234-56789abcde12。</span><span class="sxs-lookup"><span data-stu-id="27482-147">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="27482-148">キー。</span><span class="sxs-lookup"><span data-stu-id="27482-148">Key.</span></span> <span data-ttu-id="27482-149">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="27482-149">Not nullable.</span></span> <span data-ttu-id="27482-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="27482-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27482-151">関係</span><span class="sxs-lookup"><span data-stu-id="27482-151">Relationships</span></span>

<span data-ttu-id="27482-152">なし</span><span class="sxs-lookup"><span data-stu-id="27482-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27482-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27482-153">JSON representation</span></span>

<span data-ttu-id="27482-154">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="27482-154">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
