---
title: directoryObject リソースの種類
description: Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b71de12ba6a0053cd97749fd72dc22f7ab961539
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34658030"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="fbaf8-104">directoryObject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fbaf8-104">directoryObject resource type</span></span>

<span data-ttu-id="fbaf8-p102">Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。</span><span class="sxs-lookup"><span data-stu-id="fbaf8-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="fbaf8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fbaf8-107">Methods</span></span>

| <span data-ttu-id="fbaf8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fbaf8-108">Method</span></span>       | <span data-ttu-id="fbaf8-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fbaf8-109">Return Type</span></span>  |<span data-ttu-id="fbaf8-110">説明</span><span class="sxs-lookup"><span data-stu-id="fbaf8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbaf8-111">directoryObject を取得する</span><span class="sxs-lookup"><span data-stu-id="fbaf8-111">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="fbaf8-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="fbaf8-112">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="fbaf8-113">ディレクトリ オブジェクトのプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fbaf8-113">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="fbaf8-114">directoryObject を削除する</span><span class="sxs-lookup"><span data-stu-id="fbaf8-114">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="fbaf8-115">なし</span><span class="sxs-lookup"><span data-stu-id="fbaf8-115">None</span></span> |<span data-ttu-id="fbaf8-116">ディレクトリ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="fbaf8-116">Delete a directory object.</span></span> |
|[<span data-ttu-id="fbaf8-117">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="fbaf8-117">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="fbaf8-118">String collection</span><span class="sxs-lookup"><span data-stu-id="fbaf8-118">String collection</span></span>|<span data-ttu-id="fbaf8-p103">グループの一覧内のメンバーシップを確認します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="fbaf8-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="fbaf8-121">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="fbaf8-121">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="fbaf8-122">String collection</span><span class="sxs-lookup"><span data-stu-id="fbaf8-122">String collection</span></span>|<span data-ttu-id="fbaf8-p104">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="fbaf8-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="fbaf8-125">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="fbaf8-125">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="fbaf8-126">String collection</span><span class="sxs-lookup"><span data-stu-id="fbaf8-126">String collection</span></span>| <span data-ttu-id="fbaf8-p105">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="fbaf8-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="fbaf8-129">getByIds</span><span class="sxs-lookup"><span data-stu-id="fbaf8-129">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="fbaf8-130">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbaf8-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="fbaf8-131">指定された一連の ID に基づいて、一連のディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="fbaf8-131">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="fbaf8-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbaf8-132">Properties</span></span>

| <span data-ttu-id="fbaf8-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbaf8-133">Property</span></span>   | <span data-ttu-id="fbaf8-134">型</span><span class="sxs-lookup"><span data-stu-id="fbaf8-134">Type</span></span> |<span data-ttu-id="fbaf8-135">説明</span><span class="sxs-lookup"><span data-stu-id="fbaf8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbaf8-136">id</span><span class="sxs-lookup"><span data-stu-id="fbaf8-136">id</span></span>|<span data-ttu-id="fbaf8-137">String</span><span class="sxs-lookup"><span data-stu-id="fbaf8-137">String</span></span>|<span data-ttu-id="fbaf8-p106">オブジェクトの一意識別子である Guid。例: 12345678-9abc-def0-1234-56789abcde。キー。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fbaf8-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbaf8-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbaf8-142">Relationships</span></span>

<span data-ttu-id="fbaf8-143">なし</span><span class="sxs-lookup"><span data-stu-id="fbaf8-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fbaf8-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbaf8-144">JSON representation</span></span>

<span data-ttu-id="fbaf8-145">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="fbaf8-145">Here is a JSON representation of the resource</span></span>

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
