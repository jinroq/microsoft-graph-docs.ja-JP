---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f2224d255e8aa4ceb48554fdc01356277ffbc89
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939117"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="e5547-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5547-103">mimeContent resource type</span></span>

> <span data-ttu-id="e5547-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5547-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5547-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5547-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5547-106">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e5547-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="e5547-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5547-107">Properties</span></span>
|<span data-ttu-id="e5547-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5547-108">Property</span></span>|<span data-ttu-id="e5547-109">種類</span><span class="sxs-lookup"><span data-stu-id="e5547-109">Type</span></span>|<span data-ttu-id="e5547-110">説明</span><span class="sxs-lookup"><span data-stu-id="e5547-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5547-111">type</span><span class="sxs-lookup"><span data-stu-id="e5547-111">type</span></span>|<span data-ttu-id="e5547-112">String</span><span class="sxs-lookup"><span data-stu-id="e5547-112">String</span></span>|<span data-ttu-id="e5547-113">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="e5547-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="e5547-114">value</span><span class="sxs-lookup"><span data-stu-id="e5547-114">value</span></span>|<span data-ttu-id="e5547-115">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="e5547-115">Binary</span></span>|<span data-ttu-id="e5547-116">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="e5547-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5547-117">関係</span><span class="sxs-lookup"><span data-stu-id="e5547-117">Relationships</span></span>
<span data-ttu-id="e5547-118">なし</span><span class="sxs-lookup"><span data-stu-id="e5547-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5547-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5547-119">JSON Representation</span></span>
<span data-ttu-id="e5547-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5547-120">Here is a JSON representation of the resource.</span></span>
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




