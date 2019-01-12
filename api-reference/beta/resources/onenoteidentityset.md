---
title: oneNoteIdentitySet リソースの種類
description: '**準備中のサポート**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 9043b08a8586bcc9a0043a2fde13f0d5d9eea4a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947170"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="5b885-103">oneNoteIdentitySet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b885-103">oneNoteIdentitySet resource type</span></span>

> <span data-ttu-id="5b885-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b885-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b885-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b885-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b885-106">**準備中のサポート**</span><span class="sxs-lookup"><span data-stu-id="5b885-106">**Support coming soon**</span></span>

<span data-ttu-id="5b885-107">OneNoteIdentitySet 型は、 [OneNoteIdentity](onenoteidentity.md)オブジェクトのキー付きコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5b885-107">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="5b885-108">関連付けられているさまざまなイベントの_ノートブック_、_セクション_または_ページ_の_作成者_または_最終更新者_などの id のセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="5b885-108">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="5b885-109">現在 1 つのキー、_**ユーザー**_ が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5b885-109">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="5b885-110">将来的には、デバイス、またはアイテムを変更するのにはアプリケーション キーが追加されます。</span><span class="sxs-lookup"><span data-stu-id="5b885-110">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="5b885-111">[IdentitySet](identityset.md)でこの型をマージする将来的には、</span><span class="sxs-lookup"><span data-stu-id="5b885-111">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b885-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b885-112">JSON representation</span></span>

<span data-ttu-id="5b885-113">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b885-113">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="5b885-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b885-114">Properties</span></span>
| <span data-ttu-id="5b885-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b885-115">Property</span></span>     | <span data-ttu-id="5b885-116">種類</span><span class="sxs-lookup"><span data-stu-id="5b885-116">Type</span></span>   |<span data-ttu-id="5b885-117">説明</span><span class="sxs-lookup"><span data-stu-id="5b885-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b885-118">user</span><span class="sxs-lookup"><span data-stu-id="5b885-118">user</span></span>|[<span data-ttu-id="5b885-119">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="5b885-119">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="5b885-120">OneNoteIdentity のリソースで、ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="5b885-120">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
