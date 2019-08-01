---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d733abca0dd390e83e51b25afd1ba7e86886b3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028379"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="15919-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15919-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="15919-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15919-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15919-105">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="15919-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="15919-106">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="15919-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="15919-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15919-107">Properties</span></span>
|<span data-ttu-id="15919-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15919-108">Property</span></span>|<span data-ttu-id="15919-109">型</span><span class="sxs-lookup"><span data-stu-id="15919-109">Type</span></span>|<span data-ttu-id="15919-110">説明</span><span class="sxs-lookup"><span data-stu-id="15919-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15919-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="15919-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="15919-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="15919-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="15919-113">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="15919-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="15919-114">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="15919-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15919-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15919-115">Relationships</span></span>
<span data-ttu-id="15919-116">なし</span><span class="sxs-lookup"><span data-stu-id="15919-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15919-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15919-117">JSON Representation</span></span>
<span data-ttu-id="15919-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15919-118">Here is a JSON representation of the resource.</span></span>
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



