---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
ms.openlocfilehash: 0b178967f7eb8da8bdf8584bb13a7d4f9950392b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="drive-resource-type"></a><span data-ttu-id="fab8c-102">Drive リソース型</span><span class="sxs-lookup"><span data-stu-id="fab8c-102">Drive resource type</span></span>

<span data-ttu-id="fab8c-103">ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fab8c-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="fab8c-p101">OneDrive のユーザーは、少なくとも 1 つのドライブ (そのユーザーの既定のドライブ) を常に使用できます。OneDrive のライセンスが付与されていないユーザーには、使用可能な既定のドライブがないことがあります。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fab8c-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fab8c-106">JSON representation</span></span>

<span data-ttu-id="fab8c-107">Drive リソースの JSON 表記を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="fab8c-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="fab8c-108">**drive** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="fab8c-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.drive",
       "keyProperty": "id", 
       "optionalProperties": [ "activities", "createdBy", "createdDateTime", "description", "lastModifiedBy", "lastModifiedDateTime", "name", "webUrl", "items", "root", "special", "system"] } -->

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
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="fab8c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fab8c-109">Properties</span></span>

| <span data-ttu-id="fab8c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fab8c-110">Property</span></span>             | <span data-ttu-id="fab8c-111">型</span><span class="sxs-lookup"><span data-stu-id="fab8c-111">Type</span></span>                          | <span data-ttu-id="fab8c-112">説明</span><span class="sxs-lookup"><span data-stu-id="fab8c-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fab8c-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="fab8c-113">createdBy</span></span>            | <span data-ttu-id="fab8c-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="fab8c-114">[identitySet][]</span></span>               | <span data-ttu-id="fab8c-p102">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="fab8c-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fab8c-117">createdDateTime</span></span>      | <span data-ttu-id="fab8c-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fab8c-118">dateTimeOffset</span></span>                | <span data-ttu-id="fab8c-p103">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="fab8c-121">説明</span><span class="sxs-lookup"><span data-stu-id="fab8c-121">description</span></span>          | <span data-ttu-id="fab8c-122">String</span><span class="sxs-lookup"><span data-stu-id="fab8c-122">String</span></span>                        | <span data-ttu-id="fab8c-123">ユーザーに表示されるドライブの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="fab8c-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="fab8c-124">読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="fab8c-124">Read-write.</span></span>
| <span data-ttu-id="fab8c-125">driveType</span><span class="sxs-lookup"><span data-stu-id="fab8c-125">driveType</span></span>            | <span data-ttu-id="fab8c-126">String</span><span class="sxs-lookup"><span data-stu-id="fab8c-126">String</span></span>                        | <span data-ttu-id="fab8c-p105">このリソースで表されるドライブの種類についての説明。OneDrive 個人用のドライブは `personal` を返します。OneDrive for Business は `business` を返します。SharePoint ドキュメント ライブラリは `documentLibrary` を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="fab8c-132">id</span><span class="sxs-lookup"><span data-stu-id="fab8c-132">id</span></span>                   | <span data-ttu-id="fab8c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="fab8c-133">String</span></span>                        | <span data-ttu-id="fab8c-p106">ドライブの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="fab8c-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="fab8c-136">lastModifiedBy</span></span>       | <span data-ttu-id="fab8c-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="fab8c-137">[identitySet][]</span></span>               | <span data-ttu-id="fab8c-p107">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="fab8c-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fab8c-140">lastModifiedDateTime</span></span> | <span data-ttu-id="fab8c-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fab8c-141">dateTimeOffset</span></span>                | <span data-ttu-id="fab8c-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="fab8c-144">name</span><span class="sxs-lookup"><span data-stu-id="fab8c-144">name</span></span>                 | <span data-ttu-id="fab8c-145">string</span><span class="sxs-lookup"><span data-stu-id="fab8c-145">string</span></span>                        | <span data-ttu-id="fab8c-p109">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="fab8c-148">owner</span><span class="sxs-lookup"><span data-stu-id="fab8c-148">owner</span></span>                | [<span data-ttu-id="fab8c-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="fab8c-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="fab8c-p110">省略可能。ドライブを所有しているユーザー アカウント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="fab8c-153">quota</span><span class="sxs-lookup"><span data-stu-id="fab8c-153">quota</span></span>                | [<span data-ttu-id="fab8c-154">quota</span><span class="sxs-lookup"><span data-stu-id="fab8c-154">quota</span></span>](quota.md)             | <span data-ttu-id="fab8c-p111">省略可能。ドライブの記憶領域クォータに関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="fab8c-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="fab8c-158">sharepointIds</span></span>        | <span data-ttu-id="fab8c-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="fab8c-159">[sharepointIds][]</span></span>             | <span data-ttu-id="fab8c-p112">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="fab8c-162">system</span><span class="sxs-lookup"><span data-stu-id="fab8c-162">System</span></span>               | <span data-ttu-id="fab8c-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="fab8c-163">[systemFacet][]</span></span>               | <span data-ttu-id="fab8c-164">存在する場合は、これがシステム管理のドライブであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="fab8c-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="fab8c-165">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-165">Read-only.</span></span>
| <span data-ttu-id="fab8c-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="fab8c-166">webUrl</span></span>               | <span data-ttu-id="fab8c-167">string (URL)</span><span class="sxs-lookup"><span data-stu-id="fab8c-167">string (url)</span></span>                  | <span data-ttu-id="fab8c-p114">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="fab8c-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fab8c-173">Relationships</span></span>

| <span data-ttu-id="fab8c-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fab8c-174">Relationship</span></span> | <span data-ttu-id="fab8c-175">型</span><span class="sxs-lookup"><span data-stu-id="fab8c-175">Type</span></span>                                 | <span data-ttu-id="fab8c-176">説明</span><span class="sxs-lookup"><span data-stu-id="fab8c-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="fab8c-177">items</span><span class="sxs-lookup"><span data-stu-id="fab8c-177">items</span></span>        | <span data-ttu-id="fab8c-178">[driveitem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fab8c-178">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="fab8c-p115">ドライブに含まれているすべてのアイテム。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="fab8c-182">root</span><span class="sxs-lookup"><span data-stu-id="fab8c-182">root</span></span>         | [<span data-ttu-id="fab8c-183">driveitem</span><span class="sxs-lookup"><span data-stu-id="fab8c-183">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="fab8c-p116">ドライブのルート フォルダー。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="fab8c-186">special</span><span class="sxs-lookup"><span data-stu-id="fab8c-186">special</span></span>      | <span data-ttu-id="fab8c-187">[driveitem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fab8c-187">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="fab8c-p117">OneDrive で使用可能な共通フォルダーのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="fab8c-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="fab8c-191">メソッド</span><span class="sxs-lookup"><span data-stu-id="fab8c-191">Methods</span></span>

|                        <span data-ttu-id="fab8c-192">共通タスク</span><span class="sxs-lookup"><span data-stu-id="fab8c-192">Common task</span></span>                         |         <span data-ttu-id="fab8c-193">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="fab8c-193">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="fab8c-194">[別の Drive の Drive メタデータを取得する][drive-get]</span><span class="sxs-lookup"><span data-stu-id="fab8c-194">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="fab8c-195">[ユーザーの既定のドライブのルート フォルダーを取得する][item-get]</span><span class="sxs-lookup"><span data-stu-id="fab8c-195">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="fab8c-196">[ドライブの子を一覧表示する][item-children]</span><span class="sxs-lookup"><span data-stu-id="fab8c-196">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="fab8c-197">[ドライブ内のすべてのアイテムの変更を一覧表示する][item-changes]</span><span class="sxs-lookup"><span data-stu-id="fab8c-197">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="fab8c-198">[ドライブ内のアイテムを検索する][item-search]</span><span class="sxs-lookup"><span data-stu-id="fab8c-198">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="fab8c-199">特殊フォルダーにアクセスする</span><span class="sxs-lookup"><span data-stu-id="fab8c-199">Access special folder</span></span>](../api/drive_get_specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="fab8c-200">前の表では例に `/drive` を使用していますが、他のパスも有効です。</span><span class="sxs-lookup"><span data-stu-id="fab8c-200">In the previous table, the examples use , but  is valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive_get.md
[item-get]: ../api/driveitem_get.md
[item-changes]: ../api/driveitem_delta.md
[item-search]: ../api/driveitem_search.md
[item-children]: ../api/driveitem_list_children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
