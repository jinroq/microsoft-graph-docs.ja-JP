---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bb5df5f786eefc1b7b7159b1643f9d3d46d8300
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958705"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="1077d-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1077d-103">omaSetting resource type</span></span>

> <span data-ttu-id="1077d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1077d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1077d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1077d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1077d-106">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="1077d-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1077d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1077d-107">Properties</span></span>
|<span data-ttu-id="1077d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1077d-108">Property</span></span>|<span data-ttu-id="1077d-109">型</span><span class="sxs-lookup"><span data-stu-id="1077d-109">Type</span></span>|<span data-ttu-id="1077d-110">説明</span><span class="sxs-lookup"><span data-stu-id="1077d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1077d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1077d-111">displayName</span></span>|<span data-ttu-id="1077d-112">String</span><span class="sxs-lookup"><span data-stu-id="1077d-112">String</span></span>|<span data-ttu-id="1077d-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="1077d-113">Display Name.</span></span>|
|<span data-ttu-id="1077d-114">description</span><span class="sxs-lookup"><span data-stu-id="1077d-114">description</span></span>|<span data-ttu-id="1077d-115">String</span><span class="sxs-lookup"><span data-stu-id="1077d-115">String</span></span>|<span data-ttu-id="1077d-116">説明。</span><span class="sxs-lookup"><span data-stu-id="1077d-116">Description.</span></span>|
|<span data-ttu-id="1077d-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="1077d-117">omaUri</span></span>|<span data-ttu-id="1077d-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1077d-118">String</span></span>|<span data-ttu-id="1077d-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="1077d-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1077d-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1077d-120">Relationships</span></span>
<span data-ttu-id="1077d-121">なし</span><span class="sxs-lookup"><span data-stu-id="1077d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1077d-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1077d-122">JSON Representation</span></span>
<span data-ttu-id="1077d-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1077d-123">Here is a JSON representation of the resource.</span></span>
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





