---
title: keyValue リソースの種類
description: キー値の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a29fcb627a1777b2fc0a4863bbab27d5fa364982
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325520"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="fef71-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fef71-103">keyValue resource type</span></span>

> <span data-ttu-id="fef71-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fef71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fef71-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fef71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fef71-106">キー値の定義。</span><span class="sxs-lookup"><span data-stu-id="fef71-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="fef71-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fef71-107">Properties</span></span>
|<span data-ttu-id="fef71-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fef71-108">Property</span></span>|<span data-ttu-id="fef71-109">型</span><span class="sxs-lookup"><span data-stu-id="fef71-109">Type</span></span>|<span data-ttu-id="fef71-110">説明</span><span class="sxs-lookup"><span data-stu-id="fef71-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fef71-111">Key</span><span class="sxs-lookup"><span data-stu-id="fef71-111">key</span></span>|<span data-ttu-id="fef71-112">String</span><span class="sxs-lookup"><span data-stu-id="fef71-112">String</span></span>|<span data-ttu-id="fef71-113">キー。</span><span class="sxs-lookup"><span data-stu-id="fef71-113">Key.</span></span>|
|<span data-ttu-id="fef71-114">value</span><span class="sxs-lookup"><span data-stu-id="fef71-114">value</span></span>|<span data-ttu-id="fef71-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fef71-115">String</span></span>|<span data-ttu-id="fef71-116">値。</span><span class="sxs-lookup"><span data-stu-id="fef71-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fef71-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fef71-117">Relationships</span></span>
<span data-ttu-id="fef71-118">なし</span><span class="sxs-lookup"><span data-stu-id="fef71-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fef71-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fef71-119">JSON Representation</span></span>
<span data-ttu-id="fef71-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fef71-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```



