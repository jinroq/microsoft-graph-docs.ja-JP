---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de4360ce5a8873fde7d3286f55fc0c8993936a7c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260005"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="aa246-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa246-103">mimeContent resource type</span></span>

> <span data-ttu-id="aa246-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa246-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa246-105">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="aa246-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="aa246-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa246-106">Properties</span></span>
|<span data-ttu-id="aa246-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa246-107">Property</span></span>|<span data-ttu-id="aa246-108">型</span><span class="sxs-lookup"><span data-stu-id="aa246-108">Type</span></span>|<span data-ttu-id="aa246-109">説明</span><span class="sxs-lookup"><span data-stu-id="aa246-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa246-110">type</span><span class="sxs-lookup"><span data-stu-id="aa246-110">type</span></span>|<span data-ttu-id="aa246-111">String</span><span class="sxs-lookup"><span data-stu-id="aa246-111">String</span></span>|<span data-ttu-id="aa246-112">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="aa246-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="aa246-113">value</span><span class="sxs-lookup"><span data-stu-id="aa246-113">value</span></span>|<span data-ttu-id="aa246-114">バイナリ</span><span class="sxs-lookup"><span data-stu-id="aa246-114">Binary</span></span>|<span data-ttu-id="aa246-115">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="aa246-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa246-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aa246-116">Relationships</span></span>
<span data-ttu-id="aa246-117">なし</span><span class="sxs-lookup"><span data-stu-id="aa246-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa246-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa246-118">JSON Representation</span></span>
<span data-ttu-id="aa246-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aa246-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



