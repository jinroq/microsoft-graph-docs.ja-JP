---
title: omaSetting リソースの種類
description: OMA 設定の定義。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fdf74ba7e8932ce06bca83d88336239c2abcacf4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411037"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="589e5-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="589e5-103">omaSetting resource type</span></span>

> <span data-ttu-id="589e5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="589e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="589e5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="589e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="589e5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="589e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="589e5-107">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="589e5-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="589e5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="589e5-108">Properties</span></span>
|<span data-ttu-id="589e5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="589e5-109">Property</span></span>|<span data-ttu-id="589e5-110">型</span><span class="sxs-lookup"><span data-stu-id="589e5-110">Type</span></span>|<span data-ttu-id="589e5-111">説明</span><span class="sxs-lookup"><span data-stu-id="589e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="589e5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="589e5-112">displayName</span></span>|<span data-ttu-id="589e5-113">文字列</span><span class="sxs-lookup"><span data-stu-id="589e5-113">String</span></span>|<span data-ttu-id="589e5-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="589e5-114">Display Name.</span></span>|
|<span data-ttu-id="589e5-115">説明</span><span class="sxs-lookup"><span data-stu-id="589e5-115">description</span></span>|<span data-ttu-id="589e5-116">String</span><span class="sxs-lookup"><span data-stu-id="589e5-116">String</span></span>|<span data-ttu-id="589e5-117">説明。</span><span class="sxs-lookup"><span data-stu-id="589e5-117">Description.</span></span>|
|<span data-ttu-id="589e5-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="589e5-118">omaUri</span></span>|<span data-ttu-id="589e5-119">文字列</span><span class="sxs-lookup"><span data-stu-id="589e5-119">String</span></span>|<span data-ttu-id="589e5-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="589e5-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="589e5-121">関係</span><span class="sxs-lookup"><span data-stu-id="589e5-121">Relationships</span></span>
<span data-ttu-id="589e5-122">なし</span><span class="sxs-lookup"><span data-stu-id="589e5-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="589e5-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="589e5-123">JSON Representation</span></span>
<span data-ttu-id="589e5-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="589e5-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```




