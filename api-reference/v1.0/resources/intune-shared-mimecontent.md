---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de4360ce5a8873fde7d3286f55fc0c8993936a7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571878"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="90ec5-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90ec5-103">mimeContent resource type</span></span>

> <span data-ttu-id="90ec5-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90ec5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ec5-105">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="90ec5-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="90ec5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90ec5-106">Properties</span></span>
|<span data-ttu-id="90ec5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90ec5-107">Property</span></span>|<span data-ttu-id="90ec5-108">型</span><span class="sxs-lookup"><span data-stu-id="90ec5-108">Type</span></span>|<span data-ttu-id="90ec5-109">説明</span><span class="sxs-lookup"><span data-stu-id="90ec5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ec5-110">type</span><span class="sxs-lookup"><span data-stu-id="90ec5-110">type</span></span>|<span data-ttu-id="90ec5-111">String</span><span class="sxs-lookup"><span data-stu-id="90ec5-111">String</span></span>|<span data-ttu-id="90ec5-112">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="90ec5-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="90ec5-113">value</span><span class="sxs-lookup"><span data-stu-id="90ec5-113">value</span></span>|<span data-ttu-id="90ec5-114">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="90ec5-114">Binary</span></span>|<span data-ttu-id="90ec5-115">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="90ec5-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90ec5-116">関係</span><span class="sxs-lookup"><span data-stu-id="90ec5-116">Relationships</span></span>
<span data-ttu-id="90ec5-117">なし</span><span class="sxs-lookup"><span data-stu-id="90ec5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90ec5-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90ec5-118">JSON Representation</span></span>
<span data-ttu-id="90ec5-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="90ec5-119">Here is a JSON representation of the resource.</span></span>
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



