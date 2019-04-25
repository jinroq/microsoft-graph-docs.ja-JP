---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d4c232f346e9966c72bcd60e0fd08af139db068
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554437"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="3d39a-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d39a-103">omaSetting resource type</span></span>

> <span data-ttu-id="3d39a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d39a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d39a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3d39a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d39a-106">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="3d39a-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3d39a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d39a-107">Properties</span></span>
|<span data-ttu-id="3d39a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d39a-108">Property</span></span>|<span data-ttu-id="3d39a-109">型</span><span class="sxs-lookup"><span data-stu-id="3d39a-109">Type</span></span>|<span data-ttu-id="3d39a-110">説明</span><span class="sxs-lookup"><span data-stu-id="3d39a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d39a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3d39a-111">displayName</span></span>|<span data-ttu-id="3d39a-112">String</span><span class="sxs-lookup"><span data-stu-id="3d39a-112">String</span></span>|<span data-ttu-id="3d39a-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="3d39a-113">Display Name.</span></span>|
|<span data-ttu-id="3d39a-114">description</span><span class="sxs-lookup"><span data-stu-id="3d39a-114">description</span></span>|<span data-ttu-id="3d39a-115">String</span><span class="sxs-lookup"><span data-stu-id="3d39a-115">String</span></span>|<span data-ttu-id="3d39a-116">説明。</span><span class="sxs-lookup"><span data-stu-id="3d39a-116">Description.</span></span>|
|<span data-ttu-id="3d39a-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="3d39a-117">omaUri</span></span>|<span data-ttu-id="3d39a-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3d39a-118">String</span></span>|<span data-ttu-id="3d39a-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="3d39a-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d39a-120">関係</span><span class="sxs-lookup"><span data-stu-id="3d39a-120">Relationships</span></span>
<span data-ttu-id="3d39a-121">なし</span><span class="sxs-lookup"><span data-stu-id="3d39a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d39a-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d39a-122">JSON Representation</span></span>
<span data-ttu-id="3d39a-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3d39a-123">Here is a JSON representation of the resource.</span></span>
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





