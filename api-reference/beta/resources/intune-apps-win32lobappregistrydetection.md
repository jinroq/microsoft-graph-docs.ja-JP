---
title: win32LobAppRegistryDetection リソースの種類
description: Win32 アプリケーションを検出するためにレジストリのプロパティが含まれています
author: tfitzmac
ms.openlocfilehash: 5adeca1b569531d15657acc2a8960bab60580dc6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347741"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="52fa8-103">win32LobAppRegistryDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52fa8-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="52fa8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="52fa8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52fa8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52fa8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52fa8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="52fa8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52fa8-107">Win32 アプリケーションを検出するためにレジストリのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="52fa8-107">Contains registry properties to detect a Win32 App</span></span>

<span data-ttu-id="52fa8-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="52fa8-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52fa8-109">Properties</span><span class="sxs-lookup"><span data-stu-id="52fa8-109">Properties</span></span>
|<span data-ttu-id="52fa8-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52fa8-110">Property</span></span>|<span data-ttu-id="52fa8-111">種類</span><span class="sxs-lookup"><span data-stu-id="52fa8-111">Type</span></span>|<span data-ttu-id="52fa8-112">説明</span><span class="sxs-lookup"><span data-stu-id="52fa8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52fa8-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="52fa8-113">check32BitOn64System</span></span>|<span data-ttu-id="52fa8-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="52fa8-114">Boolean</span></span>|<span data-ttu-id="52fa8-115">このレジストリ パスが 64 ビット システムで 32 ビット アプリケーションをチェックするかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="52fa8-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="52fa8-116">キーパス</span><span class="sxs-lookup"><span data-stu-id="52fa8-116">keyPath</span></span>|<span data-ttu-id="52fa8-117">String</span><span class="sxs-lookup"><span data-stu-id="52fa8-117">String</span></span>|<span data-ttu-id="52fa8-118">Win32 基幹業務 (LoB) アプリケーションを検出するためにレジストリ キーのパス</span><span class="sxs-lookup"><span data-stu-id="52fa8-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="52fa8-119">値名</span><span class="sxs-lookup"><span data-stu-id="52fa8-119">valueName</span></span>|<span data-ttu-id="52fa8-120">String</span><span class="sxs-lookup"><span data-stu-id="52fa8-120">String</span></span>|<span data-ttu-id="52fa8-121">レジストリ値の名前</span><span class="sxs-lookup"><span data-stu-id="52fa8-121">The registry value name</span></span>|
|<span data-ttu-id="52fa8-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="52fa8-122">detectionType</span></span>|[<span data-ttu-id="52fa8-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="52fa8-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="52fa8-124">レジストリ データの検出型です。</span><span class="sxs-lookup"><span data-stu-id="52fa8-124">The registry data detection type.</span></span> <span data-ttu-id="52fa8-125">使用可能な値: `notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="52fa8-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="52fa8-126">operator</span><span class="sxs-lookup"><span data-stu-id="52fa8-126">operator</span></span>|[<span data-ttu-id="52fa8-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="52fa8-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="52fa8-128">レジストリ データを検出するための演算子です。</span><span class="sxs-lookup"><span data-stu-id="52fa8-128">The operator for registry data detection.</span></span> <span data-ttu-id="52fa8-129">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="52fa8-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="52fa8-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="52fa8-130">detectionValue</span></span>|<span data-ttu-id="52fa8-131">String</span><span class="sxs-lookup"><span data-stu-id="52fa8-131">String</span></span>|<span data-ttu-id="52fa8-132">レジストリ検出値</span><span class="sxs-lookup"><span data-stu-id="52fa8-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="52fa8-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52fa8-133">Relationships</span></span>
<span data-ttu-id="52fa8-134">なし</span><span class="sxs-lookup"><span data-stu-id="52fa8-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52fa8-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52fa8-135">JSON Representation</span></span>
<span data-ttu-id="52fa8-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52fa8-136">Here is a JSON representation of the resource.</span></span>
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




