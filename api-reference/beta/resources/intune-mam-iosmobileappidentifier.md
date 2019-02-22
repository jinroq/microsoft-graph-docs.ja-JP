---
title: iosMobileAppIdentifier リソースの種類
description: iOS アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b62a6d9ca0a864f703ddb41eee4f147098e740a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154104"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="eab24-103">iosMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eab24-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="eab24-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eab24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eab24-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eab24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eab24-106">iOS アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="eab24-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="eab24-107">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="eab24-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eab24-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eab24-108">Properties</span></span>
|<span data-ttu-id="eab24-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eab24-109">Property</span></span>|<span data-ttu-id="eab24-110">型</span><span class="sxs-lookup"><span data-stu-id="eab24-110">Type</span></span>|<span data-ttu-id="eab24-111">説明</span><span class="sxs-lookup"><span data-stu-id="eab24-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eab24-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="eab24-112">bundleId</span></span>|<span data-ttu-id="eab24-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="eab24-113">String</span></span>|<span data-ttu-id="eab24-114">App Store で指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="eab24-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eab24-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eab24-115">Relationships</span></span>
<span data-ttu-id="eab24-116">なし</span><span class="sxs-lookup"><span data-stu-id="eab24-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eab24-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eab24-117">JSON Representation</span></span>
<span data-ttu-id="eab24-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eab24-118">Here is a JSON representation of the resource.</span></span>
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




