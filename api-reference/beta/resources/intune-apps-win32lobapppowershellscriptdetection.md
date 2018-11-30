---
title: win32LobAppPowerShellScriptDetection リソースの種類
description: Win32 アプリケーションを検出する PowerShell スクリプトのプロパティが含まれています
ms.openlocfilehash: e5d87d3d2a90c0ac7f8ce6db7e14b105583a76f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070291"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="abf9d-103">win32LobAppPowerShellScriptDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="abf9d-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="abf9d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="abf9d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abf9d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abf9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abf9d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="abf9d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abf9d-107">Win32 アプリケーションを検出する PowerShell スクリプトのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="abf9d-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="abf9d-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="abf9d-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="abf9d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abf9d-109">Properties</span></span>
|<span data-ttu-id="abf9d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abf9d-110">Property</span></span>|<span data-ttu-id="abf9d-111">型</span><span class="sxs-lookup"><span data-stu-id="abf9d-111">Type</span></span>|<span data-ttu-id="abf9d-112">説明</span><span class="sxs-lookup"><span data-stu-id="abf9d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abf9d-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="abf9d-113">enforceSignatureCheck</span></span>|<span data-ttu-id="abf9d-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="abf9d-114">Boolean</span></span>|<span data-ttu-id="abf9d-115">署名チェックを強制するかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="abf9d-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="abf9d-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="abf9d-116">runAs32Bit</span></span>|<span data-ttu-id="abf9d-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="abf9d-117">Boolean</span></span>|<span data-ttu-id="abf9d-118">このスクリプトは 32 ビットとして実行するかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="abf9d-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="abf9d-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="abf9d-119">scriptContent</span></span>|<span data-ttu-id="abf9d-120">String</span><span class="sxs-lookup"><span data-stu-id="abf9d-120">String</span></span>|<span data-ttu-id="abf9d-121">Base64 にエンコードされた Win32 基幹業務 (LoB) アプリケーションを検出するためにスクリプトの内容</span><span class="sxs-lookup"><span data-stu-id="abf9d-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="abf9d-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="abf9d-122">Relationships</span></span>
<span data-ttu-id="abf9d-123">なし</span><span class="sxs-lookup"><span data-stu-id="abf9d-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="abf9d-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="abf9d-124">JSON Representation</span></span>
<span data-ttu-id="abf9d-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="abf9d-125">Here is a JSON representation of the resource.</span></span>
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





