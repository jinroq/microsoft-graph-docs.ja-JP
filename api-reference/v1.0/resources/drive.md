---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 3b9744d8b652f0374c71f5304c326ba862c288a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929131"
---
# <a name="drive-resource-type"></a><span data-ttu-id="f55cd-102">ドライブ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f55cd-102">Drive resource type</span></span>

<span data-ttu-id="f55cd-103">ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f55cd-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="f55cd-p101">OneDrive のユーザーは、少なくとも 1 つのドライブ (そのユーザーの既定のドライブ) を常に使用できます。OneDrive のライセンスが付与されていないユーザーには、使用可能な既定のドライブがないことがあります。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f55cd-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f55cd-106">JSON representation</span></span>

<span data-ttu-id="f55cd-107">ドライブ リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f55cd-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="f55cd-108">**drive** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="f55cd-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "sharepointIds",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="f55cd-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f55cd-109">Properties</span></span>

| <span data-ttu-id="f55cd-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f55cd-110">Property</span></span>             | <span data-ttu-id="f55cd-111">型</span><span class="sxs-lookup"><span data-stu-id="f55cd-111">Type</span></span>                          | <span data-ttu-id="f55cd-112">説明</span><span class="sxs-lookup"><span data-stu-id="f55cd-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f55cd-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="f55cd-113">createdBy</span></span>            | <span data-ttu-id="f55cd-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f55cd-114">[identitySet][]</span></span>               | <span data-ttu-id="f55cd-p102">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="f55cd-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f55cd-117">createdDateTime</span></span>      | <span data-ttu-id="f55cd-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f55cd-118">dateTimeOffset</span></span>                | <span data-ttu-id="f55cd-p103">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="f55cd-121">説明</span><span class="sxs-lookup"><span data-stu-id="f55cd-121">description</span></span>          | <span data-ttu-id="f55cd-122">String</span><span class="sxs-lookup"><span data-stu-id="f55cd-122">String</span></span>                        | <span data-ttu-id="f55cd-123">ユーザーに表示されるドライブの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="f55cd-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="f55cd-124">読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="f55cd-124">Read-write.</span></span>
| <span data-ttu-id="f55cd-125">driveType</span><span class="sxs-lookup"><span data-stu-id="f55cd-125">driveType</span></span>            | <span data-ttu-id="f55cd-126">String</span><span class="sxs-lookup"><span data-stu-id="f55cd-126">String</span></span>                        | <span data-ttu-id="f55cd-p105">このリソースで表されるドライブの種類についての説明。OneDrive 個人用のドライブは `personal` を返します。OneDrive for Business は `business` を返します。SharePoint ドキュメント ライブラリは `documentLibrary` を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="f55cd-132">id</span><span class="sxs-lookup"><span data-stu-id="f55cd-132">id</span></span>                   | <span data-ttu-id="f55cd-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f55cd-133">String</span></span>                        | <span data-ttu-id="f55cd-p106">ドライブの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="f55cd-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f55cd-136">lastModifiedBy</span></span>       | <span data-ttu-id="f55cd-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f55cd-137">[identitySet][]</span></span>               | <span data-ttu-id="f55cd-p107">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="f55cd-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f55cd-140">lastModifiedDateTime</span></span> | <span data-ttu-id="f55cd-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f55cd-141">dateTimeOffset</span></span>                | <span data-ttu-id="f55cd-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="f55cd-144">name</span><span class="sxs-lookup"><span data-stu-id="f55cd-144">name</span></span>                 | <span data-ttu-id="f55cd-145">string</span><span class="sxs-lookup"><span data-stu-id="f55cd-145">string</span></span>                        | <span data-ttu-id="f55cd-p109">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="f55cd-148">owner</span><span class="sxs-lookup"><span data-stu-id="f55cd-148">owner</span></span>                | [<span data-ttu-id="f55cd-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="f55cd-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="f55cd-p110">省略可能。ドライブを所有しているユーザー アカウント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="f55cd-153">quota</span><span class="sxs-lookup"><span data-stu-id="f55cd-153">quota</span></span>                | [<span data-ttu-id="f55cd-154">quota</span><span class="sxs-lookup"><span data-stu-id="f55cd-154">quota</span></span>](quota.md)             | <span data-ttu-id="f55cd-p111">省略可能。ドライブの記憶領域クォータに関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="f55cd-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="f55cd-158">sharepointIds</span></span>        | <span data-ttu-id="f55cd-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f55cd-159">[sharepointIds][]</span></span>             | <span data-ttu-id="f55cd-p112">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="f55cd-162">システム</span><span class="sxs-lookup"><span data-stu-id="f55cd-162">system</span></span>               | <span data-ttu-id="f55cd-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="f55cd-163">[systemFacet][]</span></span>               | <span data-ttu-id="f55cd-164">存在する場合は、これがシステム管理のドライブであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="f55cd-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="f55cd-165">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-165">Read-only.</span></span>
| <span data-ttu-id="f55cd-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="f55cd-166">webUrl</span></span>               | <span data-ttu-id="f55cd-167">string (URL)</span><span class="sxs-lookup"><span data-stu-id="f55cd-167">string (url)</span></span>                  | <span data-ttu-id="f55cd-p114">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="f55cd-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f55cd-173">Relationships</span></span>

