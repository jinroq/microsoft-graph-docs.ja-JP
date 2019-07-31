---
title: oneNoteIdentitySet リソースの種類
description: '**まもなくサポートが提供される**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 9ffbc20a73aaed885d118094a7d1946459eb7efc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009364"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="6db9f-103">oneNoteIdentitySet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6db9f-103">oneNoteIdentitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6db9f-104">**まもなくサポートが提供される**</span><span class="sxs-lookup"><span data-stu-id="6db9f-104">**Support coming soon**</span></span>

<span data-ttu-id="6db9f-105">OneNoteIdentitySet 型は、 [OneNoteIdentity](onenoteidentity.md)オブジェクトのキー付きコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6db9f-105">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="6db9f-106">_作成者_または_最終更新者_など、_ノートブック_、_セクション_、または_ページ_のさまざまなイベントに関連付けられている id のセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="6db9f-106">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="6db9f-107">現在、1つのキーの_**ユーザー**_ が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6db9f-107">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="6db9f-108">その後、アイテムを変更するためのデバイスやアプリケーションなどのキーが追加されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6db9f-108">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="6db9f-109">後で、この型は、identity [set](identityset.md)と統合されます。</span><span class="sxs-lookup"><span data-stu-id="6db9f-109">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="6db9f-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6db9f-110">JSON representation</span></span>

<span data-ttu-id="6db9f-111">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6db9f-111">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.onenoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="6db9f-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6db9f-112">Properties</span></span>
| <span data-ttu-id="6db9f-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6db9f-113">Property</span></span>     | <span data-ttu-id="6db9f-114">型</span><span class="sxs-lookup"><span data-stu-id="6db9f-114">Type</span></span>   |<span data-ttu-id="6db9f-115">説明</span><span class="sxs-lookup"><span data-stu-id="6db9f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6db9f-116">user</span><span class="sxs-lookup"><span data-stu-id="6db9f-116">user</span></span>|[<span data-ttu-id="6db9f-117">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="6db9f-117">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="6db9f-118">ユーザーを表す OneNoteIdentity リソース。</span><span class="sxs-lookup"><span data-stu-id="6db9f-118">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
