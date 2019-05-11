---
title: win32LobAppPowerShellScriptDetection リソースの種類
description: Win32 アプリを検出するための PowerShell スクリプトのプロパティが含まれています
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 440f86e0056c45f325a9a9bd88f737a91c8efb2a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949676"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="ff6d9-103">win32LobAppPowerShellScriptDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff6d9-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="ff6d9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff6d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff6d9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff6d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff6d9-106">Win32 アプリを検出するための PowerShell スクリプトのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="ff6d9-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="ff6d9-107">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ff6d9-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff6d9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff6d9-108">Properties</span></span>
|<span data-ttu-id="ff6d9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff6d9-109">Property</span></span>|<span data-ttu-id="ff6d9-110">型</span><span class="sxs-lookup"><span data-stu-id="ff6d9-110">Type</span></span>|<span data-ttu-id="ff6d9-111">説明</span><span class="sxs-lookup"><span data-stu-id="ff6d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff6d9-112">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="ff6d9-112">enforceSignatureCheck</span></span>|<span data-ttu-id="ff6d9-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff6d9-113">Boolean</span></span>|<span data-ttu-id="ff6d9-114">署名チェックを適用するかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="ff6d9-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="ff6d9-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="ff6d9-115">runAs32Bit</span></span>|<span data-ttu-id="ff6d9-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff6d9-116">Boolean</span></span>|<span data-ttu-id="ff6d9-117">このスクリプトを32ビットとして実行する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="ff6d9-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="ff6d9-118">scriptContent</span><span class="sxs-lookup"><span data-stu-id="ff6d9-118">scriptContent</span></span>|<span data-ttu-id="ff6d9-119">String</span><span class="sxs-lookup"><span data-stu-id="ff6d9-119">String</span></span>|<span data-ttu-id="ff6d9-120">Win32 基幹業務 (LoB) アプリを検出するための、base64 でエンコードされたスクリプトの内容</span><span class="sxs-lookup"><span data-stu-id="ff6d9-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff6d9-121">関係</span><span class="sxs-lookup"><span data-stu-id="ff6d9-121">Relationships</span></span>
<span data-ttu-id="ff6d9-122">なし</span><span class="sxs-lookup"><span data-stu-id="ff6d9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff6d9-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff6d9-123">JSON Representation</span></span>
<span data-ttu-id="ff6d9-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff6d9-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```




