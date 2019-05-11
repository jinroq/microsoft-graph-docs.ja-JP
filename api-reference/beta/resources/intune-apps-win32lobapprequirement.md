---
title: win32LobAppRequirement リソースの種類
description: Win32 アプリを検出するための基本クラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee8593603f00a06fc47540d2829ef851cc99facb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949508"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="2f748-103">win32LobAppRequirement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f748-103">win32LobAppRequirement resource type</span></span>

> <span data-ttu-id="2f748-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f748-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f748-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f748-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f748-106">Win32 アプリを検出するための基本クラス</span><span class="sxs-lookup"><span data-stu-id="2f748-106">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="2f748-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f748-107">Properties</span></span>
|<span data-ttu-id="2f748-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f748-108">Property</span></span>|<span data-ttu-id="2f748-109">型</span><span class="sxs-lookup"><span data-stu-id="2f748-109">Type</span></span>|<span data-ttu-id="2f748-110">説明</span><span class="sxs-lookup"><span data-stu-id="2f748-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f748-111">operator</span><span class="sxs-lookup"><span data-stu-id="2f748-111">operator</span></span>|[<span data-ttu-id="2f748-112">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="2f748-112">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="2f748-113">検出のための演算子。</span><span class="sxs-lookup"><span data-stu-id="2f748-113">The operator for detection.</span></span> <span data-ttu-id="2f748-114">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="2f748-114">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="2f748-115">detectionValue</span><span class="sxs-lookup"><span data-stu-id="2f748-115">detectionValue</span></span>|<span data-ttu-id="2f748-116">String</span><span class="sxs-lookup"><span data-stu-id="2f748-116">String</span></span>|<span data-ttu-id="2f748-117">検出値</span><span class="sxs-lookup"><span data-stu-id="2f748-117">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f748-118">関係</span><span class="sxs-lookup"><span data-stu-id="2f748-118">Relationships</span></span>
<span data-ttu-id="2f748-119">なし</span><span class="sxs-lookup"><span data-stu-id="2f748-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f748-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f748-120">JSON Representation</span></span>
<span data-ttu-id="2f748-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2f748-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRequirement",
  "operator": "String",
  "detectionValue": "String"
}
```




