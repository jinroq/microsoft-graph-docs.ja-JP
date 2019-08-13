---
title: managedDeviceReportedApp リソースの種類
description: レポート用のアプリケーションデータ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6561a6cee5a02f46c3347a1919c93c3807250fa8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368829"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="e95a0-103">managedDeviceReportedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e95a0-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="e95a0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e95a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e95a0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e95a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e95a0-106">レポート用のアプリケーションデータ</span><span class="sxs-lookup"><span data-stu-id="e95a0-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="e95a0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e95a0-107">Properties</span></span>
|<span data-ttu-id="e95a0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e95a0-108">Property</span></span>|<span data-ttu-id="e95a0-109">型</span><span class="sxs-lookup"><span data-stu-id="e95a0-109">Type</span></span>|<span data-ttu-id="e95a0-110">説明</span><span class="sxs-lookup"><span data-stu-id="e95a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e95a0-111">appId</span><span class="sxs-lookup"><span data-stu-id="e95a0-111">appId</span></span>|<span data-ttu-id="e95a0-112">String</span><span class="sxs-lookup"><span data-stu-id="e95a0-112">String</span></span>|<span data-ttu-id="e95a0-113">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="e95a0-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e95a0-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e95a0-114">Relationships</span></span>
<span data-ttu-id="e95a0-115">なし</span><span class="sxs-lookup"><span data-stu-id="e95a0-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e95a0-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e95a0-116">JSON Representation</span></span>
<span data-ttu-id="e95a0-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e95a0-117">Here is a JSON representation of the resource.</span></span>
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



