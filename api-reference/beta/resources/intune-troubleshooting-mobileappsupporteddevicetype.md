---
title: mobileAppSupportedDeviceType リソースの種類
description: デバイスのプロパティ
author: tfitzmac
ms.openlocfilehash: 5ec7d2b1e8340b73ea184dda15d842973f0fab2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314421"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="eaea2-103">mobileAppSupportedDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eaea2-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="eaea2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eaea2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaea2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eaea2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eaea2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eaea2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaea2-107">デバイスのプロパティ</span><span class="sxs-lookup"><span data-stu-id="eaea2-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="eaea2-108">Properties</span><span class="sxs-lookup"><span data-stu-id="eaea2-108">Properties</span></span>
|<span data-ttu-id="eaea2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eaea2-109">Property</span></span>|<span data-ttu-id="eaea2-110">種類</span><span class="sxs-lookup"><span data-stu-id="eaea2-110">Type</span></span>|<span data-ttu-id="eaea2-111">説明</span><span class="sxs-lookup"><span data-stu-id="eaea2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaea2-112">type</span><span class="sxs-lookup"><span data-stu-id="eaea2-112">type</span></span>|[<span data-ttu-id="eaea2-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="eaea2-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="eaea2-114">デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="eaea2-114">Device type.</span></span> <span data-ttu-id="eaea2-115">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="eaea2-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="eaea2-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="eaea2-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="eaea2-117">String</span><span class="sxs-lookup"><span data-stu-id="eaea2-117">String</span></span>|<span data-ttu-id="eaea2-118">OS の最小バージョン</span><span class="sxs-lookup"><span data-stu-id="eaea2-118">Minimum OS version</span></span>|
|<span data-ttu-id="eaea2-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="eaea2-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="eaea2-120">String</span><span class="sxs-lookup"><span data-stu-id="eaea2-120">String</span></span>|<span data-ttu-id="eaea2-121">OS の最大バージョン</span><span class="sxs-lookup"><span data-stu-id="eaea2-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaea2-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eaea2-122">Relationships</span></span>
<span data-ttu-id="eaea2-123">なし</span><span class="sxs-lookup"><span data-stu-id="eaea2-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eaea2-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eaea2-124">JSON Representation</span></span>
<span data-ttu-id="eaea2-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eaea2-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```





