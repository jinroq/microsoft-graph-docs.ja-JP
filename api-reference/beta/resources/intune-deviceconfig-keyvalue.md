---
title: keyValue リソースの種類
description: キー値の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8e8028a4863ee313499f8c4982b569ca25747b3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989379"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="ff064-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff064-103">keyValue resource type</span></span>

> <span data-ttu-id="ff064-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff064-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff064-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff064-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff064-106">キー値の定義。</span><span class="sxs-lookup"><span data-stu-id="ff064-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="ff064-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff064-107">Properties</span></span>
|<span data-ttu-id="ff064-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff064-108">Property</span></span>|<span data-ttu-id="ff064-109">型</span><span class="sxs-lookup"><span data-stu-id="ff064-109">Type</span></span>|<span data-ttu-id="ff064-110">説明</span><span class="sxs-lookup"><span data-stu-id="ff064-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff064-111">Key</span><span class="sxs-lookup"><span data-stu-id="ff064-111">key</span></span>|<span data-ttu-id="ff064-112">String</span><span class="sxs-lookup"><span data-stu-id="ff064-112">String</span></span>|<span data-ttu-id="ff064-113">キー。</span><span class="sxs-lookup"><span data-stu-id="ff064-113">Key.</span></span>|
|<span data-ttu-id="ff064-114">value</span><span class="sxs-lookup"><span data-stu-id="ff064-114">value</span></span>|<span data-ttu-id="ff064-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ff064-115">String</span></span>|<span data-ttu-id="ff064-116">値。</span><span class="sxs-lookup"><span data-stu-id="ff064-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff064-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff064-117">Relationships</span></span>
<span data-ttu-id="ff064-118">なし</span><span class="sxs-lookup"><span data-stu-id="ff064-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff064-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff064-119">JSON Representation</span></span>
<span data-ttu-id="ff064-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff064-120">Here is a JSON representation of the resource.</span></span>
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





