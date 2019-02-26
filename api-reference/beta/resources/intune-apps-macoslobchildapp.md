---
title: macoslobchildapp リソースの種類
description: バンドルパッケージ内の MacOS LOB アプリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4bf8a8715bb681d1737a2fb1b39e5bac61fb9d7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146999"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="bbaa9-103">macoslobchildapp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bbaa9-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="bbaa9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbaa9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbaa9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bbaa9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbaa9-106">バンドルパッケージ内の MacOS LOB アプリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bbaa9-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="bbaa9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbaa9-107">Properties</span></span>
|<span data-ttu-id="bbaa9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbaa9-108">Property</span></span>|<span data-ttu-id="bbaa9-109">型</span><span class="sxs-lookup"><span data-stu-id="bbaa9-109">Type</span></span>|<span data-ttu-id="bbaa9-110">説明</span><span class="sxs-lookup"><span data-stu-id="bbaa9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbaa9-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="bbaa9-111">bundleId</span></span>|<span data-ttu-id="bbaa9-112">String</span><span class="sxs-lookup"><span data-stu-id="bbaa9-112">String</span></span>|<span data-ttu-id="bbaa9-113">ID 名。</span><span class="sxs-lookup"><span data-stu-id="bbaa9-113">The Identity Name.</span></span>|
|<span data-ttu-id="bbaa9-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="bbaa9-114">buildNumber</span></span>|<span data-ttu-id="bbaa9-115">String</span><span class="sxs-lookup"><span data-stu-id="bbaa9-115">String</span></span>|<span data-ttu-id="bbaa9-116">MacOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="bbaa9-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bbaa9-117">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="bbaa9-117">versionNumber</span></span>|<span data-ttu-id="bbaa9-118">String</span><span class="sxs-lookup"><span data-stu-id="bbaa9-118">String</span></span>|<span data-ttu-id="bbaa9-119">MacOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="bbaa9-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbaa9-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bbaa9-120">Relationships</span></span>
<span data-ttu-id="bbaa9-121">なし</span><span class="sxs-lookup"><span data-stu-id="bbaa9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbaa9-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bbaa9-122">JSON Representation</span></span>
<span data-ttu-id="bbaa9-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bbaa9-123">Here is a JSON representation of the resource.</span></span>
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




