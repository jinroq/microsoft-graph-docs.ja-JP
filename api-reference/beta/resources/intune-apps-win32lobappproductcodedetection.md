---
title: win32LobAppProductCodeDetection リソースの種類
description: Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3a461661d2b2a37cd7f4e9a37561ea682ea0e0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812468"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="04cb5-103">win32LobAppProductCodeDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04cb5-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="04cb5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04cb5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04cb5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04cb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04cb5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04cb5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04cb5-107">Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="04cb5-107">Contains product code and version properties to detect a Win32 App</span></span>

<span data-ttu-id="04cb5-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="04cb5-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04cb5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04cb5-109">Properties</span></span>
|<span data-ttu-id="04cb5-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04cb5-110">Property</span></span>|<span data-ttu-id="04cb5-111">種類</span><span class="sxs-lookup"><span data-stu-id="04cb5-111">Type</span></span>|<span data-ttu-id="04cb5-112">説明</span><span class="sxs-lookup"><span data-stu-id="04cb5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04cb5-113">productCode</span><span class="sxs-lookup"><span data-stu-id="04cb5-113">productCode</span></span>|<span data-ttu-id="04cb5-114">String</span><span class="sxs-lookup"><span data-stu-id="04cb5-114">String</span></span>|<span data-ttu-id="04cb5-115">Win32 基幹業務 (LoB) アプリケーションの製品コードです。</span><span class="sxs-lookup"><span data-stu-id="04cb5-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="04cb5-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="04cb5-116">productVersionOperator</span></span>|[<span data-ttu-id="04cb5-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="04cb5-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="04cb5-118">製品のバージョンを検出する演算子です。</span><span class="sxs-lookup"><span data-stu-id="04cb5-118">The operator to detect product version.</span></span> <span data-ttu-id="04cb5-119">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="04cb5-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="04cb5-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="04cb5-120">productVersion</span></span>|<span data-ttu-id="04cb5-121">String</span><span class="sxs-lookup"><span data-stu-id="04cb5-121">String</span></span>|<span data-ttu-id="04cb5-122">Win32 基幹業務 (LoB) アプリケーションの製品バージョン。</span><span class="sxs-lookup"><span data-stu-id="04cb5-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04cb5-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="04cb5-123">Relationships</span></span>
<span data-ttu-id="04cb5-124">なし</span><span class="sxs-lookup"><span data-stu-id="04cb5-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04cb5-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04cb5-125">JSON Representation</span></span>
<span data-ttu-id="04cb5-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04cb5-126">Here is a JSON representation of the resource.</span></span>
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





