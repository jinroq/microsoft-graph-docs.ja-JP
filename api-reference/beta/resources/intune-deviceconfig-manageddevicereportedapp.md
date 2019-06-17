---
title: managedDeviceReportedApp リソースの種類
description: レポート用のアプリケーションデータ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e028ec07142a7902ec02b2b8eeccdc9c378170d8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992025"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="370b8-103">managedDeviceReportedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="370b8-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="370b8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="370b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="370b8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="370b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="370b8-106">レポート用のアプリケーションデータ</span><span class="sxs-lookup"><span data-stu-id="370b8-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="370b8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="370b8-107">Properties</span></span>
|<span data-ttu-id="370b8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="370b8-108">Property</span></span>|<span data-ttu-id="370b8-109">型</span><span class="sxs-lookup"><span data-stu-id="370b8-109">Type</span></span>|<span data-ttu-id="370b8-110">説明</span><span class="sxs-lookup"><span data-stu-id="370b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="370b8-111">appId</span><span class="sxs-lookup"><span data-stu-id="370b8-111">appId</span></span>|<span data-ttu-id="370b8-112">String</span><span class="sxs-lookup"><span data-stu-id="370b8-112">String</span></span>|<span data-ttu-id="370b8-113">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="370b8-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="370b8-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="370b8-114">Relationships</span></span>
<span data-ttu-id="370b8-115">なし</span><span class="sxs-lookup"><span data-stu-id="370b8-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="370b8-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="370b8-116">JSON Representation</span></span>
<span data-ttu-id="370b8-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="370b8-117">Here is a JSON representation of the resource.</span></span>
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





