---
title: androidMobileAppIdentifier リソースの種類
description: Android アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa3a0f90626ea01290ccd1d0eee3873374efb546
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261174"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="dbae4-103">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dbae4-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="dbae4-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dbae4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbae4-105">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="dbae4-105">The identifier for an Android app.</span></span>


<span data-ttu-id="dbae4-106">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="dbae4-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dbae4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dbae4-107">Properties</span></span>
|<span data-ttu-id="dbae4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dbae4-108">Property</span></span>|<span data-ttu-id="dbae4-109">型</span><span class="sxs-lookup"><span data-stu-id="dbae4-109">Type</span></span>|<span data-ttu-id="dbae4-110">説明</span><span class="sxs-lookup"><span data-stu-id="dbae4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbae4-111">packageId</span><span class="sxs-lookup"><span data-stu-id="dbae4-111">packageId</span></span>|<span data-ttu-id="dbae4-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dbae4-112">String</span></span>|<span data-ttu-id="dbae4-113">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="dbae4-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbae4-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dbae4-114">Relationships</span></span>
<span data-ttu-id="dbae4-115">なし</span><span class="sxs-lookup"><span data-stu-id="dbae4-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbae4-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dbae4-116">JSON Representation</span></span>
<span data-ttu-id="dbae4-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dbae4-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



