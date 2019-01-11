---
title: managedDeviceReportedApp リソースの種類
description: 報告のためのアプリケーション データ
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 676b89e98f5d54367916a3f3219ab5fc02ddbd80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877218"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="07e72-103">managedDeviceReportedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="07e72-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="07e72-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="07e72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07e72-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07e72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07e72-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="07e72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07e72-107">報告のためのアプリケーション データ</span><span class="sxs-lookup"><span data-stu-id="07e72-107">Application data for reporting</span></span>
## <a name="properties"></a><span data-ttu-id="07e72-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07e72-108">Properties</span></span>
|<span data-ttu-id="07e72-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07e72-109">Property</span></span>|<span data-ttu-id="07e72-110">種類</span><span class="sxs-lookup"><span data-stu-id="07e72-110">Type</span></span>|<span data-ttu-id="07e72-111">説明</span><span class="sxs-lookup"><span data-stu-id="07e72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07e72-112">appId</span><span class="sxs-lookup"><span data-stu-id="07e72-112">appId</span></span>|<span data-ttu-id="07e72-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="07e72-113">String</span></span>|<span data-ttu-id="07e72-114">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="07e72-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="07e72-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="07e72-115">Relationships</span></span>
<span data-ttu-id="07e72-116">なし</span><span class="sxs-lookup"><span data-stu-id="07e72-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07e72-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07e72-117">JSON Representation</span></span>
<span data-ttu-id="07e72-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="07e72-118">Here is a JSON representation of the resource.</span></span>
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





