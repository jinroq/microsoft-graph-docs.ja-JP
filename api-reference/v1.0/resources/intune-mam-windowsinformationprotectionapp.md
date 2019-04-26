---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d329baea829fa8fb7664895382a377f53461ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561203"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="2d3e5-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d3e5-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="2d3e5-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d3e5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d3e5-105">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="2d3e5-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="2d3e5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d3e5-106">Properties</span></span>
|<span data-ttu-id="2d3e5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d3e5-107">Property</span></span>|<span data-ttu-id="2d3e5-108">型</span><span class="sxs-lookup"><span data-stu-id="2d3e5-108">Type</span></span>|<span data-ttu-id="2d3e5-109">説明</span><span class="sxs-lookup"><span data-stu-id="2d3e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d3e5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="2d3e5-110">displayName</span></span>|<span data-ttu-id="2d3e5-111">String</span><span class="sxs-lookup"><span data-stu-id="2d3e5-111">String</span></span>|<span data-ttu-id="2d3e5-112">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="2d3e5-112">App display name.</span></span>|
|<span data-ttu-id="2d3e5-113">description</span><span class="sxs-lookup"><span data-stu-id="2d3e5-113">description</span></span>|<span data-ttu-id="2d3e5-114">String</span><span class="sxs-lookup"><span data-stu-id="2d3e5-114">String</span></span>|<span data-ttu-id="2d3e5-115">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="2d3e5-115">The app's description.</span></span>|
|<span data-ttu-id="2d3e5-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="2d3e5-116">publisherName</span></span>|<span data-ttu-id="2d3e5-117">String</span><span class="sxs-lookup"><span data-stu-id="2d3e5-117">String</span></span>|<span data-ttu-id="2d3e5-118">発行元名</span><span class="sxs-lookup"><span data-stu-id="2d3e5-118">The publisher name</span></span>|
|<span data-ttu-id="2d3e5-119">productName</span><span class="sxs-lookup"><span data-stu-id="2d3e5-119">productName</span></span>|<span data-ttu-id="2d3e5-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2d3e5-120">String</span></span>|<span data-ttu-id="2d3e5-121">製品名。</span><span class="sxs-lookup"><span data-stu-id="2d3e5-121">The product name.</span></span>|
|<span data-ttu-id="2d3e5-122">denied</span><span class="sxs-lookup"><span data-stu-id="2d3e5-122">denied</span></span>|<span data-ttu-id="2d3e5-123">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2d3e5-123">Boolean</span></span>|<span data-ttu-id="2d3e5-124">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="2d3e5-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d3e5-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d3e5-125">Relationships</span></span>
<span data-ttu-id="2d3e5-126">なし</span><span class="sxs-lookup"><span data-stu-id="2d3e5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d3e5-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d3e5-127">JSON Representation</span></span>
<span data-ttu-id="2d3e5-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2d3e5-128">Here is a JSON representation of the resource.</span></span>
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



