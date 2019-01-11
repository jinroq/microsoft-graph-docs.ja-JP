---
title: windows10AssociatedApps リソースの種類
description: Windows 10 関連付けられたアプリケーション定義します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 097edb32ca01d673bb4d42802e8588edd20cf2d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869623"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="27012-103">windows10AssociatedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27012-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="27012-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27012-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27012-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27012-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27012-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="27012-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27012-107">Windows 10 関連付けられたアプリケーション定義します。</span><span class="sxs-lookup"><span data-stu-id="27012-107">Windows 10 Associated Application definition.</span></span>
## <a name="properties"></a><span data-ttu-id="27012-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27012-108">Properties</span></span>
|<span data-ttu-id="27012-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27012-109">Property</span></span>|<span data-ttu-id="27012-110">種類</span><span class="sxs-lookup"><span data-stu-id="27012-110">Type</span></span>|<span data-ttu-id="27012-111">説明</span><span class="sxs-lookup"><span data-stu-id="27012-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27012-112">appType</span><span class="sxs-lookup"><span data-stu-id="27012-112">appType</span></span>|[<span data-ttu-id="27012-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="27012-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="27012-114">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="27012-114">Application type.</span></span> <span data-ttu-id="27012-115">使用可能な値は、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="27012-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="27012-116">識別子</span><span class="sxs-lookup"><span data-stu-id="27012-116">identifier</span></span>|<span data-ttu-id="27012-117">String</span><span class="sxs-lookup"><span data-stu-id="27012-117">String</span></span>|<span data-ttu-id="27012-118">識別子です。</span><span class="sxs-lookup"><span data-stu-id="27012-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27012-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27012-119">Relationships</span></span>
<span data-ttu-id="27012-120">なし</span><span class="sxs-lookup"><span data-stu-id="27012-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27012-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27012-121">JSON Representation</span></span>
<span data-ttu-id="27012-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="27012-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





