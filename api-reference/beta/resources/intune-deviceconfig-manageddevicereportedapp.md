---
title: managedDeviceReportedApp リソースの種類
description: レポート用のアプリケーションデータ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76317a14d05ad1e4a949485f2ae63e00b1e91b81
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944944"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="ba16d-103">managedDeviceReportedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba16d-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="ba16d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba16d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba16d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba16d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba16d-106">レポート用のアプリケーションデータ</span><span class="sxs-lookup"><span data-stu-id="ba16d-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="ba16d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba16d-107">Properties</span></span>
|<span data-ttu-id="ba16d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba16d-108">Property</span></span>|<span data-ttu-id="ba16d-109">型</span><span class="sxs-lookup"><span data-stu-id="ba16d-109">Type</span></span>|<span data-ttu-id="ba16d-110">説明</span><span class="sxs-lookup"><span data-stu-id="ba16d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba16d-111">appId</span><span class="sxs-lookup"><span data-stu-id="ba16d-111">appId</span></span>|<span data-ttu-id="ba16d-112">String</span><span class="sxs-lookup"><span data-stu-id="ba16d-112">String</span></span>|<span data-ttu-id="ba16d-113">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="ba16d-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba16d-114">関係</span><span class="sxs-lookup"><span data-stu-id="ba16d-114">Relationships</span></span>
<span data-ttu-id="ba16d-115">なし</span><span class="sxs-lookup"><span data-stu-id="ba16d-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba16d-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba16d-116">JSON Representation</span></span>
<span data-ttu-id="ba16d-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba16d-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```




