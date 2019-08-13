---
title: win32LobAppMsiInformation リソースの種類
description: Win32 アプリ用の MSI アプリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 958cc834a2044e623a8fa1cf7ed37bed1ec7b1f9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335649"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="0a5aa-103">win32LobAppMsiInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a5aa-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="0a5aa-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a5aa-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a5aa-106">Win32 アプリ用の MSI アプリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="0a5aa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a5aa-107">Properties</span></span>
|<span data-ttu-id="0a5aa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a5aa-108">Property</span></span>|<span data-ttu-id="0a5aa-109">型</span><span class="sxs-lookup"><span data-stu-id="0a5aa-109">Type</span></span>|<span data-ttu-id="0a5aa-110">説明</span><span class="sxs-lookup"><span data-stu-id="0a5aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a5aa-111">productCode</span><span class="sxs-lookup"><span data-stu-id="0a5aa-111">productCode</span></span>|<span data-ttu-id="0a5aa-112">String</span><span class="sxs-lookup"><span data-stu-id="0a5aa-112">String</span></span>|<span data-ttu-id="0a5aa-113">MSI 製品コード。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-113">The MSI product code.</span></span>|
|<span data-ttu-id="0a5aa-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="0a5aa-114">productVersion</span></span>|<span data-ttu-id="0a5aa-115">String</span><span class="sxs-lookup"><span data-stu-id="0a5aa-115">String</span></span>|<span data-ttu-id="0a5aa-116">MSI 製品バージョン。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-116">The MSI product version.</span></span>|
|<span data-ttu-id="0a5aa-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="0a5aa-117">upgradeCode</span></span>|<span data-ttu-id="0a5aa-118">String</span><span class="sxs-lookup"><span data-stu-id="0a5aa-118">String</span></span>|<span data-ttu-id="0a5aa-119">MSI アップグレードコード。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="0a5aa-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="0a5aa-120">requiresReboot</span></span>|<span data-ttu-id="0a5aa-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a5aa-121">Boolean</span></span>|<span data-ttu-id="0a5aa-122">MSI アプリがインストールを完了するためにコンピューターを再起動する必要があるかどうか。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="0a5aa-123">packageType</span><span class="sxs-lookup"><span data-stu-id="0a5aa-123">packageType</span></span>|[<span data-ttu-id="0a5aa-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="0a5aa-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="0a5aa-125">MSI パッケージの種類。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-125">The MSI package type.</span></span> <span data-ttu-id="0a5aa-126">可能な値は、`perMachine`、`perUser`、`dualPurpose` です。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="0a5aa-127">productName</span><span class="sxs-lookup"><span data-stu-id="0a5aa-127">productName</span></span>|<span data-ttu-id="0a5aa-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0a5aa-128">String</span></span>|<span data-ttu-id="0a5aa-129">MSI 製品名。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-129">The MSI product name.</span></span>|
|<span data-ttu-id="0a5aa-130">publisher</span><span class="sxs-lookup"><span data-stu-id="0a5aa-130">publisher</span></span>|<span data-ttu-id="0a5aa-131">String</span><span class="sxs-lookup"><span data-stu-id="0a5aa-131">String</span></span>|<span data-ttu-id="0a5aa-132">MSI パブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a5aa-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a5aa-133">Relationships</span></span>
<span data-ttu-id="0a5aa-134">なし</span><span class="sxs-lookup"><span data-stu-id="0a5aa-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a5aa-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a5aa-135">JSON Representation</span></span>
<span data-ttu-id="0a5aa-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a5aa-136">Here is a JSON representation of the resource.</span></span>
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



