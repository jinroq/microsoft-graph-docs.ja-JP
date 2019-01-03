---
title: win32LobAppPowerShellScriptDetection リソースの種類
description: Win32 アプリケーションを検出する PowerShell スクリプトのプロパティが含まれています
author: tfitzmac
ms.openlocfilehash: 7f69b2c066ae90cfcd805b3d3cfe57193046d440
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327574"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="221c3-103">win32LobAppPowerShellScriptDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="221c3-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="221c3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="221c3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="221c3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="221c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="221c3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="221c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="221c3-107">Win32 アプリケーションを検出する PowerShell スクリプトのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="221c3-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="221c3-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="221c3-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="221c3-109">Properties</span><span class="sxs-lookup"><span data-stu-id="221c3-109">Properties</span></span>
|<span data-ttu-id="221c3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="221c3-110">Property</span></span>|<span data-ttu-id="221c3-111">種類</span><span class="sxs-lookup"><span data-stu-id="221c3-111">Type</span></span>|<span data-ttu-id="221c3-112">説明</span><span class="sxs-lookup"><span data-stu-id="221c3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="221c3-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="221c3-113">enforceSignatureCheck</span></span>|<span data-ttu-id="221c3-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="221c3-114">Boolean</span></span>|<span data-ttu-id="221c3-115">署名チェックを強制するかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="221c3-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="221c3-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="221c3-116">runAs32Bit</span></span>|<span data-ttu-id="221c3-117">ブール型</span><span class="sxs-lookup"><span data-stu-id="221c3-117">Boolean</span></span>|<span data-ttu-id="221c3-118">このスクリプトは 32 ビットとして実行するかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="221c3-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="221c3-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="221c3-119">scriptContent</span></span>|<span data-ttu-id="221c3-120">String</span><span class="sxs-lookup"><span data-stu-id="221c3-120">String</span></span>|<span data-ttu-id="221c3-121">Base64 にエンコードされた Win32 基幹業務 (LoB) アプリケーションを検出するためにスクリプトの内容</span><span class="sxs-lookup"><span data-stu-id="221c3-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="221c3-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="221c3-122">Relationships</span></span>
<span data-ttu-id="221c3-123">なし</span><span class="sxs-lookup"><span data-stu-id="221c3-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="221c3-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="221c3-124">JSON Representation</span></span>
<span data-ttu-id="221c3-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="221c3-125">Here is a JSON representation of the resource.</span></span>
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




