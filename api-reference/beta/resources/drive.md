---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a01a2a8a8ad827145ee98a3ef0687546581d3096
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340659"
---
# <a name="drive-resource-type"></a><span data-ttu-id="ebb85-102">Drive リソース型</span><span class="sxs-lookup"><span data-stu-id="ebb85-102">drive resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebb85-103">ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ebb85-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="ebb85-p101">OneDrive のユーザーは、少なくとも 1 つのドライブ (そのユーザーの既定のドライブ) を常に使用できます。OneDrive のライセンスが付与されていないユーザーには、使用可能な既定のドライブがないことがあります。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebb85-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebb85-106">JSON representation</span></span>

<span data-ttu-id="ebb85-107">Drive リソースの JSON 表記を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="ebb85-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="ebb85-108">**drive** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="ebb85-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
  "items": [{"@odata.type": "microsoft.graph.driveItem"}],
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "root": {"@odata.type": "microsoft.graph.driveItem"},
  "special": [{"@odata.type": "microsoft.graph.driveItem"}],
  "system": {"@odata.type": "microsoft.graph.systemFacet"},
  "webUrl": "string",
  "sharepointIds": {"@odata.type": "microsoft.graph.sharepointIds"}
}
```

## <a name="properties"></a><span data-ttu-id="ebb85-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebb85-109">Properties</span></span>

| <span data-ttu-id="ebb85-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebb85-110">Property</span></span>             | <span data-ttu-id="ebb85-111">型</span><span class="sxs-lookup"><span data-stu-id="ebb85-111">Type</span></span>                          | <span data-ttu-id="ebb85-112">説明</span><span class="sxs-lookup"><span data-stu-id="ebb85-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ebb85-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="ebb85-113">createdBy</span></span>            | <span data-ttu-id="ebb85-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ebb85-114">[identitySet][]</span></span>               | <span data-ttu-id="ebb85-p102">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="ebb85-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebb85-117">createdDateTime</span></span>      | <span data-ttu-id="ebb85-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebb85-118">dateTimeOffset</span></span>                | <span data-ttu-id="ebb85-p103">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="ebb85-121">説明</span><span class="sxs-lookup"><span data-stu-id="ebb85-121">description</span></span>          | <span data-ttu-id="ebb85-122">String</span><span class="sxs-lookup"><span data-stu-id="ebb85-122">String</span></span>                        | <span data-ttu-id="ebb85-123">ユーザーに表示されるドライブの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="ebb85-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="ebb85-124">読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ebb85-124">Read-write.</span></span>
| <span data-ttu-id="ebb85-125">driveType</span><span class="sxs-lookup"><span data-stu-id="ebb85-125">driveType</span></span>            | <span data-ttu-id="ebb85-126">String</span><span class="sxs-lookup"><span data-stu-id="ebb85-126">String</span></span>                        | <span data-ttu-id="ebb85-p105">このリソースで表されるドライブの種類についての説明。OneDrive 個人用のドライブは `personal` を返します。OneDrive for Business は `business` を返します。SharePoint ドキュメント ライブラリは `documentLibrary` を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="ebb85-132">id</span><span class="sxs-lookup"><span data-stu-id="ebb85-132">id</span></span>                   | <span data-ttu-id="ebb85-133">String</span><span class="sxs-lookup"><span data-stu-id="ebb85-133">String</span></span>                        | <span data-ttu-id="ebb85-p106">ドライブの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="ebb85-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ebb85-136">lastModifiedBy</span></span>       | <span data-ttu-id="ebb85-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ebb85-137">[identitySet][]</span></span>               | <span data-ttu-id="ebb85-p107">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="ebb85-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebb85-140">lastModifiedDateTime</span></span> | <span data-ttu-id="ebb85-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebb85-141">dateTimeOffset</span></span>                | <span data-ttu-id="ebb85-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="ebb85-144">name</span><span class="sxs-lookup"><span data-stu-id="ebb85-144">name</span></span>                 | <span data-ttu-id="ebb85-145">string</span><span class="sxs-lookup"><span data-stu-id="ebb85-145">string</span></span>                        | <span data-ttu-id="ebb85-p109">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="ebb85-148">owner</span><span class="sxs-lookup"><span data-stu-id="ebb85-148">owner</span></span>                | [<span data-ttu-id="ebb85-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="ebb85-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="ebb85-p110">省略可能。ドライブを所有しているユーザー アカウント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="ebb85-153">quota</span><span class="sxs-lookup"><span data-stu-id="ebb85-153">quota</span></span>                | [<span data-ttu-id="ebb85-154">quota</span><span class="sxs-lookup"><span data-stu-id="ebb85-154">quota</span></span>](quota.md)             | <span data-ttu-id="ebb85-p111">省略可能。ドライブの記憶領域クォータに関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="ebb85-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ebb85-158">sharepointIds</span></span>        | <span data-ttu-id="ebb85-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ebb85-159">[sharepointIds][]</span></span>             | <span data-ttu-id="ebb85-p112">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="ebb85-162">system</span><span class="sxs-lookup"><span data-stu-id="ebb85-162">system</span></span>               | <span data-ttu-id="ebb85-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="ebb85-163">[systemFacet][]</span></span>               | <span data-ttu-id="ebb85-164">存在する場合は、これがシステム管理のドライブであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="ebb85-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="ebb85-165">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-165">Read-only.</span></span>
| <span data-ttu-id="ebb85-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="ebb85-166">webUrl</span></span>               | <span data-ttu-id="ebb85-167">string (URL)</span><span class="sxs-lookup"><span data-stu-id="ebb85-167">string (url)</span></span>                  | <span data-ttu-id="ebb85-p114">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="ebb85-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ebb85-173">Relationships</span></span>

| <span data-ttu-id="ebb85-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ebb85-174">Relationship</span></span> | <span data-ttu-id="ebb85-175">型</span><span class="sxs-lookup"><span data-stu-id="ebb85-175">Type</span></span>                                 | <span data-ttu-id="ebb85-176">説明</span><span class="sxs-lookup"><span data-stu-id="ebb85-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="ebb85-177">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="ebb85-177">activities</span></span>   | <span data-ttu-id="ebb85-178">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ebb85-178">[itemActivity][] collection</span></span>          | <span data-ttu-id="ebb85-179">このドライブに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="ebb85-179">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="ebb85-180">items</span><span class="sxs-lookup"><span data-stu-id="ebb85-180">items</span></span>        | <span data-ttu-id="ebb85-181">[driveItem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebb85-181">[driveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ebb85-p115">ドライブに含まれているすべてのアイテム。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="ebb85-185">root</span><span class="sxs-lookup"><span data-stu-id="ebb85-185">root</span></span>         | [<span data-ttu-id="ebb85-186">driveItem</span><span class="sxs-lookup"><span data-stu-id="ebb85-186">driveItem</span></span>](driveitem.md)            | <span data-ttu-id="ebb85-p116">ドライブのルート フォルダー。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="ebb85-189">special</span><span class="sxs-lookup"><span data-stu-id="ebb85-189">special</span></span>      | <span data-ttu-id="ebb85-190">[driveItem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebb85-190">[driveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ebb85-p117">OneDrive で使用可能な共通フォルダーのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ebb85-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="ebb85-194">フォロー中</span><span class="sxs-lookup"><span data-stu-id="ebb85-194">following</span></span>    | <span data-ttu-id="ebb85-195">[driveItem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebb85-195">[driveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ebb85-196">ユーザーがフォローしているアイテムの一覧。</span><span class="sxs-lookup"><span data-stu-id="ebb85-196">The list of items the user is following.</span></span> <span data-ttu-id="ebb85-197">OneDrive for Business のみ。</span><span class="sxs-lookup"><span data-stu-id="ebb85-197">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="ebb85-198">メソッド</span><span class="sxs-lookup"><span data-stu-id="ebb85-198">Methods</span></span>

|                        <span data-ttu-id="ebb85-199">共通タスク</span><span class="sxs-lookup"><span data-stu-id="ebb85-199">Common task</span></span>                         |         <span data-ttu-id="ebb85-200">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="ebb85-200">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="ebb85-201">[別の Drive の Drive メタデータを取得する][drive-get]</span><span class="sxs-lookup"><span data-stu-id="ebb85-201">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="ebb85-202">[ユーザーの既定のドライブのルート フォルダーを取得する][item-get]</span><span class="sxs-lookup"><span data-stu-id="ebb85-202">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="ebb85-203">[ドライブのアクティビティを一覧表示する][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="ebb85-203">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="ebb85-204">[フォローされたアイテムを一覧表示する][drive-following]</span><span class="sxs-lookup"><span data-stu-id="ebb85-204">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="ebb85-205">[ドライブの子を一覧表示する][item-children]</span><span class="sxs-lookup"><span data-stu-id="ebb85-205">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="ebb85-206">[ドライブ内のすべてのアイテムの変更を一覧表示する][item-changes]</span><span class="sxs-lookup"><span data-stu-id="ebb85-206">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="ebb85-207">[ドライブ内のアイテムを検索する][item-search]</span><span class="sxs-lookup"><span data-stu-id="ebb85-207">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="ebb85-208">特別なフォルダーにアクセスする</span><span class="sxs-lookup"><span data-stu-id="ebb85-208">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="ebb85-209">前の表では例に `/drive` を使用していますが、他のパスも有効です。</span><span class="sxs-lookup"><span data-stu-id="ebb85-209">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive": "#"
  },
  "suppressions": []
}
-->
