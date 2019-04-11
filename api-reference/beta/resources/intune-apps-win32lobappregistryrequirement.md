---
title: win32LobAppRegistryRequirement リソースの種類
description: Win32 アプリを検出するためのレジストリプロパティが含まれています
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64eb6a437350d569a8cbc65b5f8cac0da9661508
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31808966"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="ccf5e-103">win32LobAppRegistryRequirement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ccf5e-103">win32LobAppRegistryRequirement resource type</span></span>

> <span data-ttu-id="ccf5e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccf5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccf5e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ccf5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccf5e-106">Win32 アプリを検出するためのレジストリプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="ccf5e-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="ccf5e-107">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ccf5e-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ccf5e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccf5e-108">Properties</span></span>
|<span data-ttu-id="ccf5e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccf5e-109">Property</span></span>|<span data-ttu-id="ccf5e-110">型</span><span class="sxs-lookup"><span data-stu-id="ccf5e-110">Type</span></span>|<span data-ttu-id="ccf5e-111">説明</span><span class="sxs-lookup"><span data-stu-id="ccf5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccf5e-112">operator</span><span class="sxs-lookup"><span data-stu-id="ccf5e-112">operator</span></span>|[<span data-ttu-id="ccf5e-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="ccf5e-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="ccf5e-114">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出の演算子。</span><span class="sxs-lookup"><span data-stu-id="ccf5e-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="ccf5e-115">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="ccf5e-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="ccf5e-116">detectionValue</span><span class="sxs-lookup"><span data-stu-id="ccf5e-116">detectionValue</span></span>|<span data-ttu-id="ccf5e-117">文字列</span><span class="sxs-lookup"><span data-stu-id="ccf5e-117">String</span></span>|<span data-ttu-id="ccf5e-118">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出値</span><span class="sxs-lookup"><span data-stu-id="ccf5e-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="ccf5e-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="ccf5e-119">check32BitOn64System</span></span>|<span data-ttu-id="ccf5e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccf5e-120">Boolean</span></span>|<span data-ttu-id="ccf5e-121">このレジストリパスが、64ビットシステムの32ビットアプリをチェックするためのものであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="ccf5e-121">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="ccf5e-122">キーパス</span><span class="sxs-lookup"><span data-stu-id="ccf5e-122">keyPath</span></span>|<span data-ttu-id="ccf5e-123">文字列</span><span class="sxs-lookup"><span data-stu-id="ccf5e-123">String</span></span>|<span data-ttu-id="ccf5e-124">Win32 基幹業務 (LoB) アプリを検出するためのレジストリキーのパス</span><span class="sxs-lookup"><span data-stu-id="ccf5e-124">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="ccf5e-125">valueName</span><span class="sxs-lookup"><span data-stu-id="ccf5e-125">valueName</span></span>|<span data-ttu-id="ccf5e-126">文字列</span><span class="sxs-lookup"><span data-stu-id="ccf5e-126">String</span></span>|<span data-ttu-id="ccf5e-127">レジストリ値の名前</span><span class="sxs-lookup"><span data-stu-id="ccf5e-127">The registry value name</span></span>|
|<span data-ttu-id="ccf5e-128">detectionType</span><span class="sxs-lookup"><span data-stu-id="ccf5e-128">detectionType</span></span>|[<span data-ttu-id="ccf5e-129">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="ccf5e-129">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="ccf5e-130">レジストリデータ検出の種類。</span><span class="sxs-lookup"><span data-stu-id="ccf5e-130">The registry data detection type.</span></span> <span data-ttu-id="ccf5e-131">可能な値は `notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version` です。</span><span class="sxs-lookup"><span data-stu-id="ccf5e-131">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccf5e-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ccf5e-132">Relationships</span></span>
<span data-ttu-id="ccf5e-133">なし</span><span class="sxs-lookup"><span data-stu-id="ccf5e-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccf5e-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ccf5e-134">JSON Representation</span></span>
<span data-ttu-id="ccf5e-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ccf5e-135">Here is a JSON representation of the resource.</span></span>
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




