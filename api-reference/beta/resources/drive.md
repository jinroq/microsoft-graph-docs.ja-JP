---
author: JeremyKelley
ms.author: JeremyKelley
title: Drive リソース型
description: ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表すドライブ リソース
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 689c020a0c717fb395d13822c2c8de8f265988a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012724"
---
# <a name="drive-resource-type"></a><span data-ttu-id="8e3d5-103">Drive リソース型</span><span class="sxs-lookup"><span data-stu-id="8e3d5-103">drive resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e3d5-104">ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-104">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="8e3d5-p101">OneDrive のユーザーは、少なくとも 1 つのドライブ (そのユーザーの既定のドライブ) を常に使用できます。OneDrive のライセンスが付与されていないユーザーには、使用可能な既定のドライブがないことがあります。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="methods"></a><span data-ttu-id="8e3d5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8e3d5-107">Methods</span></span>

|                        <span data-ttu-id="8e3d5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8e3d5-108">Method</span></span>                              |         <span data-ttu-id="8e3d5-109">戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="8e3d5-109">Return type</span></span>         | <span data-ttu-id="8e3d5-110">説明</span><span class="sxs-lookup"><span data-stu-id="8e3d5-110">Description</span></span> |
| :--------------------------------------------------------- | :-------------------------- |-------------|
| <span data-ttu-id="8e3d5-111">[ドライブを取得する][drive-get]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-111">[Get drive][drive-get]</span></span>                                     | <span data-ttu-id="8e3d5-112">ドライブ</span><span class="sxs-lookup"><span data-stu-id="8e3d5-112">drive</span></span>                       | <span data-ttu-id="8e3d5-113">ドライブに関するメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="8e3d5-113">Get metadata about a user's default drive on OneDrive.</span></span> |
| <span data-ttu-id="8e3d5-114">[ドライブのルートを取得する][item-get]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-114">[Get drive root][item-get]</span></span>                                 | <span data-ttu-id="8e3d5-115">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-115">[driveItem][]</span></span>               | <span data-ttu-id="8e3d5-116">ドライブのルート フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="8e3d5-116">Get root folder for a drive</span></span> |
| <span data-ttu-id="8e3d5-117">[アクティビティを一覧表示する][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-117">[List activities][drive-activities]</span></span>                        | <span data-ttu-id="8e3d5-118">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-118">[itemActivity][] collection</span></span> | <span data-ttu-id="8e3d5-119">ドライブの下に発生したアクティビティを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8e3d5-119">List activities that occurred under the drive</span></span> |
| <span data-ttu-id="8e3d5-120">[フォローされたアイテムを一覧表示する][drive-following]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-120">[List followed Items][drive-following]</span></span>                     | <span data-ttu-id="8e3d5-121">[driveItem][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-121">[driveItem][] collection</span></span>    | <span data-ttu-id="8e3d5-122">ユーザーのフォローされたドライブアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8e3d5-122">List the user's followed driveItems</span></span> |
| <span data-ttu-id="8e3d5-123">[子を一覧表示する][item-children]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-123">[List children][item-children]</span></span>                             | <span data-ttu-id="8e3d5-124">[driveItem][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-124">[driveItem][] collection</span></span>    | <span data-ttu-id="8e3d5-125">ドライブのルート フォルダーの子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8e3d5-125">List children of the root folder of a drive</span></span> |
| <span data-ttu-id="8e3d5-126">[変更を一覧表示する][item-changes]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-126">[List changes][item-changes]</span></span>                               | <span data-ttu-id="8e3d5-127">[driveItem][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-127">[driveItem][] collection</span></span>    | <span data-ttu-id="8e3d5-128">ドライブ内のすべてのドライブアイテムの変更を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8e3d5-128">List changes for all Items in the Drive</span></span> |
| <span data-ttu-id="8e3d5-129">[検索][item-search]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-129">[Search][item-search]</span></span>                                      | <span data-ttu-id="8e3d5-130">[driveItem][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-130">[driveItem][] collection</span></span>    | <span data-ttu-id="8e3d5-131">ドライブでドライブアイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="8e3d5-131">Search for driveItems in a drive</span></span> |
| [<span data-ttu-id="8e3d5-132">特殊なフォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="8e3d5-132">Get special folder</span></span>](../api/drive-get-specialfolder.md)    | <span data-ttu-id="8e3d5-133">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-133">[driveItem][]</span></span>               | <span data-ttu-id="8e3d5-134">特殊なフォルダーに正規名でアクセスする</span><span class="sxs-lookup"><span data-stu-id="8e3d5-134">Access a special (named) folder in the user's OneDrive by its known name.</span></span> |


## <a name="properties"></a><span data-ttu-id="8e3d5-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e3d5-135">Properties</span></span>

| <span data-ttu-id="8e3d5-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e3d5-136">Property</span></span>             | <span data-ttu-id="8e3d5-137">型</span><span class="sxs-lookup"><span data-stu-id="8e3d5-137">Type</span></span>                          | <span data-ttu-id="8e3d5-138">説明</span><span class="sxs-lookup"><span data-stu-id="8e3d5-138">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8e3d5-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="8e3d5-139">createdBy</span></span>            | <span data-ttu-id="8e3d5-140">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-140">[identitySet][]</span></span>               | <span data-ttu-id="8e3d5-p102">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="8e3d5-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e3d5-143">createdDateTime</span></span>      | <span data-ttu-id="8e3d5-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3d5-144">dateTimeOffset</span></span>                | <span data-ttu-id="8e3d5-p103">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="8e3d5-147">説明</span><span class="sxs-lookup"><span data-stu-id="8e3d5-147">description</span></span>          | <span data-ttu-id="8e3d5-148">String</span><span class="sxs-lookup"><span data-stu-id="8e3d5-148">String</span></span>                        | <span data-ttu-id="8e3d5-149">ユーザーに表示されるドライブの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-149">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="8e3d5-150">読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-150">Read-write.</span></span>
| <span data-ttu-id="8e3d5-151">driveType</span><span class="sxs-lookup"><span data-stu-id="8e3d5-151">driveType</span></span>            | <span data-ttu-id="8e3d5-152">String</span><span class="sxs-lookup"><span data-stu-id="8e3d5-152">String</span></span>                        | <span data-ttu-id="8e3d5-p105">このリソースで表されるドライブの種類についての説明。OneDrive 個人用のドライブは `personal` を返します。OneDrive for Business は `business` を返します。SharePoint ドキュメント ライブラリは `documentLibrary` を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="8e3d5-158">id</span><span class="sxs-lookup"><span data-stu-id="8e3d5-158">id</span></span>                   | <span data-ttu-id="8e3d5-159">String</span><span class="sxs-lookup"><span data-stu-id="8e3d5-159">String</span></span>                        | <span data-ttu-id="8e3d5-p106">ドライブの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="8e3d5-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8e3d5-162">lastModifiedBy</span></span>       | <span data-ttu-id="8e3d5-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-163">[identitySet][]</span></span>               | <span data-ttu-id="8e3d5-p107">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="8e3d5-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e3d5-166">lastModifiedDateTime</span></span> | <span data-ttu-id="8e3d5-167">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3d5-167">dateTimeOffset</span></span>                | <span data-ttu-id="8e3d5-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="8e3d5-170">name</span><span class="sxs-lookup"><span data-stu-id="8e3d5-170">name</span></span>                 | <span data-ttu-id="8e3d5-171">string</span><span class="sxs-lookup"><span data-stu-id="8e3d5-171">string</span></span>                        | <span data-ttu-id="8e3d5-p109">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="8e3d5-174">owner</span><span class="sxs-lookup"><span data-stu-id="8e3d5-174">owner</span></span>                | [<span data-ttu-id="8e3d5-175">identitySet</span><span class="sxs-lookup"><span data-stu-id="8e3d5-175">identitySet</span></span>](identityset.md) | <span data-ttu-id="8e3d5-p110">省略可能。ドライブを所有しているユーザー アカウント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="8e3d5-179">quota</span><span class="sxs-lookup"><span data-stu-id="8e3d5-179">quota</span></span>                | [<span data-ttu-id="8e3d5-180">quota</span><span class="sxs-lookup"><span data-stu-id="8e3d5-180">quota</span></span>](quota.md)             | <span data-ttu-id="8e3d5-p111">省略可能。ドライブの記憶領域クォータに関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="8e3d5-184">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="8e3d5-184">sharepointIds</span></span>        | <span data-ttu-id="8e3d5-185">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-185">[sharepointIds][]</span></span>             | <span data-ttu-id="8e3d5-p112">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="8e3d5-188">system</span><span class="sxs-lookup"><span data-stu-id="8e3d5-188">system</span></span>               | <span data-ttu-id="8e3d5-189">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-189">[systemFacet][]</span></span>               | <span data-ttu-id="8e3d5-190">存在する場合は、これがシステム管理のドライブであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-190">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="8e3d5-191">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-191">Read-only.</span></span>
| <span data-ttu-id="8e3d5-192">webUrl</span><span class="sxs-lookup"><span data-stu-id="8e3d5-192">webUrl</span></span>               | <span data-ttu-id="8e3d5-193">string (URL)</span><span class="sxs-lookup"><span data-stu-id="8e3d5-193">string (url)</span></span>                  | <span data-ttu-id="8e3d5-p114">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="8e3d5-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8e3d5-199">Relationships</span></span>

| <span data-ttu-id="8e3d5-200">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8e3d5-200">Relationship</span></span> | <span data-ttu-id="8e3d5-201">型</span><span class="sxs-lookup"><span data-stu-id="8e3d5-201">Type</span></span>                                 | <span data-ttu-id="8e3d5-202">説明</span><span class="sxs-lookup"><span data-stu-id="8e3d5-202">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="8e3d5-203">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="8e3d5-203">activities</span></span>   | <span data-ttu-id="8e3d5-204">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-204">[itemActivity][] collection</span></span>          | <span data-ttu-id="8e3d5-205">このドライブに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-205">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="8e3d5-206">バンドル</span><span class="sxs-lookup"><span data-stu-id="8e3d5-206">Multiple bundles</span></span>      | <span data-ttu-id="8e3d5-207">[driveItem][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-207">[driveItem][] collection</span></span>             | <span data-ttu-id="8e3d5-208">[バンドル][bundle] のコレクション (アルバムとアイテムの複数選択共有セット)。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-208">Collection of [bundles][bundle] (albums and multi-select-shared sets of items).</span></span> <span data-ttu-id="8e3d5-209">個人用 OneDrive でのみ。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-209">Only in personal OneDrive.</span></span>
| <span data-ttu-id="8e3d5-210">フォロー中</span><span class="sxs-lookup"><span data-stu-id="8e3d5-210">following</span></span>    | <span data-ttu-id="8e3d5-211">[driveItem][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-211">[driveItem][] collection</span></span>             | <span data-ttu-id="8e3d5-212">ユーザーがフォローしているアイテムの一覧。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-212">The list of items the user is following.</span></span> <span data-ttu-id="8e3d5-213">OneDrive for Business のみ。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-213">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="8e3d5-214">items</span><span class="sxs-lookup"><span data-stu-id="8e3d5-214">items</span></span>        | <span data-ttu-id="8e3d5-215">[driveItem][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-215">[driveItem][] collection</span></span>             | <span data-ttu-id="8e3d5-p117">ドライブに含まれているすべてのアイテム。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p117">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="8e3d5-219">root</span><span class="sxs-lookup"><span data-stu-id="8e3d5-219">root</span></span>         | <span data-ttu-id="8e3d5-220">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="8e3d5-220">[driveItem][]</span></span>                        | <span data-ttu-id="8e3d5-p118">ドライブのルート フォルダー。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p118">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="8e3d5-223">special</span><span class="sxs-lookup"><span data-stu-id="8e3d5-223">special</span></span>      | <span data-ttu-id="8e3d5-224">[driveItem][] コレクション</span><span class="sxs-lookup"><span data-stu-id="8e3d5-224">[driveItem][] collection</span></span>             | <span data-ttu-id="8e3d5-p119">OneDrive で使用可能な共通フォルダーのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-p119">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8e3d5-228">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8e3d5-228">JSON representation</span></span>

<span data-ttu-id="8e3d5-229">Drive リソースの JSON 表記を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-229">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="8e3d5-230">**drive** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="8e3d5-230">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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


[bundle]: bundle.md
[driveItem]: driveItem.md
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
