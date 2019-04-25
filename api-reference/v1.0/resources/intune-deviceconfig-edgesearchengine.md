---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6867dd6b2243541b193b8b741924487f16ff61c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565976"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="8da63-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8da63-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="8da63-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8da63-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8da63-105">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="8da63-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="8da63-106">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8da63-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8da63-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8da63-107">Properties</span></span>
|<span data-ttu-id="8da63-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8da63-108">Property</span></span>|<span data-ttu-id="8da63-109">型</span><span class="sxs-lookup"><span data-stu-id="8da63-109">Type</span></span>|<span data-ttu-id="8da63-110">説明</span><span class="sxs-lookup"><span data-stu-id="8da63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8da63-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="8da63-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="8da63-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="8da63-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="8da63-113">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="8da63-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="8da63-114">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="8da63-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8da63-115">関係</span><span class="sxs-lookup"><span data-stu-id="8da63-115">Relationships</span></span>
<span data-ttu-id="8da63-116">なし</span><span class="sxs-lookup"><span data-stu-id="8da63-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8da63-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8da63-117">JSON Representation</span></span>
<span data-ttu-id="8da63-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8da63-118">Here is a JSON representation of the resource.</span></span>
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



