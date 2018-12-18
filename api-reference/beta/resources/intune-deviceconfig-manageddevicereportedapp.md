---
title: managedDeviceReportedApp リソースの種類
description: 報告のためのアプリケーション データ
author: tfitzmac
ms.openlocfilehash: 7fd01c5fd7553769653abd6e16ecc9ec40a79b8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359494"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="f8010-103">managedDeviceReportedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f8010-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="f8010-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f8010-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8010-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8010-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8010-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f8010-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8010-107">報告のためのアプリケーション データ</span><span class="sxs-lookup"><span data-stu-id="f8010-107">Application data for reporting</span></span>
## <a name="properties"></a><span data-ttu-id="f8010-108">Properties</span><span class="sxs-lookup"><span data-stu-id="f8010-108">Properties</span></span>
|<span data-ttu-id="f8010-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8010-109">Property</span></span>|<span data-ttu-id="f8010-110">種類</span><span class="sxs-lookup"><span data-stu-id="f8010-110">Type</span></span>|<span data-ttu-id="f8010-111">説明</span><span class="sxs-lookup"><span data-stu-id="f8010-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8010-112">appId</span><span class="sxs-lookup"><span data-stu-id="f8010-112">appId</span></span>|<span data-ttu-id="f8010-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f8010-113">String</span></span>|<span data-ttu-id="f8010-114">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="f8010-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8010-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f8010-115">Relationships</span></span>
<span data-ttu-id="f8010-116">なし</span><span class="sxs-lookup"><span data-stu-id="f8010-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8010-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f8010-117">JSON Representation</span></span>
<span data-ttu-id="f8010-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f8010-118">Here is a JSON representation of the resource.</span></span>
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





