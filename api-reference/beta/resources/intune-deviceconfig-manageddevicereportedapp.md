---
title: managedDeviceReportedApp リソースの種類
description: 報告のためのアプリケーション データ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8aa9a4d825e2333e135a676fa1eeb88e7cfe079c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942977"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="42895-103">managedDeviceReportedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42895-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="42895-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="42895-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42895-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42895-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42895-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="42895-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42895-107">報告のためのアプリケーション データ</span><span class="sxs-lookup"><span data-stu-id="42895-107">Application data for reporting</span></span>
## <a name="properties"></a><span data-ttu-id="42895-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42895-108">Properties</span></span>
|<span data-ttu-id="42895-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42895-109">Property</span></span>|<span data-ttu-id="42895-110">種類</span><span class="sxs-lookup"><span data-stu-id="42895-110">Type</span></span>|<span data-ttu-id="42895-111">説明</span><span class="sxs-lookup"><span data-stu-id="42895-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42895-112">appId</span><span class="sxs-lookup"><span data-stu-id="42895-112">appId</span></span>|<span data-ttu-id="42895-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="42895-113">String</span></span>|<span data-ttu-id="42895-114">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="42895-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="42895-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42895-115">Relationships</span></span>
<span data-ttu-id="42895-116">なし</span><span class="sxs-lookup"><span data-stu-id="42895-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42895-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42895-117">JSON Representation</span></span>
<span data-ttu-id="42895-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42895-118">Here is a JSON representation of the resource.</span></span>
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





