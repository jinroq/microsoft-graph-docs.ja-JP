---
title: win32LobAppRegistryDetection リソースの種類
description: Win32 アプリを検出するためのレジストリプロパティが含まれています
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 076251ea185359127c3dad3610ec944f7cdb3178
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169546"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="9a818-103">win32LobAppRegistryDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a818-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="9a818-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a818-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a818-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9a818-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a818-106">Win32 アプリを検出するためのレジストリプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="9a818-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="9a818-107">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9a818-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9a818-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a818-108">Properties</span></span>
|<span data-ttu-id="9a818-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a818-109">Property</span></span>|<span data-ttu-id="9a818-110">型</span><span class="sxs-lookup"><span data-stu-id="9a818-110">Type</span></span>|<span data-ttu-id="9a818-111">説明</span><span class="sxs-lookup"><span data-stu-id="9a818-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a818-112">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="9a818-112">check32BitOn64System</span></span>|<span data-ttu-id="9a818-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="9a818-113">Boolean</span></span>|<span data-ttu-id="9a818-114">このレジストリパスが、64ビットシステムの32ビットアプリをチェックするためのものであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="9a818-114">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="9a818-115">キーパス</span><span class="sxs-lookup"><span data-stu-id="9a818-115">keyPath</span></span>|<span data-ttu-id="9a818-116">String</span><span class="sxs-lookup"><span data-stu-id="9a818-116">String</span></span>|<span data-ttu-id="9a818-117">Win32 基幹業務 (LoB) アプリを検出するためのレジストリキーのパス</span><span class="sxs-lookup"><span data-stu-id="9a818-117">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="9a818-118">valueName</span><span class="sxs-lookup"><span data-stu-id="9a818-118">valueName</span></span>|<span data-ttu-id="9a818-119">String</span><span class="sxs-lookup"><span data-stu-id="9a818-119">String</span></span>|<span data-ttu-id="9a818-120">レジストリ値の名前</span><span class="sxs-lookup"><span data-stu-id="9a818-120">The registry value name</span></span>|
|<span data-ttu-id="9a818-121">detectionType</span><span class="sxs-lookup"><span data-stu-id="9a818-121">detectionType</span></span>|[<span data-ttu-id="9a818-122">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="9a818-122">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="9a818-123">レジストリデータ検出の種類。</span><span class="sxs-lookup"><span data-stu-id="9a818-123">The registry data detection type.</span></span> <span data-ttu-id="9a818-124">使用可能な値: `notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="9a818-124">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="9a818-125">operator</span><span class="sxs-lookup"><span data-stu-id="9a818-125">operator</span></span>|[<span data-ttu-id="9a818-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="9a818-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="9a818-127">レジストリデータを検出するための演算子。</span><span class="sxs-lookup"><span data-stu-id="9a818-127">The operator for registry data detection.</span></span> <span data-ttu-id="9a818-128">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="9a818-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="9a818-129">detectionValue</span><span class="sxs-lookup"><span data-stu-id="9a818-129">detectionValue</span></span>|<span data-ttu-id="9a818-130">String</span><span class="sxs-lookup"><span data-stu-id="9a818-130">String</span></span>|<span data-ttu-id="9a818-131">レジストリの検出値</span><span class="sxs-lookup"><span data-stu-id="9a818-131">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a818-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9a818-132">Relationships</span></span>
<span data-ttu-id="9a818-133">なし</span><span class="sxs-lookup"><span data-stu-id="9a818-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a818-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a818-134">JSON Representation</span></span>
<span data-ttu-id="9a818-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9a818-135">Here is a JSON representation of the resource.</span></span>
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




