---
title: win32LobAppPowerShellScriptRequirement リソースの種類
description: Win32 アプリを検出するための PowerShell スクリプトのプロパティが含まれています
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 854a1d348d4701ab52895856df306791a20c91d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335572"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="a1d9d-103">win32LobAppPowerShellScriptRequirement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1d9d-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

> <span data-ttu-id="a1d9d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1d9d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1d9d-106">Win32 アプリを検出するための PowerShell スクリプトのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="a1d9d-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="a1d9d-107">[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a1d9d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1d9d-108">Properties</span></span>
|<span data-ttu-id="a1d9d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1d9d-109">Property</span></span>|<span data-ttu-id="a1d9d-110">型</span><span class="sxs-lookup"><span data-stu-id="a1d9d-110">Type</span></span>|<span data-ttu-id="a1d9d-111">説明</span><span class="sxs-lookup"><span data-stu-id="a1d9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1d9d-112">operator</span><span class="sxs-lookup"><span data-stu-id="a1d9d-112">operator</span></span>|[<span data-ttu-id="a1d9d-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="a1d9d-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="a1d9d-114">[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出の演算子。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="a1d9d-115">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="a1d9d-116">detectionValue</span><span class="sxs-lookup"><span data-stu-id="a1d9d-116">detectionValue</span></span>|<span data-ttu-id="a1d9d-117">String</span><span class="sxs-lookup"><span data-stu-id="a1d9d-117">String</span></span>|<span data-ttu-id="a1d9d-118">[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)から継承された検出値</span><span class="sxs-lookup"><span data-stu-id="a1d9d-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="a1d9d-119">displayName</span><span class="sxs-lookup"><span data-stu-id="a1d9d-119">displayName</span></span>|<span data-ttu-id="a1d9d-120">String</span><span class="sxs-lookup"><span data-stu-id="a1d9d-120">String</span></span>|<span data-ttu-id="a1d9d-121">このルールの一意の表示名</span><span class="sxs-lookup"><span data-stu-id="a1d9d-121">The unique display name for this rule</span></span>|
|<span data-ttu-id="a1d9d-122">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="a1d9d-122">enforceSignatureCheck</span></span>|<span data-ttu-id="a1d9d-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1d9d-123">Boolean</span></span>|<span data-ttu-id="a1d9d-124">署名チェックを適用するかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="a1d9d-124">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="a1d9d-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="a1d9d-125">runAs32Bit</span></span>|<span data-ttu-id="a1d9d-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1d9d-126">Boolean</span></span>|<span data-ttu-id="a1d9d-127">このスクリプトを32ビットとして実行する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-127">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="a1d9d-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="a1d9d-128">runAsAccount</span></span>|[<span data-ttu-id="a1d9d-129">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="a1d9d-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="a1d9d-130">スクリプトを実行する実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-130">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="a1d9d-131">可能な値は、`system`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-131">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="a1d9d-132">scriptContent</span><span class="sxs-lookup"><span data-stu-id="a1d9d-132">scriptContent</span></span>|<span data-ttu-id="a1d9d-133">String</span><span class="sxs-lookup"><span data-stu-id="a1d9d-133">String</span></span>|<span data-ttu-id="a1d9d-134">Win32 基幹業務 (LoB) アプリを検出するための、base64 でエンコードされたスクリプトの内容</span><span class="sxs-lookup"><span data-stu-id="a1d9d-134">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="a1d9d-135">detectionType</span><span class="sxs-lookup"><span data-stu-id="a1d9d-135">detectionType</span></span>|[<span data-ttu-id="a1d9d-136">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="a1d9d-136">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="a1d9d-137">スクリプト出力の検出の種類。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-137">The detection type for script output.</span></span> <span data-ttu-id="a1d9d-138">可能な値は、`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version`、`boolean` です。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-138">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1d9d-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1d9d-139">Relationships</span></span>
<span data-ttu-id="a1d9d-140">なし</span><span class="sxs-lookup"><span data-stu-id="a1d9d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1d9d-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1d9d-141">JSON Representation</span></span>
<span data-ttu-id="a1d9d-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a1d9d-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```



