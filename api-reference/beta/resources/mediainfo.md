---
title: mediaInfo リソースの種類
description: プロンプトのアクションで使用されるメディア情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6a5e5677cb479839449a5e82323729b68201791a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966870"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="d973a-103">mediaInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d973a-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d973a-104">プロンプトのアクションで使用されるメディア情報。</span><span class="sxs-lookup"><span data-stu-id="d973a-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="d973a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d973a-105">Properties</span></span>
| <span data-ttu-id="d973a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d973a-106">Property</span></span>       | <span data-ttu-id="d973a-107">型</span><span class="sxs-lookup"><span data-stu-id="d973a-107">Type</span></span>    | <span data-ttu-id="d973a-108">説明</span><span class="sxs-lookup"><span data-stu-id="d973a-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="d973a-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="d973a-109">resourceId</span></span>     | <span data-ttu-id="d973a-110">String</span><span class="sxs-lookup"><span data-stu-id="d973a-110">String</span></span>  | <span data-ttu-id="d973a-111">省略可能。リソースを一意に識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d973a-111">Optional, used to uniquely identity the resource.</span></span> <span data-ttu-id="d973a-112">渡された場合、プロンプト uri はこの resourceId に対してキーとしてキャッシュされます。</span><span class="sxs-lookup"><span data-stu-id="d973a-112">If passed the prompt uri will be cached against this resourceId as key.</span></span> |
| <span data-ttu-id="d973a-113">uri</span><span class="sxs-lookup"><span data-stu-id="d973a-113">uri</span></span>            | <span data-ttu-id="d973a-114">String</span><span class="sxs-lookup"><span data-stu-id="d973a-114">String</span></span>  | <span data-ttu-id="d973a-115">再生するプロンプトへのパス。</span><span class="sxs-lookup"><span data-stu-id="d973a-115">Path to the prompt to be played.</span></span> <span data-ttu-id="d973a-116">現時点では、Wave ファイル (.wav) 形式のみで、16000 (16KHz) のサンプリングレートを持つ16ビットのサンプルのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d973a-116">Currently only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate is only supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d973a-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d973a-117">JSON representation</span></span>

<span data-ttu-id="d973a-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d973a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
