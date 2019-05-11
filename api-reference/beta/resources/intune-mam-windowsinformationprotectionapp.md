---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72b7654712241549aaa1377e48dfdc856dd3bc1b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940611"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="1d4f2-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d4f2-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="1d4f2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d4f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d4f2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d4f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d4f2-106">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="1d4f2-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="1d4f2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d4f2-107">Properties</span></span>
|<span data-ttu-id="1d4f2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d4f2-108">Property</span></span>|<span data-ttu-id="1d4f2-109">型</span><span class="sxs-lookup"><span data-stu-id="1d4f2-109">Type</span></span>|<span data-ttu-id="1d4f2-110">説明</span><span class="sxs-lookup"><span data-stu-id="1d4f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d4f2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1d4f2-111">displayName</span></span>|<span data-ttu-id="1d4f2-112">文字列</span><span class="sxs-lookup"><span data-stu-id="1d4f2-112">String</span></span>|<span data-ttu-id="1d4f2-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="1d4f2-113">App display name.</span></span>|
|<span data-ttu-id="1d4f2-114">description</span><span class="sxs-lookup"><span data-stu-id="1d4f2-114">description</span></span>|<span data-ttu-id="1d4f2-115">String</span><span class="sxs-lookup"><span data-stu-id="1d4f2-115">String</span></span>|<span data-ttu-id="1d4f2-116">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="1d4f2-116">The app's description.</span></span>|
|<span data-ttu-id="1d4f2-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="1d4f2-117">publisherName</span></span>|<span data-ttu-id="1d4f2-118">String</span><span class="sxs-lookup"><span data-stu-id="1d4f2-118">String</span></span>|<span data-ttu-id="1d4f2-119">発行元名</span><span class="sxs-lookup"><span data-stu-id="1d4f2-119">The publisher name</span></span>|
|<span data-ttu-id="1d4f2-120">productName</span><span class="sxs-lookup"><span data-stu-id="1d4f2-120">productName</span></span>|<span data-ttu-id="1d4f2-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1d4f2-121">String</span></span>|<span data-ttu-id="1d4f2-122">製品名。</span><span class="sxs-lookup"><span data-stu-id="1d4f2-122">The product name.</span></span>|
|<span data-ttu-id="1d4f2-123">denied</span><span class="sxs-lookup"><span data-stu-id="1d4f2-123">denied</span></span>|<span data-ttu-id="1d4f2-124">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1d4f2-124">Boolean</span></span>|<span data-ttu-id="1d4f2-125">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="1d4f2-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d4f2-126">関係</span><span class="sxs-lookup"><span data-stu-id="1d4f2-126">Relationships</span></span>
<span data-ttu-id="1d4f2-127">なし</span><span class="sxs-lookup"><span data-stu-id="1d4f2-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d4f2-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d4f2-128">JSON Representation</span></span>
<span data-ttu-id="1d4f2-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d4f2-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```




