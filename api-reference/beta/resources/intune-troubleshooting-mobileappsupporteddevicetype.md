---
title: mobileAppSupportedDeviceType リソースの種類
description: デバイスのプロパティ
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1d261b35b5de64057ca2dcdbe516081909523548
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858549"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="77bad-103">mobileAppSupportedDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77bad-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="77bad-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="77bad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77bad-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77bad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77bad-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="77bad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77bad-107">デバイスのプロパティ</span><span class="sxs-lookup"><span data-stu-id="77bad-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="77bad-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77bad-108">Properties</span></span>
|<span data-ttu-id="77bad-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77bad-109">Property</span></span>|<span data-ttu-id="77bad-110">種類</span><span class="sxs-lookup"><span data-stu-id="77bad-110">Type</span></span>|<span data-ttu-id="77bad-111">説明</span><span class="sxs-lookup"><span data-stu-id="77bad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77bad-112">type</span><span class="sxs-lookup"><span data-stu-id="77bad-112">type</span></span>|[<span data-ttu-id="77bad-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="77bad-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="77bad-114">デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="77bad-114">Device type.</span></span> <span data-ttu-id="77bad-115">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="77bad-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="77bad-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="77bad-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="77bad-117">String</span><span class="sxs-lookup"><span data-stu-id="77bad-117">String</span></span>|<span data-ttu-id="77bad-118">OS の最小バージョン</span><span class="sxs-lookup"><span data-stu-id="77bad-118">Minimum OS version</span></span>|
|<span data-ttu-id="77bad-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="77bad-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="77bad-120">String</span><span class="sxs-lookup"><span data-stu-id="77bad-120">String</span></span>|<span data-ttu-id="77bad-121">OS の最大バージョン</span><span class="sxs-lookup"><span data-stu-id="77bad-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="77bad-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="77bad-122">Relationships</span></span>
<span data-ttu-id="77bad-123">なし</span><span class="sxs-lookup"><span data-stu-id="77bad-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="77bad-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77bad-124">JSON Representation</span></span>
<span data-ttu-id="77bad-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="77bad-125">Here is a JSON representation of the resource.</span></span>
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





