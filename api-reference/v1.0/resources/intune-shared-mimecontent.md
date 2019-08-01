---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24563bb89af91c05dd71aeb284934c0406819711
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036891"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="b90d5-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b90d5-103">mimeContent resource type</span></span>

> <span data-ttu-id="b90d5-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b90d5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b90d5-105">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b90d5-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="b90d5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b90d5-106">Properties</span></span>
|<span data-ttu-id="b90d5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b90d5-107">Property</span></span>|<span data-ttu-id="b90d5-108">型</span><span class="sxs-lookup"><span data-stu-id="b90d5-108">Type</span></span>|<span data-ttu-id="b90d5-109">説明</span><span class="sxs-lookup"><span data-stu-id="b90d5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b90d5-110">type</span><span class="sxs-lookup"><span data-stu-id="b90d5-110">type</span></span>|<span data-ttu-id="b90d5-111">String</span><span class="sxs-lookup"><span data-stu-id="b90d5-111">String</span></span>|<span data-ttu-id="b90d5-112">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="b90d5-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="b90d5-113">value</span><span class="sxs-lookup"><span data-stu-id="b90d5-113">value</span></span>|<span data-ttu-id="b90d5-114">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="b90d5-114">Binary</span></span>|<span data-ttu-id="b90d5-115">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="b90d5-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b90d5-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b90d5-116">Relationships</span></span>
<span data-ttu-id="b90d5-117">なし</span><span class="sxs-lookup"><span data-stu-id="b90d5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b90d5-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b90d5-118">JSON Representation</span></span>
<span data-ttu-id="b90d5-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b90d5-119">Here is a JSON representation of the resource.</span></span>
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



