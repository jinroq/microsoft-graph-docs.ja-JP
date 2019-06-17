---
title: iosMobileAppIdentifier リソースの種類
description: iOS アプリの識別子。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b8b19d08122d16b9cfc9099547e86d155d0540cf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975855"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="1ab11-103">iosMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1ab11-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="1ab11-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ab11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ab11-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1ab11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ab11-106">iOS アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="1ab11-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="1ab11-107">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1ab11-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ab11-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ab11-108">Properties</span></span>
|<span data-ttu-id="1ab11-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ab11-109">Property</span></span>|<span data-ttu-id="1ab11-110">型</span><span class="sxs-lookup"><span data-stu-id="1ab11-110">Type</span></span>|<span data-ttu-id="1ab11-111">説明</span><span class="sxs-lookup"><span data-stu-id="1ab11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ab11-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="1ab11-112">bundleId</span></span>|<span data-ttu-id="1ab11-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1ab11-113">String</span></span>|<span data-ttu-id="1ab11-114">App Store で指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="1ab11-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ab11-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1ab11-115">Relationships</span></span>
<span data-ttu-id="1ab11-116">なし</span><span class="sxs-lookup"><span data-stu-id="1ab11-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ab11-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1ab11-117">JSON Representation</span></span>
<span data-ttu-id="1ab11-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1ab11-118">Here is a JSON representation of the resource.</span></span>
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





