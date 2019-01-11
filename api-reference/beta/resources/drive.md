---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.openlocfilehash: 684a200d38aea52054bedb9eb4357c28e03b37e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840832"
---
# <a name="drive-resource-type"></a><span data-ttu-id="5f12d-102">ドライブ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f12d-102">drive resource type</span></span>

> <span data-ttu-id="5f12d-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5f12d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f12d-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f12d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f12d-105">ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5f12d-105">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="5f12d-p102">OneDrive のユーザーは、少なくとも 1 つのドライブ (そのユーザーの既定のドライブ) を常に使用できます。OneDrive のライセンスが付与されていないユーザーには、使用可能な既定のドライブがないことがあります。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p102">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f12d-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f12d-108">JSON representation</span></span>

<span data-ttu-id="5f12d-109">ドライブ リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f12d-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="5f12d-110">**drive** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="5f12d-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="5f12d-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f12d-111">Properties</span></span>

| <span data-ttu-id="5f12d-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f12d-112">Property</span></span>             | <span data-ttu-id="5f12d-113">種類</span><span class="sxs-lookup"><span data-stu-id="5f12d-113">Type</span></span>                          | <span data-ttu-id="5f12d-114">説明</span><span class="sxs-lookup"><span data-stu-id="5f12d-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5f12d-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="5f12d-115">createdBy</span></span>            | <span data-ttu-id="5f12d-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5f12d-116">[identitySet][]</span></span>               | <span data-ttu-id="5f12d-p103">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="5f12d-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f12d-119">createdDateTime</span></span>      | <span data-ttu-id="5f12d-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f12d-120">dateTimeOffset</span></span>                | <span data-ttu-id="5f12d-p104">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="5f12d-123">説明</span><span class="sxs-lookup"><span data-stu-id="5f12d-123">description</span></span>          | <span data-ttu-id="5f12d-124">String</span><span class="sxs-lookup"><span data-stu-id="5f12d-124">String</span></span>                        | <span data-ttu-id="5f12d-125">ユーザーに表示されるドライブの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="5f12d-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="5f12d-126">読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="5f12d-126">Read-write.</span></span>
| <span data-ttu-id="5f12d-127">driveType</span><span class="sxs-lookup"><span data-stu-id="5f12d-127">driveType</span></span>            | <span data-ttu-id="5f12d-128">String</span><span class="sxs-lookup"><span data-stu-id="5f12d-128">String</span></span>                        | <span data-ttu-id="5f12d-p106">このリソースで表されるドライブの種類についての説明。OneDrive 個人用のドライブは `personal` を返します。OneDrive for Business は `business` を返します。SharePoint ドキュメント ライブラリは `documentLibrary` を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p106">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="5f12d-134">id</span><span class="sxs-lookup"><span data-stu-id="5f12d-134">id</span></span>                   | <span data-ttu-id="5f12d-135">String</span><span class="sxs-lookup"><span data-stu-id="5f12d-135">String</span></span>                        | <span data-ttu-id="5f12d-p107">ドライブの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p107">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="5f12d-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5f12d-138">lastModifiedBy</span></span>       | <span data-ttu-id="5f12d-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5f12d-139">[identitySet][]</span></span>               | <span data-ttu-id="5f12d-p108">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="5f12d-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f12d-142">lastModifiedDateTime</span></span> | <span data-ttu-id="5f12d-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f12d-143">dateTimeOffset</span></span>                | <span data-ttu-id="5f12d-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="5f12d-146">name</span><span class="sxs-lookup"><span data-stu-id="5f12d-146">name</span></span>                 | <span data-ttu-id="5f12d-147">文字列</span><span class="sxs-lookup"><span data-stu-id="5f12d-147">string</span></span>                        | <span data-ttu-id="5f12d-p110">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p110">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="5f12d-150">owner</span><span class="sxs-lookup"><span data-stu-id="5f12d-150">owner</span></span>                | [<span data-ttu-id="5f12d-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="5f12d-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="5f12d-p111">省略可能。ドライブを所有しているユーザー アカウント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p111">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="5f12d-155">quota</span><span class="sxs-lookup"><span data-stu-id="5f12d-155">quota</span></span>                | [<span data-ttu-id="5f12d-156">quota</span><span class="sxs-lookup"><span data-stu-id="5f12d-156">quota</span></span>](quota.md)             | <span data-ttu-id="5f12d-p112">省略可能。ドライブの記憶領域クォータに関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p112">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="5f12d-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="5f12d-160">sharepointIds</span></span>        | <span data-ttu-id="5f12d-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="5f12d-161">[sharepointIds][]</span></span>             | <span data-ttu-id="5f12d-p113">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p113">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="5f12d-164">システム</span><span class="sxs-lookup"><span data-stu-id="5f12d-164">system</span></span>               | <span data-ttu-id="5f12d-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="5f12d-165">[systemFacet][]</span></span>               | <span data-ttu-id="5f12d-166">存在する場合は、これがシステム管理のドライブであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="5f12d-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="5f12d-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-167">Read-only.</span></span>
| <span data-ttu-id="5f12d-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="5f12d-168">webUrl</span></span>               | <span data-ttu-id="5f12d-169">string (URL)</span><span class="sxs-lookup"><span data-stu-id="5f12d-169">string (url)</span></span>                  | <span data-ttu-id="5f12d-p115">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p115">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="5f12d-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5f12d-175">Relationships</span></span>

| <span data-ttu-id="5f12d-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5f12d-176">Relationship</span></span> | <span data-ttu-id="5f12d-177">型</span><span class="sxs-lookup"><span data-stu-id="5f12d-177">Type</span></span>                                 | <span data-ttu-id="5f12d-178">説明</span><span class="sxs-lookup"><span data-stu-id="5f12d-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="5f12d-179">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="5f12d-179">activities</span></span>   | <span data-ttu-id="5f12d-180">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="5f12d-180">[itemActivity][] collection</span></span>          | <span data-ttu-id="5f12d-181">このドライブに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="5f12d-181">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="5f12d-182">items</span><span class="sxs-lookup"><span data-stu-id="5f12d-182">items</span></span>        | <span data-ttu-id="5f12d-183">[driveitem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5f12d-183">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="5f12d-p116">ドライブに含まれているすべてのアイテム。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="5f12d-187">root</span><span class="sxs-lookup"><span data-stu-id="5f12d-187">root</span></span>         | [<span data-ttu-id="5f12d-188">driveitem</span><span class="sxs-lookup"><span data-stu-id="5f12d-188">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="5f12d-p117">ドライブのルート フォルダー。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="5f12d-191">special</span><span class="sxs-lookup"><span data-stu-id="5f12d-191">special</span></span>      | <span data-ttu-id="5f12d-192">[driveitem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5f12d-192">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="5f12d-p118">OneDrive で使用可能な共通フォルダーのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5f12d-p118">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="5f12d-196">次</span><span class="sxs-lookup"><span data-stu-id="5f12d-196">following</span></span>    | <span data-ttu-id="5f12d-197">[DriveItem](driveitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5f12d-197">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="5f12d-198">ユーザーは、次の項目の一覧です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-198">The list of items the user is following.</span></span> <span data-ttu-id="5f12d-199">でビジネスの OneDrive です。</span><span class="sxs-lookup"><span data-stu-id="5f12d-199">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="5f12d-200">メソッド</span><span class="sxs-lookup"><span data-stu-id="5f12d-200">Methods</span></span>

|                        <span data-ttu-id="5f12d-201">共通タスク</span><span class="sxs-lookup"><span data-stu-id="5f12d-201">Common task</span></span>                         |         <span data-ttu-id="5f12d-202">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="5f12d-202">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="5f12d-203">[別のドライブのドライブ メタデータを取得する][drive-get]</span><span class="sxs-lookup"><span data-stu-id="5f12d-203">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="5f12d-204">[ユーザーの既定のドライブのルート フォルダーを取得する][item-get]</span><span class="sxs-lookup"><span data-stu-id="5f12d-204">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="5f12d-205">[ドライブのアクティビティを一覧表示する][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="5f12d-205">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="5f12d-206">[リスト項目の後に][drive-following]</span><span class="sxs-lookup"><span data-stu-id="5f12d-206">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="5f12d-207">[ドライブの子を一覧表示する][item-children]</span><span class="sxs-lookup"><span data-stu-id="5f12d-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="5f12d-208">[ドライブ内のすべてのアイテムの変更を一覧表示する][item-changes]</span><span class="sxs-lookup"><span data-stu-id="5f12d-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="5f12d-209">[ドライブ内のアイテムを検索する][item-search]</span><span class="sxs-lookup"><span data-stu-id="5f12d-209">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="5f12d-210">特別なフォルダーにアクセスする</span><span class="sxs-lookup"><span data-stu-id="5f12d-210">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="5f12d-211">例を使用して上記の表では、 `/drive`、他のパスは有効なすぎます。</span><span class="sxs-lookup"><span data-stu-id="5f12d-211">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
