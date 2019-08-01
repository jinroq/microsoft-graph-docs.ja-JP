---
title: iosMobileAppIdentifier リソースの種類
description: iOS アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7388e6872eb48d3aba188448c263f492d913f79b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038151"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="c67fe-103">iosMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c67fe-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="c67fe-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c67fe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c67fe-105">iOS アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="c67fe-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="c67fe-106">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c67fe-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c67fe-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c67fe-107">Properties</span></span>
|<span data-ttu-id="c67fe-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c67fe-108">Property</span></span>|<span data-ttu-id="c67fe-109">型</span><span class="sxs-lookup"><span data-stu-id="c67fe-109">Type</span></span>|<span data-ttu-id="c67fe-110">説明</span><span class="sxs-lookup"><span data-stu-id="c67fe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c67fe-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="c67fe-111">bundleId</span></span>|<span data-ttu-id="c67fe-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c67fe-112">String</span></span>|<span data-ttu-id="c67fe-113">App Store で指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="c67fe-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c67fe-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c67fe-114">Relationships</span></span>
<span data-ttu-id="c67fe-115">なし</span><span class="sxs-lookup"><span data-stu-id="c67fe-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c67fe-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c67fe-116">JSON Representation</span></span>
<span data-ttu-id="c67fe-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c67fe-117">Here is a JSON representation of the resource.</span></span>
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



