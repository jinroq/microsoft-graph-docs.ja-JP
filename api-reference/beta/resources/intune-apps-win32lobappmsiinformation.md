---
title: win32LobAppMsiInformation リソースの種類
description: Win32 アプリケーションの MSI アプリケーションのプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ba91c572286020a3e349527f325d22bf0be5d67
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399249"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="6de81-103">win32LobAppMsiInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6de81-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="6de81-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6de81-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6de81-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6de81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6de81-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6de81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6de81-107">Win32 アプリケーションの MSI アプリケーションのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6de81-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="6de81-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6de81-108">Properties</span></span>
|<span data-ttu-id="6de81-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6de81-109">Property</span></span>|<span data-ttu-id="6de81-110">型</span><span class="sxs-lookup"><span data-stu-id="6de81-110">Type</span></span>|<span data-ttu-id="6de81-111">説明</span><span class="sxs-lookup"><span data-stu-id="6de81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6de81-112">productCode</span><span class="sxs-lookup"><span data-stu-id="6de81-112">productCode</span></span>|<span data-ttu-id="6de81-113">String</span><span class="sxs-lookup"><span data-stu-id="6de81-113">String</span></span>|<span data-ttu-id="6de81-114">MSI の製品コードです。</span><span class="sxs-lookup"><span data-stu-id="6de81-114">The MSI product code.</span></span>|
|<span data-ttu-id="6de81-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="6de81-115">productVersion</span></span>|<span data-ttu-id="6de81-116">String</span><span class="sxs-lookup"><span data-stu-id="6de81-116">String</span></span>|<span data-ttu-id="6de81-117">MSI 製品のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="6de81-117">The MSI product version.</span></span>|
|<span data-ttu-id="6de81-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="6de81-118">upgradeCode</span></span>|<span data-ttu-id="6de81-119">String</span><span class="sxs-lookup"><span data-stu-id="6de81-119">String</span></span>|<span data-ttu-id="6de81-120">Msi ファイルは、コードをアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="6de81-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="6de81-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="6de81-121">requiresReboot</span></span>|<span data-ttu-id="6de81-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6de81-122">Boolean</span></span>|<span data-ttu-id="6de81-123">かどうか、MSI アプリケーションには、インストールの完了に再起動するコンピューターが必要です。</span><span class="sxs-lookup"><span data-stu-id="6de81-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="6de81-124">packageType</span><span class="sxs-lookup"><span data-stu-id="6de81-124">packageType</span></span>|[<span data-ttu-id="6de81-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="6de81-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="6de81-126">MSI パッケージの種類です。</span><span class="sxs-lookup"><span data-stu-id="6de81-126">The MSI package type.</span></span> <span data-ttu-id="6de81-127">可能な値は、`perMachine`、`perUser`、`dualPurpose` です。</span><span class="sxs-lookup"><span data-stu-id="6de81-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6de81-128">関係</span><span class="sxs-lookup"><span data-stu-id="6de81-128">Relationships</span></span>
<span data-ttu-id="6de81-129">なし</span><span class="sxs-lookup"><span data-stu-id="6de81-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6de81-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6de81-130">JSON Representation</span></span>
<span data-ttu-id="6de81-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6de81-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String"
}
```




