---
title: chatMessageHostedContent リソースの種類
description: チャットメッセージでホストされているコンテンツ
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2787138819160a25d72fb9ed273950eee326399c
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720951"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="dfcc8-103">chatMessageHostedContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfcc8-103">chatMessageHostedContent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfcc8-104">画像やコードスニペットなど、チャットメッセージでホストされているコンテンツを表します。</span><span class="sxs-lookup"><span data-stu-id="dfcc8-104">Represents content hosted in a chat message, such as images or code snippets.</span></span>

## <a name="methods"></a><span data-ttu-id="dfcc8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfcc8-105">Methods</span></span>

| <span data-ttu-id="dfcc8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfcc8-106">Method</span></span>       | <span data-ttu-id="dfcc8-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dfcc8-107">Return Type</span></span> | <span data-ttu-id="dfcc8-108">説明</span><span class="sxs-lookup"><span data-stu-id="dfcc8-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dfcc8-109">ChatMessageHostedContent を取得する</span><span class="sxs-lookup"><span data-stu-id="dfcc8-109">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="dfcc8-110">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="dfcc8-110">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="dfcc8-111">**ChatMessageHostedContent**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dfcc8-111">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dfcc8-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfcc8-112">Properties</span></span>

| <span data-ttu-id="dfcc8-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfcc8-113">Property</span></span>     | <span data-ttu-id="dfcc8-114">型</span><span class="sxs-lookup"><span data-stu-id="dfcc8-114">Type</span></span>        | <span data-ttu-id="dfcc8-115">説明</span><span class="sxs-lookup"><span data-stu-id="dfcc8-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dfcc8-116">id</span><span class="sxs-lookup"><span data-stu-id="dfcc8-116">id</span></span>|<span data-ttu-id="dfcc8-117">String</span><span class="sxs-lookup"><span data-stu-id="dfcc8-117">String</span></span>| <span data-ttu-id="dfcc8-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfcc8-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfcc8-119">関係</span><span class="sxs-lookup"><span data-stu-id="dfcc8-119">Relationships</span></span>

<span data-ttu-id="dfcc8-120">なし。</span><span class="sxs-lookup"><span data-stu-id="dfcc8-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfcc8-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfcc8-121">JSON representation</span></span>

<span data-ttu-id="dfcc8-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dfcc8-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
