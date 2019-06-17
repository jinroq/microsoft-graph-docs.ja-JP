---
title: operatingSystemVersionRange リソースの種類
description: オペレーティングシステムのバージョンの範囲。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a123c645262986711dbe28cc170443f948d2f5c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987902"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="f1c46-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1c46-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="f1c46-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1c46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1c46-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1c46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1c46-106">オペレーティングシステムのバージョンの範囲。</span><span class="sxs-lookup"><span data-stu-id="f1c46-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="f1c46-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1c46-107">Properties</span></span>
|<span data-ttu-id="f1c46-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1c46-108">Property</span></span>|<span data-ttu-id="f1c46-109">型</span><span class="sxs-lookup"><span data-stu-id="f1c46-109">Type</span></span>|<span data-ttu-id="f1c46-110">説明</span><span class="sxs-lookup"><span data-stu-id="f1c46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1c46-111">description</span><span class="sxs-lookup"><span data-stu-id="f1c46-111">description</span></span>|<span data-ttu-id="f1c46-112">String</span><span class="sxs-lookup"><span data-stu-id="f1c46-112">String</span></span>|<span data-ttu-id="f1c46-113">この範囲の説明 (例: 有効な1702ビルド)</span><span class="sxs-lookup"><span data-stu-id="f1c46-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="f1c46-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="f1c46-114">lowestVersion</span></span>|<span data-ttu-id="f1c46-115">String</span><span class="sxs-lookup"><span data-stu-id="f1c46-115">String</span></span>|<span data-ttu-id="f1c46-116">この範囲に含まれている最小の包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="f1c46-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="f1c46-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="f1c46-117">highestVersion</span></span>|<span data-ttu-id="f1c46-118">String</span><span class="sxs-lookup"><span data-stu-id="f1c46-118">String</span></span>|<span data-ttu-id="f1c46-119">この範囲に含まれている最も高い包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="f1c46-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1c46-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f1c46-120">Relationships</span></span>
<span data-ttu-id="f1c46-121">なし</span><span class="sxs-lookup"><span data-stu-id="f1c46-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1c46-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1c46-122">JSON Representation</span></span>
<span data-ttu-id="f1c46-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1c46-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