| <span data-ttu-id="f55cd-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f55cd-174">Relationship</span></span> | <span data-ttu-id="f55cd-175">型</span><span class="sxs-lookup"><span data-stu-id="f55cd-175">Type</span></span>                                 | <span data-ttu-id="f55cd-176">説明</span><span class="sxs-lookup"><span data-stu-id="f55cd-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="f55cd-177">items</span><span class="sxs-lookup"><span data-stu-id="f55cd-177">items</span></span>        | <span data-ttu-id="f55cd-178">[DriveItem](driveitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f55cd-178">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="f55cd-p115">ドライブに含まれているすべてのアイテム。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="f55cd-182">root</span><span class="sxs-lookup"><span data-stu-id="f55cd-182">root</span></span>         | [<span data-ttu-id="f55cd-183">DriveItem</span><span class="sxs-lookup"><span data-stu-id="f55cd-183">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="f55cd-p116">ドライブのルート フォルダー。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="f55cd-186">special</span><span class="sxs-lookup"><span data-stu-id="f55cd-186">special</span></span>      | <span data-ttu-id="f55cd-187">[DriveItem](driveitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f55cd-187">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="f55cd-p117">OneDrive で使用可能な共通フォルダーのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f55cd-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="f55cd-191">リスト</span><span class="sxs-lookup"><span data-stu-id="f55cd-191">list</span></span>         | [<span data-ttu-id="f55cd-192">List</span><span class="sxs-lookup"><span data-stu-id="f55cd-192">List</span></span>](list.md)                      | <span data-ttu-id="f55cd-193">SharePoint では、基になるドキュメント ライブラリの一覧でドライブします。</span><span class="sxs-lookup"><span data-stu-id="f55cd-193">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="f55cd-194">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-194">Read-only.</span></span> <span data-ttu-id="f55cd-195">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f55cd-195">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="f55cd-196">メソッド</span><span class="sxs-lookup"><span data-stu-id="f55cd-196">Methods</span></span>

|                        <span data-ttu-id="f55cd-197">共通タスク</span><span class="sxs-lookup"><span data-stu-id="f55cd-197">Common task</span></span>                         |         <span data-ttu-id="f55cd-198">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="f55cd-198">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="f55cd-199">[別のドライブのドライブ メタデータを取得する][drive-get]</span><span class="sxs-lookup"><span data-stu-id="f55cd-199">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="f55cd-200">[ユーザーの既定のドライブのルート フォルダーを取得する][item-get]</span><span class="sxs-lookup"><span data-stu-id="f55cd-200">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="f55cd-201">[ドライブの子を一覧表示する][item-children]</span><span class="sxs-lookup"><span data-stu-id="f55cd-201">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="f55cd-202">[ドライブ内のすべてのアイテムの変更を一覧表示する][item-changes]</span><span class="sxs-lookup"><span data-stu-id="f55cd-202">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="f55cd-203">[ドライブ内のアイテムを検索する][item-search]</span><span class="sxs-lookup"><span data-stu-id="f55cd-203">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="f55cd-204">特別なフォルダーにアクセスする</span><span class="sxs-lookup"><span data-stu-id="f55cd-204">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="f55cd-205">前の表では例に `/drive` を使用していますが、他のパスも有効です。</span><span class="sxs-lookup"><span data-stu-id="f55cd-205">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/drive.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
