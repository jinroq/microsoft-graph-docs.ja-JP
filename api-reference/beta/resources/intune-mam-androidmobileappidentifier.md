---
title: androidMobileAppIdentifier リソースの種類
description: Android アプリの識別子。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ca2a2d9d548a94651514d1b3db2b385b5dc64bd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940905"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="c8a51-103">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8a51-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="c8a51-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8a51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8a51-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8a51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8a51-106">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="c8a51-106">The identifier for an Android app.</span></span>


<span data-ttu-id="c8a51-107">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c8a51-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8a51-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8a51-108">Properties</span></span>
|<span data-ttu-id="c8a51-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8a51-109">Property</span></span>|<span data-ttu-id="c8a51-110">型</span><span class="sxs-lookup"><span data-stu-id="c8a51-110">Type</span></span>|<span data-ttu-id="c8a51-111">説明</span><span class="sxs-lookup"><span data-stu-id="c8a51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8a51-112">packageId</span><span class="sxs-lookup"><span data-stu-id="c8a51-112">packageId</span></span>|<span data-ttu-id="c8a51-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c8a51-113">String</span></span>|<span data-ttu-id="c8a51-114">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="c8a51-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8a51-115">関係</span><span class="sxs-lookup"><span data-stu-id="c8a51-115">Relationships</span></span>
<span data-ttu-id="c8a51-116">なし</span><span class="sxs-lookup"><span data-stu-id="c8a51-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8a51-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8a51-117">JSON Representation</span></span>
<span data-ttu-id="c8a51-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8a51-118">Here is a JSON representation of the resource.</span></span>
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




