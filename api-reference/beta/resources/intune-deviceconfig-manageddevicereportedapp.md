---
title: managedDeviceReportedApp リソースの種類
description: 報告のためのアプリケーション データ
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 104503083f5f599bc366de2ca8082fd9fdf3102e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422608"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="f42e5-103">managedDeviceReportedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f42e5-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="f42e5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f42e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f42e5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f42e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f42e5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f42e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f42e5-107">報告のためのアプリケーション データ</span><span class="sxs-lookup"><span data-stu-id="f42e5-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="f42e5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f42e5-108">Properties</span></span>
|<span data-ttu-id="f42e5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f42e5-109">Property</span></span>|<span data-ttu-id="f42e5-110">型</span><span class="sxs-lookup"><span data-stu-id="f42e5-110">Type</span></span>|<span data-ttu-id="f42e5-111">説明</span><span class="sxs-lookup"><span data-stu-id="f42e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f42e5-112">appId</span><span class="sxs-lookup"><span data-stu-id="f42e5-112">appId</span></span>|<span data-ttu-id="f42e5-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f42e5-113">String</span></span>|<span data-ttu-id="f42e5-114">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="f42e5-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="f42e5-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f42e5-115">Relationships</span></span>
<span data-ttu-id="f42e5-116">なし</span><span class="sxs-lookup"><span data-stu-id="f42e5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f42e5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f42e5-117">JSON Representation</span></span>
<span data-ttu-id="f42e5-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f42e5-118">Here is a JSON representation of the resource.</span></span>
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




