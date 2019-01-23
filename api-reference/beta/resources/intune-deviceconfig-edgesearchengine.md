---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b868be9ff34e85516e34040cb3ccb6f0efb95cb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402371"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="c0c4e-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0c4e-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="c0c4e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0c4e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0c4e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0c4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0c4e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0c4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0c4e-107">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="c0c4e-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="c0c4e-108">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c0c4e-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0c4e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0c4e-109">Properties</span></span>
|<span data-ttu-id="c0c4e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0c4e-110">Property</span></span>|<span data-ttu-id="c0c4e-111">型</span><span class="sxs-lookup"><span data-stu-id="c0c4e-111">Type</span></span>|<span data-ttu-id="c0c4e-112">説明</span><span class="sxs-lookup"><span data-stu-id="c0c4e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c4e-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c0c4e-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="c0c4e-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c0c4e-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="c0c4e-115">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="c0c4e-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="c0c4e-116">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="c0c4e-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0c4e-117">関係</span><span class="sxs-lookup"><span data-stu-id="c0c4e-117">Relationships</span></span>
<span data-ttu-id="c0c4e-118">なし</span><span class="sxs-lookup"><span data-stu-id="c0c4e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0c4e-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0c4e-119">JSON Representation</span></span>
<span data-ttu-id="c0c4e-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0c4e-120">Here is a JSON representation of the resource.</span></span>
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




