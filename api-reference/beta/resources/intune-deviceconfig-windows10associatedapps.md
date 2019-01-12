---
title: windows10AssociatedApps リソースの種類
description: Windows 10 関連付けられたアプリケーション定義します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d1f6363027ae46263146efdbf3f5ac5254afcd93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911911"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="95e37-103">windows10AssociatedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95e37-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="95e37-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95e37-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95e37-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95e37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95e37-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="95e37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95e37-107">Windows 10 関連付けられたアプリケーション定義します。</span><span class="sxs-lookup"><span data-stu-id="95e37-107">Windows 10 Associated Application definition.</span></span>
## <a name="properties"></a><span data-ttu-id="95e37-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95e37-108">Properties</span></span>
|<span data-ttu-id="95e37-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95e37-109">Property</span></span>|<span data-ttu-id="95e37-110">種類</span><span class="sxs-lookup"><span data-stu-id="95e37-110">Type</span></span>|<span data-ttu-id="95e37-111">説明</span><span class="sxs-lookup"><span data-stu-id="95e37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95e37-112">appType</span><span class="sxs-lookup"><span data-stu-id="95e37-112">appType</span></span>|[<span data-ttu-id="95e37-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="95e37-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="95e37-114">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="95e37-114">Application type.</span></span> <span data-ttu-id="95e37-115">使用可能な値は、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="95e37-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="95e37-116">識別子</span><span class="sxs-lookup"><span data-stu-id="95e37-116">identifier</span></span>|<span data-ttu-id="95e37-117">String</span><span class="sxs-lookup"><span data-stu-id="95e37-117">String</span></span>|<span data-ttu-id="95e37-118">識別子です。</span><span class="sxs-lookup"><span data-stu-id="95e37-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95e37-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95e37-119">Relationships</span></span>
<span data-ttu-id="95e37-120">なし</span><span class="sxs-lookup"><span data-stu-id="95e37-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="95e37-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95e37-121">JSON Representation</span></span>
<span data-ttu-id="95e37-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95e37-122">Here is a JSON representation of the resource.</span></span>
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





