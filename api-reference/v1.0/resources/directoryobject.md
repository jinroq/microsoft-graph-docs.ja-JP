---
title: directoryObject リソースの種類
description: Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ae7340d273a2a02673fdfe5115e602f24680c221
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805208"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="bb5b0-104">directoryObject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb5b0-104">directoryObject resource type</span></span>

<span data-ttu-id="bb5b0-p102">Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。</span><span class="sxs-lookup"><span data-stu-id="bb5b0-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="bb5b0-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb5b0-107">Methods</span></span>

| <span data-ttu-id="bb5b0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb5b0-108">Method</span></span>       | <span data-ttu-id="bb5b0-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bb5b0-109">Return Type</span></span>  |<span data-ttu-id="bb5b0-110">説明</span><span class="sxs-lookup"><span data-stu-id="bb5b0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb5b0-111">directoryObject を取得する</span><span class="sxs-lookup"><span data-stu-id="bb5b0-111">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="bb5b0-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="bb5b0-112">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="bb5b0-113">ディレクトリ オブジェクトのプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bb5b0-113">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="bb5b0-114">directoryObject を削除する</span><span class="sxs-lookup"><span data-stu-id="bb5b0-114">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="bb5b0-115">なし</span><span class="sxs-lookup"><span data-stu-id="bb5b0-115">None</span></span> |<span data-ttu-id="bb5b0-116">ディレクトリ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="bb5b0-116">Delete a directory object.</span></span> |
|[<span data-ttu-id="bb5b0-117">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="bb5b0-117">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="bb5b0-118">String collection</span><span class="sxs-lookup"><span data-stu-id="bb5b0-118">String collection</span></span>|<span data-ttu-id="bb5b0-p103">グループの一覧内のメンバーシップを確認します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="bb5b0-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="bb5b0-121">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="bb5b0-121">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="bb5b0-122">String collection</span><span class="sxs-lookup"><span data-stu-id="bb5b0-122">String collection</span></span>|<span data-ttu-id="bb5b0-p104">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="bb5b0-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="bb5b0-125">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="bb5b0-125">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="bb5b0-126">String collection</span><span class="sxs-lookup"><span data-stu-id="bb5b0-126">String collection</span></span>| <span data-ttu-id="bb5b0-p105">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="bb5b0-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="bb5b0-129">getByIds</span><span class="sxs-lookup"><span data-stu-id="bb5b0-129">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="bb5b0-130">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bb5b0-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="bb5b0-131">指定された一連の ID に基づいて、一連のディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="bb5b0-131">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="bb5b0-132">validateProperties</span><span class="sxs-lookup"><span data-stu-id="bb5b0-132">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="bb5b0-133">Json</span><span class="sxs-lookup"><span data-stu-id="bb5b0-133">Json</span></span>| <span data-ttu-id="bb5b0-134">名前付けポリシーに準拠した Office 365 グループの表示名またはメールのニックネームを検証します。</span><span class="sxs-lookup"><span data-stu-id="bb5b0-134">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="bb5b0-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb5b0-135">Properties</span></span>

| <span data-ttu-id="bb5b0-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb5b0-136">Property</span></span>   | <span data-ttu-id="bb5b0-137">型</span><span class="sxs-lookup"><span data-stu-id="bb5b0-137">Type</span></span> |<span data-ttu-id="bb5b0-138">説明</span><span class="sxs-lookup"><span data-stu-id="bb5b0-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb5b0-139">id</span><span class="sxs-lookup"><span data-stu-id="bb5b0-139">id</span></span>|<span data-ttu-id="bb5b0-140">String</span><span class="sxs-lookup"><span data-stu-id="bb5b0-140">String</span></span>|<span data-ttu-id="bb5b0-p106">オブジェクトの一意識別子である Guid。例: 12345678-9abc-def0-1234-56789abcde。キー。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bb5b0-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb5b0-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb5b0-145">Relationships</span></span>

<span data-ttu-id="bb5b0-146">なし</span><span class="sxs-lookup"><span data-stu-id="bb5b0-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bb5b0-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb5b0-147">JSON representation</span></span>

<span data-ttu-id="bb5b0-148">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="bb5b0-148">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
