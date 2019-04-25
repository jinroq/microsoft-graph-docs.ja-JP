---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d0a69c10f1f0075caee48276bdbc37f6d616f22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549553"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="ba78d-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba78d-103">omaSetting resource type</span></span>

> <span data-ttu-id="ba78d-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba78d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba78d-105">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="ba78d-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="ba78d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba78d-106">Properties</span></span>
|<span data-ttu-id="ba78d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba78d-107">Property</span></span>|<span data-ttu-id="ba78d-108">型</span><span class="sxs-lookup"><span data-stu-id="ba78d-108">Type</span></span>|<span data-ttu-id="ba78d-109">説明</span><span class="sxs-lookup"><span data-stu-id="ba78d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba78d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ba78d-110">displayName</span></span>|<span data-ttu-id="ba78d-111">String</span><span class="sxs-lookup"><span data-stu-id="ba78d-111">String</span></span>|<span data-ttu-id="ba78d-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="ba78d-112">Display Name.</span></span>|
|<span data-ttu-id="ba78d-113">description</span><span class="sxs-lookup"><span data-stu-id="ba78d-113">description</span></span>|<span data-ttu-id="ba78d-114">String</span><span class="sxs-lookup"><span data-stu-id="ba78d-114">String</span></span>|<span data-ttu-id="ba78d-115">説明。</span><span class="sxs-lookup"><span data-stu-id="ba78d-115">Description.</span></span>|
|<span data-ttu-id="ba78d-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="ba78d-116">omaUri</span></span>|<span data-ttu-id="ba78d-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ba78d-117">String</span></span>|<span data-ttu-id="ba78d-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="ba78d-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba78d-119">関係</span><span class="sxs-lookup"><span data-stu-id="ba78d-119">Relationships</span></span>
<span data-ttu-id="ba78d-120">なし</span><span class="sxs-lookup"><span data-stu-id="ba78d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba78d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba78d-121">JSON Representation</span></span>
<span data-ttu-id="ba78d-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba78d-122">Here is a JSON representation of the resource.</span></span>
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



