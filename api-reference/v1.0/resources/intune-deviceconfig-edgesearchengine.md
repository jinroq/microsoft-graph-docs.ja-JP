---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6867dd6b2243541b193b8b741924487f16ff61c5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254472"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="c7a30-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7a30-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="c7a30-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7a30-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7a30-105">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="c7a30-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="c7a30-106">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c7a30-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7a30-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7a30-107">Properties</span></span>
|<span data-ttu-id="c7a30-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7a30-108">Property</span></span>|<span data-ttu-id="c7a30-109">型</span><span class="sxs-lookup"><span data-stu-id="c7a30-109">Type</span></span>|<span data-ttu-id="c7a30-110">説明</span><span class="sxs-lookup"><span data-stu-id="c7a30-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7a30-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c7a30-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="c7a30-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c7a30-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="c7a30-113">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="c7a30-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="c7a30-114">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="c7a30-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7a30-115">関係</span><span class="sxs-lookup"><span data-stu-id="c7a30-115">Relationships</span></span>
<span data-ttu-id="c7a30-116">なし</span><span class="sxs-lookup"><span data-stu-id="c7a30-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7a30-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7a30-117">JSON Representation</span></span>
<span data-ttu-id="c7a30-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7a30-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



