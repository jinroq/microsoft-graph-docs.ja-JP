---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c595256953928138ec140b799410f5ba43d0b3de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950971"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="6935f-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6935f-103">omaSetting resource type</span></span>

> <span data-ttu-id="6935f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6935f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6935f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6935f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6935f-106">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="6935f-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="6935f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6935f-107">Properties</span></span>
|<span data-ttu-id="6935f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6935f-108">Property</span></span>|<span data-ttu-id="6935f-109">型</span><span class="sxs-lookup"><span data-stu-id="6935f-109">Type</span></span>|<span data-ttu-id="6935f-110">説明</span><span class="sxs-lookup"><span data-stu-id="6935f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6935f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6935f-111">displayName</span></span>|<span data-ttu-id="6935f-112">String</span><span class="sxs-lookup"><span data-stu-id="6935f-112">String</span></span>|<span data-ttu-id="6935f-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="6935f-113">Display Name.</span></span>|
|<span data-ttu-id="6935f-114">description</span><span class="sxs-lookup"><span data-stu-id="6935f-114">description</span></span>|<span data-ttu-id="6935f-115">String</span><span class="sxs-lookup"><span data-stu-id="6935f-115">String</span></span>|<span data-ttu-id="6935f-116">説明。</span><span class="sxs-lookup"><span data-stu-id="6935f-116">Description.</span></span>|
|<span data-ttu-id="6935f-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="6935f-117">omaUri</span></span>|<span data-ttu-id="6935f-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6935f-118">String</span></span>|<span data-ttu-id="6935f-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="6935f-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6935f-120">関係</span><span class="sxs-lookup"><span data-stu-id="6935f-120">Relationships</span></span>
<span data-ttu-id="6935f-121">なし</span><span class="sxs-lookup"><span data-stu-id="6935f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6935f-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6935f-122">JSON Representation</span></span>
<span data-ttu-id="6935f-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6935f-123">Here is a JSON representation of the resource.</span></span>
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




