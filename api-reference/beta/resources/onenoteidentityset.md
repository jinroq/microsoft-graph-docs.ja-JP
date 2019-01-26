---
title: oneNoteIdentitySet リソースの種類
description: '**準備中のサポート**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: dc8256cb2459ae23fcdae9e2e658394df899a134
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577292"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="dfb2e-103">oneNoteIdentitySet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfb2e-103">oneNoteIdentitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfb2e-104">**準備中のサポート**</span><span class="sxs-lookup"><span data-stu-id="dfb2e-104">**Support coming soon**</span></span>

<span data-ttu-id="dfb2e-105">OneNoteIdentitySet 型は、 [OneNoteIdentity](onenoteidentity.md)オブジェクトのキー付きコレクションです。</span><span class="sxs-lookup"><span data-stu-id="dfb2e-105">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="dfb2e-106">関連付けられているさまざまなイベントの_ノートブック_、_セクション_または_ページ_の_作成者_または_最終更新者_などの id のセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="dfb2e-106">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="dfb2e-107">現在 1 つのキー、_**ユーザー**_ が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dfb2e-107">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="dfb2e-108">将来的には、デバイス、またはアイテムを変更するのにはアプリケーション キーが追加されます。</span><span class="sxs-lookup"><span data-stu-id="dfb2e-108">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="dfb2e-109">[IdentitySet](identityset.md)でこの型をマージする将来的には、</span><span class="sxs-lookup"><span data-stu-id="dfb2e-109">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfb2e-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfb2e-110">JSON representation</span></span>

<span data-ttu-id="dfb2e-111">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dfb2e-111">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oneNoteIdentitySet"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="dfb2e-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfb2e-112">Properties</span></span>
| <span data-ttu-id="dfb2e-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfb2e-113">Property</span></span>     | <span data-ttu-id="dfb2e-114">型</span><span class="sxs-lookup"><span data-stu-id="dfb2e-114">Type</span></span>   |<span data-ttu-id="dfb2e-115">説明</span><span class="sxs-lookup"><span data-stu-id="dfb2e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfb2e-116">user</span><span class="sxs-lookup"><span data-stu-id="dfb2e-116">user</span></span>|[<span data-ttu-id="dfb2e-117">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="dfb2e-117">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="dfb2e-118">OneNoteIdentity のリソースで、ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="dfb2e-118">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentityset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
