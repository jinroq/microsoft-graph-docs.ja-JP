---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブ
localization_priority: Priority
ms.prod: sharepoint
description: ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位レベルのオブジェクトです。
doc_type: resourcePageType
ms.openlocfilehash: ba40d2ac0605a255b0b7df05db1e5bebb68c2e42
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030542"
---
# <a name="drive-resource-type"></a><span data-ttu-id="a0069-103">Drive リソース型</span><span class="sxs-lookup"><span data-stu-id="a0069-103">Drive resource type</span></span>

<span data-ttu-id="a0069-104">ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a0069-104">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="a0069-p101">OneDrive のユーザーは、少なくとも 1 つのドライブ (そのユーザーの既定のドライブ) を常に使用できます。OneDrive のライセンスが付与されていないユーザーには、使用可能な既定のドライブがないことがあります。</span><span class="sxs-lookup"><span data-stu-id="a0069-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0069-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0069-107">JSON representation</span></span>

<span data-ttu-id="a0069-108">Drive リソースの JSON 表記を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="a0069-108">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="a0069-109">**drive** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="a0069-109">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a0069-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0069-110">Properties</span></span>

| <span data-ttu-id="a0069-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0069-111">Property</span></span>             | <span data-ttu-id="a0069-112">型</span><span class="sxs-lookup"><span data-stu-id="a0069-112">Type</span></span>                          | <span data-ttu-id="a0069-113">説明</span><span class="sxs-lookup"><span data-stu-id="a0069-113">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a0069-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="a0069-114">createdBy</span></span>            | <span data-ttu-id="a0069-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a0069-115">[identitySet][]</span></span>               | <span data-ttu-id="a0069-p102">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="a0069-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0069-118">createdDateTime</span></span>      | <span data-ttu-id="a0069-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0069-119">dateTimeOffset</span></span>                | <span data-ttu-id="a0069-p103">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="a0069-122">説明</span><span class="sxs-lookup"><span data-stu-id="a0069-122">description</span></span>          | <span data-ttu-id="a0069-123">String</span><span class="sxs-lookup"><span data-stu-id="a0069-123">String</span></span>                        | <span data-ttu-id="a0069-124">ユーザーに表示されるドライブの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="a0069-124">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="a0069-125">読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="a0069-125">Read-write.</span></span>
| <span data-ttu-id="a0069-126">driveType</span><span class="sxs-lookup"><span data-stu-id="a0069-126">driveType</span></span>            | <span data-ttu-id="a0069-127">String</span><span class="sxs-lookup"><span data-stu-id="a0069-127">String</span></span>                        | <span data-ttu-id="a0069-p105">このリソースで表されるドライブの種類についての説明。OneDrive 個人用のドライブは `personal` を返します。OneDrive for Business は `business` を返します。SharePoint ドキュメント ライブラリは `documentLibrary` を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a0069-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="a0069-133">id</span><span class="sxs-lookup"><span data-stu-id="a0069-133">id</span></span>                   | <span data-ttu-id="a0069-134">String</span><span class="sxs-lookup"><span data-stu-id="a0069-134">String</span></span>                        | <span data-ttu-id="a0069-p106">ドライブの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a0069-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="a0069-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a0069-137">lastModifiedBy</span></span>       | <span data-ttu-id="a0069-138">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a0069-138">[identitySet][]</span></span>               | <span data-ttu-id="a0069-p107">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="a0069-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0069-141">lastModifiedDateTime</span></span> | <span data-ttu-id="a0069-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0069-142">dateTimeOffset</span></span>                | <span data-ttu-id="a0069-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="a0069-145">name</span><span class="sxs-lookup"><span data-stu-id="a0069-145">name</span></span>                 | <span data-ttu-id="a0069-146">string</span><span class="sxs-lookup"><span data-stu-id="a0069-146">string</span></span>                        | <span data-ttu-id="a0069-p109">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="a0069-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="a0069-149">owner</span><span class="sxs-lookup"><span data-stu-id="a0069-149">owner</span></span>                | [<span data-ttu-id="a0069-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="a0069-150">identitySet</span></span>](identityset.md) | <span data-ttu-id="a0069-p110">省略可能。ドライブを所有しているユーザー アカウント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="a0069-154">quota</span><span class="sxs-lookup"><span data-stu-id="a0069-154">quota</span></span>                | [<span data-ttu-id="a0069-155">quota</span><span class="sxs-lookup"><span data-stu-id="a0069-155">quota</span></span>](quota.md)             | <span data-ttu-id="a0069-p111">省略可能。ドライブの記憶領域クォータに関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="a0069-159">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="a0069-159">sharepointIds</span></span>        | <span data-ttu-id="a0069-160">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="a0069-160">[sharepointIds][]</span></span>             | <span data-ttu-id="a0069-p112">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="a0069-163">system</span><span class="sxs-lookup"><span data-stu-id="a0069-163">system</span></span>               | <span data-ttu-id="a0069-164">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="a0069-164">[systemFacet][]</span></span>               | <span data-ttu-id="a0069-165">存在する場合は、これがシステム管理のドライブであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="a0069-165">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="a0069-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-166">Read-only.</span></span>
| <span data-ttu-id="a0069-167">webUrl</span><span class="sxs-lookup"><span data-stu-id="a0069-167">webUrl</span></span>               | <span data-ttu-id="a0069-168">string (URL)</span><span class="sxs-lookup"><span data-stu-id="a0069-168">string (url)</span></span>                  | <span data-ttu-id="a0069-p114">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="a0069-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a0069-174">Relationships</span></span>

