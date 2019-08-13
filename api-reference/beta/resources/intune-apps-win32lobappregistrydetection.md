---
title: win32LobAppRegistryDetection リソースの種類
description: Win32 アプリを検出するためのレジストリプロパティが含まれています
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0fbd54fe4ed8f7df35ae6acdcde8722b98d1c24a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335551"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="955ba-103">win32LobAppRegistryDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="955ba-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="955ba-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="955ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="955ba-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="955ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="955ba-106">Win32 アプリを検出するためのレジストリプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="955ba-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="955ba-107">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="955ba-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="955ba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="955ba-108">Properties</span></span>
|<span data-ttu-id="955ba-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="955ba-109">Property</span></span>|<span data-ttu-id="955ba-110">型</span><span class="sxs-lookup"><span data-stu-id="955ba-110">Type</span></span>|<span data-ttu-id="955ba-111">説明</span><span class="sxs-lookup"><span data-stu-id="955ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="955ba-112">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="955ba-112">check32BitOn64System</span></span>|<span data-ttu-id="955ba-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="955ba-113">Boolean</span></span>|<span data-ttu-id="955ba-114">このレジストリパスが、64ビットシステムの32ビットアプリをチェックするためのものであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="955ba-114">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="955ba-115">キーパス</span><span class="sxs-lookup"><span data-stu-id="955ba-115">keyPath</span></span>|<span data-ttu-id="955ba-116">String</span><span class="sxs-lookup"><span data-stu-id="955ba-116">String</span></span>|<span data-ttu-id="955ba-117">Win32 基幹業務 (LoB) アプリを検出するためのレジストリキーのパス</span><span class="sxs-lookup"><span data-stu-id="955ba-117">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="955ba-118">valueName</span><span class="sxs-lookup"><span data-stu-id="955ba-118">valueName</span></span>|<span data-ttu-id="955ba-119">String</span><span class="sxs-lookup"><span data-stu-id="955ba-119">String</span></span>|<span data-ttu-id="955ba-120">レジストリ値の名前</span><span class="sxs-lookup"><span data-stu-id="955ba-120">The registry value name</span></span>|
|<span data-ttu-id="955ba-121">detectionType</span><span class="sxs-lookup"><span data-stu-id="955ba-121">detectionType</span></span>|[<span data-ttu-id="955ba-122">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="955ba-122">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="955ba-123">レジストリデータ検出の種類。</span><span class="sxs-lookup"><span data-stu-id="955ba-123">The registry data detection type.</span></span> <span data-ttu-id="955ba-124">使用可能な値: `notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="955ba-124">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="955ba-125">operator</span><span class="sxs-lookup"><span data-stu-id="955ba-125">operator</span></span>|[<span data-ttu-id="955ba-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="955ba-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="955ba-127">レジストリデータを検出するための演算子。</span><span class="sxs-lookup"><span data-stu-id="955ba-127">The operator for registry data detection.</span></span> <span data-ttu-id="955ba-128">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="955ba-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="955ba-129">detectionValue</span><span class="sxs-lookup"><span data-stu-id="955ba-129">detectionValue</span></span>|<span data-ttu-id="955ba-130">String</span><span class="sxs-lookup"><span data-stu-id="955ba-130">String</span></span>|<span data-ttu-id="955ba-131">レジストリの検出値</span><span class="sxs-lookup"><span data-stu-id="955ba-131">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="955ba-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="955ba-132">Relationships</span></span>
<span data-ttu-id="955ba-133">なし</span><span class="sxs-lookup"><span data-stu-id="955ba-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="955ba-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="955ba-134">JSON Representation</span></span>
<span data-ttu-id="955ba-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="955ba-135">Here is a JSON representation of the resource.</span></span>
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



