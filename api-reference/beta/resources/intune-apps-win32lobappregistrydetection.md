---
title: win32LobAppRegistryDetection リソースの種類
description: Win32 アプリを検出するためのレジストリプロパティが含まれています
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4cd9ce4223d18d001ca1d299f8dbcae31c6f99d2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949529"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="fd30f-103">win32LobAppRegistryDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd30f-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="fd30f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd30f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd30f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fd30f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd30f-106">Win32 アプリを検出するためのレジストリプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="fd30f-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="fd30f-107">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="fd30f-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd30f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd30f-108">Properties</span></span>
|<span data-ttu-id="fd30f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd30f-109">Property</span></span>|<span data-ttu-id="fd30f-110">型</span><span class="sxs-lookup"><span data-stu-id="fd30f-110">Type</span></span>|<span data-ttu-id="fd30f-111">説明</span><span class="sxs-lookup"><span data-stu-id="fd30f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd30f-112">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="fd30f-112">check32BitOn64System</span></span>|<span data-ttu-id="fd30f-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd30f-113">Boolean</span></span>|<span data-ttu-id="fd30f-114">このレジストリパスが、64ビットシステムの32ビットアプリをチェックするためのものであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="fd30f-114">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="fd30f-115">キーパス</span><span class="sxs-lookup"><span data-stu-id="fd30f-115">keyPath</span></span>|<span data-ttu-id="fd30f-116">String</span><span class="sxs-lookup"><span data-stu-id="fd30f-116">String</span></span>|<span data-ttu-id="fd30f-117">Win32 基幹業務 (LoB) アプリを検出するためのレジストリキーのパス</span><span class="sxs-lookup"><span data-stu-id="fd30f-117">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="fd30f-118">valueName</span><span class="sxs-lookup"><span data-stu-id="fd30f-118">valueName</span></span>|<span data-ttu-id="fd30f-119">String</span><span class="sxs-lookup"><span data-stu-id="fd30f-119">String</span></span>|<span data-ttu-id="fd30f-120">レジストリ値の名前</span><span class="sxs-lookup"><span data-stu-id="fd30f-120">The registry value name</span></span>|
|<span data-ttu-id="fd30f-121">detectionType</span><span class="sxs-lookup"><span data-stu-id="fd30f-121">detectionType</span></span>|[<span data-ttu-id="fd30f-122">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="fd30f-122">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="fd30f-123">レジストリデータ検出の種類。</span><span class="sxs-lookup"><span data-stu-id="fd30f-123">The registry data detection type.</span></span> <span data-ttu-id="fd30f-124">使用可能な値: `notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="fd30f-124">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="fd30f-125">operator</span><span class="sxs-lookup"><span data-stu-id="fd30f-125">operator</span></span>|[<span data-ttu-id="fd30f-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="fd30f-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="fd30f-127">レジストリデータを検出するための演算子。</span><span class="sxs-lookup"><span data-stu-id="fd30f-127">The operator for registry data detection.</span></span> <span data-ttu-id="fd30f-128">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="fd30f-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="fd30f-129">detectionValue</span><span class="sxs-lookup"><span data-stu-id="fd30f-129">detectionValue</span></span>|<span data-ttu-id="fd30f-130">String</span><span class="sxs-lookup"><span data-stu-id="fd30f-130">String</span></span>|<span data-ttu-id="fd30f-131">レジストリの検出値</span><span class="sxs-lookup"><span data-stu-id="fd30f-131">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd30f-132">関係</span><span class="sxs-lookup"><span data-stu-id="fd30f-132">Relationships</span></span>
<span data-ttu-id="fd30f-133">なし</span><span class="sxs-lookup"><span data-stu-id="fd30f-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd30f-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd30f-134">JSON Representation</span></span>
<span data-ttu-id="fd30f-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fd30f-135">Here is a JSON representation of the resource.</span></span>
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




