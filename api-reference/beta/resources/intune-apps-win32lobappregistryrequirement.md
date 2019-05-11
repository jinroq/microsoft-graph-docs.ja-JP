---
title: win32LobAppRegistryRequirement リソースの種類
description: Win32 アプリを検出するためのレジストリプロパティが含まれています
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bd6f5e64953f71bcea6ed5e6e06205213bba58b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949536"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="f9092-103">win32LobAppRegistryRequirement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f9092-103">win32LobAppRegistryRequirement resource type</span></span>

> <span data-ttu-id="f9092-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9092-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9092-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9092-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9092-106">Win32 アプリを検出するためのレジストリプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="f9092-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="f9092-107">[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f9092-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f9092-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9092-108">Properties</span></span>
|<span data-ttu-id="f9092-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9092-109">Property</span></span>|<span data-ttu-id="f9092-110">型</span><span class="sxs-lookup"><span data-stu-id="f9092-110">Type</span></span>|<span data-ttu-id="f9092-111">説明</span><span class="sxs-lookup"><span data-stu-id="f9092-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9092-112">operator</span><span class="sxs-lookup"><span data-stu-id="f9092-112">operator</span></span>|[<span data-ttu-id="f9092-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="f9092-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="f9092-114">[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出の演算子。</span><span class="sxs-lookup"><span data-stu-id="f9092-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="f9092-115">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="f9092-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="f9092-116">detectionValue</span><span class="sxs-lookup"><span data-stu-id="f9092-116">detectionValue</span></span>|<span data-ttu-id="f9092-117">String</span><span class="sxs-lookup"><span data-stu-id="f9092-117">String</span></span>|<span data-ttu-id="f9092-118">[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出値</span><span class="sxs-lookup"><span data-stu-id="f9092-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="f9092-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="f9092-119">check32BitOn64System</span></span>|<span data-ttu-id="f9092-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9092-120">Boolean</span></span>|<span data-ttu-id="f9092-121">このレジストリパスが、64ビットシステムの32ビットアプリをチェックするためのものであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="f9092-121">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="f9092-122">キーパス</span><span class="sxs-lookup"><span data-stu-id="f9092-122">keyPath</span></span>|<span data-ttu-id="f9092-123">String</span><span class="sxs-lookup"><span data-stu-id="f9092-123">String</span></span>|<span data-ttu-id="f9092-124">Win32 基幹業務 (LoB) アプリを検出するためのレジストリキーのパス</span><span class="sxs-lookup"><span data-stu-id="f9092-124">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="f9092-125">valueName</span><span class="sxs-lookup"><span data-stu-id="f9092-125">valueName</span></span>|<span data-ttu-id="f9092-126">String</span><span class="sxs-lookup"><span data-stu-id="f9092-126">String</span></span>|<span data-ttu-id="f9092-127">レジストリ値の名前</span><span class="sxs-lookup"><span data-stu-id="f9092-127">The registry value name</span></span>|
|<span data-ttu-id="f9092-128">detectionType</span><span class="sxs-lookup"><span data-stu-id="f9092-128">detectionType</span></span>|[<span data-ttu-id="f9092-129">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="f9092-129">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="f9092-130">レジストリデータ検出の種類。</span><span class="sxs-lookup"><span data-stu-id="f9092-130">The registry data detection type.</span></span> <span data-ttu-id="f9092-131">使用可能な値: `notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="f9092-131">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9092-132">関係</span><span class="sxs-lookup"><span data-stu-id="f9092-132">Relationships</span></span>
<span data-ttu-id="f9092-133">なし</span><span class="sxs-lookup"><span data-stu-id="f9092-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9092-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f9092-134">JSON Representation</span></span>
<span data-ttu-id="f9092-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f9092-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRequirement",
  "operator": "String",
  "detectionValue": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String"
}
```




