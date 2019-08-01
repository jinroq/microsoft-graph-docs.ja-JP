---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5a2d2152d107050f655d43dab2cb2c65f114868
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031347"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="8f5d2-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f5d2-103">omaSetting resource type</span></span>

> <span data-ttu-id="8f5d2-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f5d2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f5d2-105">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="8f5d2-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8f5d2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f5d2-106">Properties</span></span>
|<span data-ttu-id="8f5d2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f5d2-107">Property</span></span>|<span data-ttu-id="8f5d2-108">型</span><span class="sxs-lookup"><span data-stu-id="8f5d2-108">Type</span></span>|<span data-ttu-id="8f5d2-109">説明</span><span class="sxs-lookup"><span data-stu-id="8f5d2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f5d2-110">displayName</span><span class="sxs-lookup"><span data-stu-id="8f5d2-110">displayName</span></span>|<span data-ttu-id="8f5d2-111">String</span><span class="sxs-lookup"><span data-stu-id="8f5d2-111">String</span></span>|<span data-ttu-id="8f5d2-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="8f5d2-112">Display Name.</span></span>|
|<span data-ttu-id="8f5d2-113">description</span><span class="sxs-lookup"><span data-stu-id="8f5d2-113">description</span></span>|<span data-ttu-id="8f5d2-114">String</span><span class="sxs-lookup"><span data-stu-id="8f5d2-114">String</span></span>|<span data-ttu-id="8f5d2-115">説明。</span><span class="sxs-lookup"><span data-stu-id="8f5d2-115">Description.</span></span>|
|<span data-ttu-id="8f5d2-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="8f5d2-116">omaUri</span></span>|<span data-ttu-id="8f5d2-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8f5d2-117">String</span></span>|<span data-ttu-id="8f5d2-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="8f5d2-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f5d2-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8f5d2-119">Relationships</span></span>
<span data-ttu-id="8f5d2-120">なし</span><span class="sxs-lookup"><span data-stu-id="8f5d2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f5d2-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f5d2-121">JSON Representation</span></span>
<span data-ttu-id="8f5d2-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8f5d2-122">Here is a JSON representation of the resource.</span></span>
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



