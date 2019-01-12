---
title: win32LobAppMsiInformation リソースの種類
description: Win32 アプリケーションの MSI アプリケーションのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 04972e9e7fa909c220fe55ca6337be3ac44138ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967876"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="9de3e-103">win32LobAppMsiInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9de3e-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="9de3e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9de3e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9de3e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9de3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9de3e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9de3e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9de3e-107">Win32 アプリケーションの MSI アプリケーションのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9de3e-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="9de3e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9de3e-108">Properties</span></span>
|<span data-ttu-id="9de3e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9de3e-109">Property</span></span>|<span data-ttu-id="9de3e-110">種類</span><span class="sxs-lookup"><span data-stu-id="9de3e-110">Type</span></span>|<span data-ttu-id="9de3e-111">説明</span><span class="sxs-lookup"><span data-stu-id="9de3e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9de3e-112">productCode</span><span class="sxs-lookup"><span data-stu-id="9de3e-112">productCode</span></span>|<span data-ttu-id="9de3e-113">String</span><span class="sxs-lookup"><span data-stu-id="9de3e-113">String</span></span>|<span data-ttu-id="9de3e-114">MSI の製品コードです。</span><span class="sxs-lookup"><span data-stu-id="9de3e-114">The MSI product code.</span></span>|
|<span data-ttu-id="9de3e-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="9de3e-115">productVersion</span></span>|<span data-ttu-id="9de3e-116">String</span><span class="sxs-lookup"><span data-stu-id="9de3e-116">String</span></span>|<span data-ttu-id="9de3e-117">MSI 製品のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="9de3e-117">The MSI product version.</span></span>|
|<span data-ttu-id="9de3e-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="9de3e-118">upgradeCode</span></span>|<span data-ttu-id="9de3e-119">String</span><span class="sxs-lookup"><span data-stu-id="9de3e-119">String</span></span>|<span data-ttu-id="9de3e-120">Msi ファイルは、コードをアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="9de3e-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="9de3e-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="9de3e-121">requiresReboot</span></span>|<span data-ttu-id="9de3e-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="9de3e-122">Boolean</span></span>|<span data-ttu-id="9de3e-123">かどうか、MSI アプリケーションには、インストールの完了に再起動するコンピューターが必要です。</span><span class="sxs-lookup"><span data-stu-id="9de3e-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="9de3e-124">packageType</span><span class="sxs-lookup"><span data-stu-id="9de3e-124">packageType</span></span>|[<span data-ttu-id="9de3e-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="9de3e-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="9de3e-126">MSI パッケージの種類です。</span><span class="sxs-lookup"><span data-stu-id="9de3e-126">The MSI package type.</span></span> <span data-ttu-id="9de3e-127">可能な値は、`perMachine`、`perUser`、`dualPurpose` です。</span><span class="sxs-lookup"><span data-stu-id="9de3e-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9de3e-128">関係</span><span class="sxs-lookup"><span data-stu-id="9de3e-128">Relationships</span></span>
<span data-ttu-id="9de3e-129">なし</span><span class="sxs-lookup"><span data-stu-id="9de3e-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9de3e-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9de3e-130">JSON Representation</span></span>
<span data-ttu-id="9de3e-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9de3e-131">Here is a JSON representation of the resource.</span></span>
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





