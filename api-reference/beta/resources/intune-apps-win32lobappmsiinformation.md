---
title: win32LobAppMsiInformation リソースの種類
description: Win32 アプリ用の MSI アプリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d993306cdd5f6c69d373669ed83fab6f986497df
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971656"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="90a4c-103">win32LobAppMsiInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90a4c-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="90a4c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90a4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90a4c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90a4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90a4c-106">Win32 アプリ用の MSI アプリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="90a4c-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="90a4c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90a4c-107">Properties</span></span>
|<span data-ttu-id="90a4c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90a4c-108">Property</span></span>|<span data-ttu-id="90a4c-109">型</span><span class="sxs-lookup"><span data-stu-id="90a4c-109">Type</span></span>|<span data-ttu-id="90a4c-110">説明</span><span class="sxs-lookup"><span data-stu-id="90a4c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90a4c-111">productCode</span><span class="sxs-lookup"><span data-stu-id="90a4c-111">productCode</span></span>|<span data-ttu-id="90a4c-112">String</span><span class="sxs-lookup"><span data-stu-id="90a4c-112">String</span></span>|<span data-ttu-id="90a4c-113">MSI 製品コード。</span><span class="sxs-lookup"><span data-stu-id="90a4c-113">The MSI product code.</span></span>|
|<span data-ttu-id="90a4c-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="90a4c-114">productVersion</span></span>|<span data-ttu-id="90a4c-115">String</span><span class="sxs-lookup"><span data-stu-id="90a4c-115">String</span></span>|<span data-ttu-id="90a4c-116">MSI 製品バージョン。</span><span class="sxs-lookup"><span data-stu-id="90a4c-116">The MSI product version.</span></span>|
|<span data-ttu-id="90a4c-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="90a4c-117">upgradeCode</span></span>|<span data-ttu-id="90a4c-118">String</span><span class="sxs-lookup"><span data-stu-id="90a4c-118">String</span></span>|<span data-ttu-id="90a4c-119">MSI アップグレードコード。</span><span class="sxs-lookup"><span data-stu-id="90a4c-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="90a4c-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="90a4c-120">requiresReboot</span></span>|<span data-ttu-id="90a4c-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="90a4c-121">Boolean</span></span>|<span data-ttu-id="90a4c-122">MSI アプリがインストールを完了するためにコンピューターを再起動する必要があるかどうか。</span><span class="sxs-lookup"><span data-stu-id="90a4c-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="90a4c-123">packageType</span><span class="sxs-lookup"><span data-stu-id="90a4c-123">packageType</span></span>|[<span data-ttu-id="90a4c-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="90a4c-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="90a4c-125">MSI パッケージの種類。</span><span class="sxs-lookup"><span data-stu-id="90a4c-125">The MSI package type.</span></span> <span data-ttu-id="90a4c-126">可能な値は、`perMachine`、`perUser`、`dualPurpose` です。</span><span class="sxs-lookup"><span data-stu-id="90a4c-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="90a4c-127">productName</span><span class="sxs-lookup"><span data-stu-id="90a4c-127">productName</span></span>|<span data-ttu-id="90a4c-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="90a4c-128">String</span></span>|<span data-ttu-id="90a4c-129">MSI 製品名。</span><span class="sxs-lookup"><span data-stu-id="90a4c-129">The MSI product name.</span></span>|
|<span data-ttu-id="90a4c-130">publisher</span><span class="sxs-lookup"><span data-stu-id="90a4c-130">publisher</span></span>|<span data-ttu-id="90a4c-131">String</span><span class="sxs-lookup"><span data-stu-id="90a4c-131">String</span></span>|<span data-ttu-id="90a4c-132">MSI パブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="90a4c-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90a4c-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="90a4c-133">Relationships</span></span>
<span data-ttu-id="90a4c-134">なし</span><span class="sxs-lookup"><span data-stu-id="90a4c-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90a4c-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90a4c-135">JSON Representation</span></span>
<span data-ttu-id="90a4c-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="90a4c-136">Here is a JSON representation of the resource.</span></span>
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
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```





