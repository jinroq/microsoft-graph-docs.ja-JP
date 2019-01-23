---
title: win32LobAppProductCodeDetection リソースの種類
description: Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f5af1cfc5fffe5241ef3b7883c3ebe6a2100278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411205"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="25c5f-103">win32LobAppProductCodeDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25c5f-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="25c5f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="25c5f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="25c5f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25c5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25c5f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="25c5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25c5f-107">Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="25c5f-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="25c5f-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="25c5f-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25c5f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25c5f-109">Properties</span></span>
|<span data-ttu-id="25c5f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25c5f-110">Property</span></span>|<span data-ttu-id="25c5f-111">型</span><span class="sxs-lookup"><span data-stu-id="25c5f-111">Type</span></span>|<span data-ttu-id="25c5f-112">説明</span><span class="sxs-lookup"><span data-stu-id="25c5f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25c5f-113">productCode</span><span class="sxs-lookup"><span data-stu-id="25c5f-113">productCode</span></span>|<span data-ttu-id="25c5f-114">String</span><span class="sxs-lookup"><span data-stu-id="25c5f-114">String</span></span>|<span data-ttu-id="25c5f-115">Win32 基幹業務 (LoB) アプリケーションの製品コードです。</span><span class="sxs-lookup"><span data-stu-id="25c5f-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="25c5f-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="25c5f-116">productVersionOperator</span></span>|[<span data-ttu-id="25c5f-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="25c5f-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="25c5f-118">製品のバージョンを検出する演算子です。</span><span class="sxs-lookup"><span data-stu-id="25c5f-118">The operator to detect product version.</span></span> <span data-ttu-id="25c5f-119">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="25c5f-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="25c5f-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="25c5f-120">productVersion</span></span>|<span data-ttu-id="25c5f-121">String</span><span class="sxs-lookup"><span data-stu-id="25c5f-121">String</span></span>|<span data-ttu-id="25c5f-122">Win32 基幹業務 (LoB) アプリケーションの製品バージョン。</span><span class="sxs-lookup"><span data-stu-id="25c5f-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25c5f-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25c5f-123">Relationships</span></span>
<span data-ttu-id="25c5f-124">なし</span><span class="sxs-lookup"><span data-stu-id="25c5f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25c5f-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25c5f-125">JSON Representation</span></span>
<span data-ttu-id="25c5f-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="25c5f-126">Here is a JSON representation of the resource.</span></span>
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




