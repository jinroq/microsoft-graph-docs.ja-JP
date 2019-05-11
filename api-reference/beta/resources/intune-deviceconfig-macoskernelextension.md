---
title: macOSKernelExtension リソースの種類
description: 特定の macOS カーネル拡張情報を表します。 MacOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b75288befb0f8ba7101d88d5b6f0767174469ac3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946193"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="d4746-104">macOSKernelExtension リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4746-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="d4746-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4746-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4746-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4746-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4746-107">特定の macOS カーネル拡張情報を表します。</span><span class="sxs-lookup"><span data-stu-id="d4746-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="d4746-108">MacOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。</span><span class="sxs-lookup"><span data-stu-id="d4746-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="d4746-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4746-109">Properties</span></span>
|<span data-ttu-id="d4746-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4746-110">Property</span></span>|<span data-ttu-id="d4746-111">型</span><span class="sxs-lookup"><span data-stu-id="d4746-111">Type</span></span>|<span data-ttu-id="d4746-112">説明</span><span class="sxs-lookup"><span data-stu-id="d4746-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4746-113">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="d4746-113">teamIdentifier</span></span>|<span data-ttu-id="d4746-114">String</span><span class="sxs-lookup"><span data-stu-id="d4746-114">String</span></span>|<span data-ttu-id="d4746-115">カーネル拡張機能の署名に使用されたチーム識別子。</span><span class="sxs-lookup"><span data-stu-id="d4746-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="d4746-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="d4746-116">bundleId</span></span>|<span data-ttu-id="d4746-117">String</span><span class="sxs-lookup"><span data-stu-id="d4746-117">String</span></span>|<span data-ttu-id="d4746-118">カーネル拡張機能のバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="d4746-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4746-119">関係</span><span class="sxs-lookup"><span data-stu-id="d4746-119">Relationships</span></span>
<span data-ttu-id="d4746-120">なし</span><span class="sxs-lookup"><span data-stu-id="d4746-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4746-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4746-121">JSON Representation</span></span>
<span data-ttu-id="d4746-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d4746-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```




