---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a83965eb67762135eba3dcf1edf31fb4aec7827
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946729"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="747c5-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="747c5-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="747c5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="747c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="747c5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="747c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="747c5-106">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="747c5-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="747c5-107">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="747c5-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="747c5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="747c5-108">Properties</span></span>
|<span data-ttu-id="747c5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="747c5-109">Property</span></span>|<span data-ttu-id="747c5-110">型</span><span class="sxs-lookup"><span data-stu-id="747c5-110">Type</span></span>|<span data-ttu-id="747c5-111">説明</span><span class="sxs-lookup"><span data-stu-id="747c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="747c5-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="747c5-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="747c5-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="747c5-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="747c5-114">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="747c5-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="747c5-115">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="747c5-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="747c5-116">関係</span><span class="sxs-lookup"><span data-stu-id="747c5-116">Relationships</span></span>
<span data-ttu-id="747c5-117">なし</span><span class="sxs-lookup"><span data-stu-id="747c5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="747c5-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="747c5-118">JSON Representation</span></span>
<span data-ttu-id="747c5-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="747c5-119">Here is a JSON representation of the resource.</span></span>
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




