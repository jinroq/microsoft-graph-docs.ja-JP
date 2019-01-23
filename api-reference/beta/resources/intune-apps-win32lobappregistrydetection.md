---
title: win32LobAppRegistryDetection リソースの種類
description: Win32 アプリケーションを検出するためにレジストリのプロパティが含まれています
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb10a96a14d3c26503b33191fbb3c1b883245da7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402665"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="a31e4-103">win32LobAppRegistryDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a31e4-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="a31e4-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a31e4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a31e4-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a31e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a31e4-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a31e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a31e4-107">Win32 アプリケーションを検出するためにレジストリのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="a31e4-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="a31e4-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a31e4-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a31e4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a31e4-109">Properties</span></span>
|<span data-ttu-id="a31e4-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a31e4-110">Property</span></span>|<span data-ttu-id="a31e4-111">型</span><span class="sxs-lookup"><span data-stu-id="a31e4-111">Type</span></span>|<span data-ttu-id="a31e4-112">説明</span><span class="sxs-lookup"><span data-stu-id="a31e4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a31e4-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="a31e4-113">check32BitOn64System</span></span>|<span data-ttu-id="a31e4-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a31e4-114">Boolean</span></span>|<span data-ttu-id="a31e4-115">このレジストリ パスが 64 ビット システムで 32 ビット アプリケーションをチェックするかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="a31e4-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="a31e4-116">キーパス</span><span class="sxs-lookup"><span data-stu-id="a31e4-116">keyPath</span></span>|<span data-ttu-id="a31e4-117">String</span><span class="sxs-lookup"><span data-stu-id="a31e4-117">String</span></span>|<span data-ttu-id="a31e4-118">Win32 基幹業務 (LoB) アプリケーションを検出するためにレジストリ キーのパス</span><span class="sxs-lookup"><span data-stu-id="a31e4-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="a31e4-119">値名</span><span class="sxs-lookup"><span data-stu-id="a31e4-119">valueName</span></span>|<span data-ttu-id="a31e4-120">String</span><span class="sxs-lookup"><span data-stu-id="a31e4-120">String</span></span>|<span data-ttu-id="a31e4-121">レジストリ値の名前</span><span class="sxs-lookup"><span data-stu-id="a31e4-121">The registry value name</span></span>|
|<span data-ttu-id="a31e4-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="a31e4-122">detectionType</span></span>|[<span data-ttu-id="a31e4-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="a31e4-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="a31e4-124">レジストリ データの検出型です。</span><span class="sxs-lookup"><span data-stu-id="a31e4-124">The registry data detection type.</span></span> <span data-ttu-id="a31e4-125">使用可能な値: `notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="a31e4-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="a31e4-126">operator</span><span class="sxs-lookup"><span data-stu-id="a31e4-126">operator</span></span>|[<span data-ttu-id="a31e4-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="a31e4-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="a31e4-128">レジストリ データを検出するための演算子です。</span><span class="sxs-lookup"><span data-stu-id="a31e4-128">The operator for registry data detection.</span></span> <span data-ttu-id="a31e4-129">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="a31e4-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="a31e4-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="a31e4-130">detectionValue</span></span>|<span data-ttu-id="a31e4-131">String</span><span class="sxs-lookup"><span data-stu-id="a31e4-131">String</span></span>|<span data-ttu-id="a31e4-132">レジストリ検出値</span><span class="sxs-lookup"><span data-stu-id="a31e4-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="a31e4-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a31e4-133">Relationships</span></span>
<span data-ttu-id="a31e4-134">なし</span><span class="sxs-lookup"><span data-stu-id="a31e4-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a31e4-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a31e4-135">JSON Representation</span></span>
<span data-ttu-id="a31e4-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a31e4-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```




