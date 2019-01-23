---
title: win32LobAppPowerShellScriptDetection リソースの種類
description: Win32 アプリケーションを検出する PowerShell スクリプトのプロパティが含まれています
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5c02228589042d0abf36c34c5818c5a4610514e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399641"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="9f231-103">win32LobAppPowerShellScriptDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f231-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="9f231-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f231-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f231-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f231-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f231-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f231-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f231-107">Win32 アプリケーションを検出する PowerShell スクリプトのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="9f231-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="9f231-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9f231-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9f231-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f231-109">Properties</span></span>
|<span data-ttu-id="9f231-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f231-110">Property</span></span>|<span data-ttu-id="9f231-111">型</span><span class="sxs-lookup"><span data-stu-id="9f231-111">Type</span></span>|<span data-ttu-id="9f231-112">説明</span><span class="sxs-lookup"><span data-stu-id="9f231-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f231-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="9f231-113">enforceSignatureCheck</span></span>|<span data-ttu-id="9f231-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f231-114">Boolean</span></span>|<span data-ttu-id="9f231-115">署名チェックを強制するかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="9f231-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="9f231-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="9f231-116">runAs32Bit</span></span>|<span data-ttu-id="9f231-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f231-117">Boolean</span></span>|<span data-ttu-id="9f231-118">このスクリプトは 32 ビットとして実行するかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="9f231-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="9f231-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="9f231-119">scriptContent</span></span>|<span data-ttu-id="9f231-120">String</span><span class="sxs-lookup"><span data-stu-id="9f231-120">String</span></span>|<span data-ttu-id="9f231-121">Base64 にエンコードされた Win32 基幹業務 (LoB) アプリケーションを検出するためにスクリプトの内容</span><span class="sxs-lookup"><span data-stu-id="9f231-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f231-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f231-122">Relationships</span></span>
<span data-ttu-id="9f231-123">なし</span><span class="sxs-lookup"><span data-stu-id="9f231-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f231-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f231-124">JSON Representation</span></span>
<span data-ttu-id="9f231-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f231-125">Here is a JSON representation of the resource.</span></span>
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




