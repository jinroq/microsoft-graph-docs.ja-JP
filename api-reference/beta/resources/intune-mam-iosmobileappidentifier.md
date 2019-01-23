---
title: iosMobileAppIdentifier リソースの種類
description: iOS アプリの識別子。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ddd09f6d1f0d49b00282c55bfa6dcbef1fcb1d2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409931"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="91fe3-103">iosMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91fe3-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="91fe3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91fe3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="91fe3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91fe3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91fe3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91fe3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91fe3-107">iOS アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="91fe3-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="91fe3-108">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="91fe3-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91fe3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91fe3-109">Properties</span></span>
|<span data-ttu-id="91fe3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91fe3-110">Property</span></span>|<span data-ttu-id="91fe3-111">型</span><span class="sxs-lookup"><span data-stu-id="91fe3-111">Type</span></span>|<span data-ttu-id="91fe3-112">説明</span><span class="sxs-lookup"><span data-stu-id="91fe3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91fe3-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="91fe3-113">bundleId</span></span>|<span data-ttu-id="91fe3-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="91fe3-114">String</span></span>|<span data-ttu-id="91fe3-115">App Store で指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="91fe3-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91fe3-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91fe3-116">Relationships</span></span>
<span data-ttu-id="91fe3-117">なし</span><span class="sxs-lookup"><span data-stu-id="91fe3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91fe3-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91fe3-118">JSON Representation</span></span>
<span data-ttu-id="91fe3-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91fe3-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```