| <span data-ttu-id="a0069-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a0069-175">Relationship</span></span> | <span data-ttu-id="a0069-176">型</span><span class="sxs-lookup"><span data-stu-id="a0069-176">Type</span></span>                                 | <span data-ttu-id="a0069-177">説明</span><span class="sxs-lookup"><span data-stu-id="a0069-177">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="a0069-178">items</span><span class="sxs-lookup"><span data-stu-id="a0069-178">items</span></span>        | <span data-ttu-id="a0069-179">[DriveItem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a0069-179">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="a0069-p115">ドライブに含まれているすべてのアイテム。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a0069-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="a0069-183">root</span><span class="sxs-lookup"><span data-stu-id="a0069-183">root</span></span>         | [<span data-ttu-id="a0069-184">DriveItem</span><span class="sxs-lookup"><span data-stu-id="a0069-184">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="a0069-p116">ドライブのルート フォルダー。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a0069-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="a0069-187">special</span><span class="sxs-lookup"><span data-stu-id="a0069-187">special</span></span>      | <span data-ttu-id="a0069-188">[DriveItem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a0069-188">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="a0069-189">OneDrive で使用可能な共通フォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="a0069-189">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="a0069-190">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a0069-190">Read-only.</span></span> <span data-ttu-id="a0069-191">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a0069-191">Nullable.</span></span>
| <span data-ttu-id="a0069-192">リスト</span><span class="sxs-lookup"><span data-stu-id="a0069-192">list</span></span>         | [<span data-ttu-id="a0069-193">List</span><span class="sxs-lookup"><span data-stu-id="a0069-193">List</span></span>](list.md)                      | <span data-ttu-id="a0069-194">SharePoint のドライブの場合は、基になるドキュメント ライブラリのリスト。</span><span class="sxs-lookup"><span data-stu-id="a0069-194">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="a0069-195">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0069-195">Read-only.</span></span> <span data-ttu-id="a0069-196">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a0069-196">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="a0069-197">メソッド</span><span class="sxs-lookup"><span data-stu-id="a0069-197">Methods</span></span>

|                        <span data-ttu-id="a0069-198">共通タスク</span><span class="sxs-lookup"><span data-stu-id="a0069-198">Common task</span></span>                         |         <span data-ttu-id="a0069-199">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="a0069-199">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="a0069-200">[別の Drive の Drive メタデータを取得する][drive-get]</span><span class="sxs-lookup"><span data-stu-id="a0069-200">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="a0069-201">[ユーザーの既定のドライブのルート フォルダーを取得する][item-get]</span><span class="sxs-lookup"><span data-stu-id="a0069-201">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="a0069-202">[ドライブの子を一覧表示する][item-children]</span><span class="sxs-lookup"><span data-stu-id="a0069-202">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="a0069-203">[ドライブ内のすべてのアイテムの変更を一覧表示する][item-changes]</span><span class="sxs-lookup"><span data-stu-id="a0069-203">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="a0069-204">[ドライブ内のアイテムを検索する][item-search]</span><span class="sxs-lookup"><span data-stu-id="a0069-204">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="a0069-205">特殊フォルダーにアクセスする</span><span class="sxs-lookup"><span data-stu-id="a0069-205">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="a0069-206">前の表では例に `/drive` を使用していますが、他のパスも有効です。</span><span class="sxs-lookup"><span data-stu-id="a0069-206">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

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
