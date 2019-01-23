---
title: windows10AssociatedApps リソースの種類
description: Windows 10 関連付けられたアプリケーション定義します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5dd5b664bde2970caa4b09c027592684b9ecd5e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425919"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="da2a3-103">windows10AssociatedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="da2a3-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="da2a3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="da2a3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da2a3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da2a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da2a3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da2a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da2a3-107">Windows 10 関連付けられたアプリケーション定義します。</span><span class="sxs-lookup"><span data-stu-id="da2a3-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="da2a3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da2a3-108">Properties</span></span>
|<span data-ttu-id="da2a3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da2a3-109">Property</span></span>|<span data-ttu-id="da2a3-110">型</span><span class="sxs-lookup"><span data-stu-id="da2a3-110">Type</span></span>|<span data-ttu-id="da2a3-111">説明</span><span class="sxs-lookup"><span data-stu-id="da2a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da2a3-112">appType</span><span class="sxs-lookup"><span data-stu-id="da2a3-112">appType</span></span>|[<span data-ttu-id="da2a3-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="da2a3-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="da2a3-114">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="da2a3-114">Application type.</span></span> <span data-ttu-id="da2a3-115">使用可能な値は、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="da2a3-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="da2a3-116">識別子</span><span class="sxs-lookup"><span data-stu-id="da2a3-116">identifier</span></span>|<span data-ttu-id="da2a3-117">String</span><span class="sxs-lookup"><span data-stu-id="da2a3-117">String</span></span>|<span data-ttu-id="da2a3-118">識別子です。</span><span class="sxs-lookup"><span data-stu-id="da2a3-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da2a3-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da2a3-119">Relationships</span></span>
<span data-ttu-id="da2a3-120">なし</span><span class="sxs-lookup"><span data-stu-id="da2a3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da2a3-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da2a3-121">JSON Representation</span></span>
<span data-ttu-id="da2a3-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="da2a3-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```




