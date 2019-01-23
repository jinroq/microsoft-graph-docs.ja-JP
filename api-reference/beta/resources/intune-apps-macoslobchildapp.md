---
title: macOSLobChildApp リソースの種類
description: バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a6a8cafc0f9b47f40fe7e922130a41d37a427e5e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403022"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="f9d47-103">macOSLobChildApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f9d47-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="f9d47-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9d47-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9d47-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9d47-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9d47-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9d47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9d47-107">バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="f9d47-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="f9d47-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9d47-108">Properties</span></span>
|<span data-ttu-id="f9d47-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9d47-109">Property</span></span>|<span data-ttu-id="f9d47-110">型</span><span class="sxs-lookup"><span data-stu-id="f9d47-110">Type</span></span>|<span data-ttu-id="f9d47-111">説明</span><span class="sxs-lookup"><span data-stu-id="f9d47-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9d47-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="f9d47-112">bundleId</span></span>|<span data-ttu-id="f9d47-113">String</span><span class="sxs-lookup"><span data-stu-id="f9d47-113">String</span></span>|<span data-ttu-id="f9d47-114">ID 名。</span><span class="sxs-lookup"><span data-stu-id="f9d47-114">The Identity Name.</span></span>|
|<span data-ttu-id="f9d47-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="f9d47-115">buildNumber</span></span>|<span data-ttu-id="f9d47-116">String</span><span class="sxs-lookup"><span data-stu-id="f9d47-116">String</span></span>|<span data-ttu-id="f9d47-117">MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。</span><span class="sxs-lookup"><span data-stu-id="f9d47-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f9d47-118">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="f9d47-118">versionNumber</span></span>|<span data-ttu-id="f9d47-119">String</span><span class="sxs-lookup"><span data-stu-id="f9d47-119">String</span></span>|<span data-ttu-id="f9d47-120">MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="f9d47-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9d47-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f9d47-121">Relationships</span></span>
<span data-ttu-id="f9d47-122">なし</span><span class="sxs-lookup"><span data-stu-id="f9d47-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9d47-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f9d47-123">JSON Representation</span></span>
<span data-ttu-id="f9d47-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f9d47-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```




