---
title: win32LobAppProductCodeDetection リソースの種類
description: Win32 アプリを検出するための製品コードとバージョンプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 755d0470873da1e5176e0962ace955d1fc647b80
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780456"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="f007e-103">win32LobAppProductCodeDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f007e-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="f007e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f007e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f007e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f007e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f007e-106">Win32 アプリを検出するための製品コードとバージョンプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f007e-106">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="f007e-107">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f007e-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f007e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f007e-108">Properties</span></span>
|<span data-ttu-id="f007e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f007e-109">Property</span></span>|<span data-ttu-id="f007e-110">型</span><span class="sxs-lookup"><span data-stu-id="f007e-110">Type</span></span>|<span data-ttu-id="f007e-111">説明</span><span class="sxs-lookup"><span data-stu-id="f007e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f007e-112">productCode</span><span class="sxs-lookup"><span data-stu-id="f007e-112">productCode</span></span>|<span data-ttu-id="f007e-113">文字列</span><span class="sxs-lookup"><span data-stu-id="f007e-113">String</span></span>|<span data-ttu-id="f007e-114">Win32 基幹業務 (LoB) アプリの製品コード。</span><span class="sxs-lookup"><span data-stu-id="f007e-114">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f007e-115">productversionoperator</span><span class="sxs-lookup"><span data-stu-id="f007e-115">productVersionOperator</span></span>|[<span data-ttu-id="f007e-116">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="f007e-116">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="f007e-117">製品バージョンを検出するための演算子。</span><span class="sxs-lookup"><span data-stu-id="f007e-117">The operator to detect product version.</span></span> <span data-ttu-id="f007e-118">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="f007e-118">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="f007e-119">productVersion</span><span class="sxs-lookup"><span data-stu-id="f007e-119">productVersion</span></span>|<span data-ttu-id="f007e-120">String</span><span class="sxs-lookup"><span data-stu-id="f007e-120">String</span></span>|<span data-ttu-id="f007e-121">Win32 基幹業務 (LoB) アプリの製品バージョン。</span><span class="sxs-lookup"><span data-stu-id="f007e-121">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f007e-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f007e-122">Relationships</span></span>
<span data-ttu-id="f007e-123">なし</span><span class="sxs-lookup"><span data-stu-id="f007e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f007e-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f007e-124">JSON Representation</span></span>
<span data-ttu-id="f007e-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f007e-125">Here is a JSON representation of the resource.</span></span>
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





