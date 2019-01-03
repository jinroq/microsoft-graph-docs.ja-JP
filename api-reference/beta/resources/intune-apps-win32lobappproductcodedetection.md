---
title: win32LobAppProductCodeDetection リソースの種類
description: Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています
author: tfitzmac
ms.openlocfilehash: d66dab5a43a11c480e0e30f70eb8aecbe47e1fa7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353985"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="24df6-103">win32LobAppProductCodeDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24df6-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="24df6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24df6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24df6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24df6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24df6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24df6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24df6-107">Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="24df6-107">Contains product code and version properties to detect a Win32 App</span></span>

<span data-ttu-id="24df6-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24df6-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24df6-109">Properties</span><span class="sxs-lookup"><span data-stu-id="24df6-109">Properties</span></span>
|<span data-ttu-id="24df6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24df6-110">Property</span></span>|<span data-ttu-id="24df6-111">種類</span><span class="sxs-lookup"><span data-stu-id="24df6-111">Type</span></span>|<span data-ttu-id="24df6-112">説明</span><span class="sxs-lookup"><span data-stu-id="24df6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24df6-113">productCode</span><span class="sxs-lookup"><span data-stu-id="24df6-113">productCode</span></span>|<span data-ttu-id="24df6-114">String</span><span class="sxs-lookup"><span data-stu-id="24df6-114">String</span></span>|<span data-ttu-id="24df6-115">Win32 基幹業務 (LoB) アプリケーションの製品コードです。</span><span class="sxs-lookup"><span data-stu-id="24df6-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="24df6-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="24df6-116">productVersionOperator</span></span>|[<span data-ttu-id="24df6-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="24df6-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="24df6-118">製品のバージョンを検出する演算子です。</span><span class="sxs-lookup"><span data-stu-id="24df6-118">The operator to detect product version.</span></span> <span data-ttu-id="24df6-119">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="24df6-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="24df6-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="24df6-120">productVersion</span></span>|<span data-ttu-id="24df6-121">String</span><span class="sxs-lookup"><span data-stu-id="24df6-121">String</span></span>|<span data-ttu-id="24df6-122">Win32 基幹業務 (LoB) アプリケーションの製品バージョン。</span><span class="sxs-lookup"><span data-stu-id="24df6-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24df6-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24df6-123">Relationships</span></span>
<span data-ttu-id="24df6-124">なし</span><span class="sxs-lookup"><span data-stu-id="24df6-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="24df6-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24df6-125">JSON Representation</span></span>
<span data-ttu-id="24df6-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24df6-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```




