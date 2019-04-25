---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb14092fa9f347e551a4871da69d9a3631b96e8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579178"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="91666-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91666-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="91666-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91666-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91666-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91666-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91666-106">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="91666-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="91666-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91666-107">Properties</span></span>
|<span data-ttu-id="91666-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91666-108">Property</span></span>|<span data-ttu-id="91666-109">型</span><span class="sxs-lookup"><span data-stu-id="91666-109">Type</span></span>|<span data-ttu-id="91666-110">説明</span><span class="sxs-lookup"><span data-stu-id="91666-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91666-111">displayName</span><span class="sxs-lookup"><span data-stu-id="91666-111">displayName</span></span>|<span data-ttu-id="91666-112">String</span><span class="sxs-lookup"><span data-stu-id="91666-112">String</span></span>|<span data-ttu-id="91666-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="91666-113">App display name.</span></span>|
|<span data-ttu-id="91666-114">説明</span><span class="sxs-lookup"><span data-stu-id="91666-114">description</span></span>|<span data-ttu-id="91666-115">String</span><span class="sxs-lookup"><span data-stu-id="91666-115">String</span></span>|<span data-ttu-id="91666-116">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="91666-116">The app's description.</span></span>|
|<span data-ttu-id="91666-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="91666-117">publisherName</span></span>|<span data-ttu-id="91666-118">String</span><span class="sxs-lookup"><span data-stu-id="91666-118">String</span></span>|<span data-ttu-id="91666-119">発行元名</span><span class="sxs-lookup"><span data-stu-id="91666-119">The publisher name</span></span>|
|<span data-ttu-id="91666-120">productName</span><span class="sxs-lookup"><span data-stu-id="91666-120">productName</span></span>|<span data-ttu-id="91666-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="91666-121">String</span></span>|<span data-ttu-id="91666-122">製品名。</span><span class="sxs-lookup"><span data-stu-id="91666-122">The product name.</span></span>|
|<span data-ttu-id="91666-123">denied</span><span class="sxs-lookup"><span data-stu-id="91666-123">denied</span></span>|<span data-ttu-id="91666-124">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="91666-124">Boolean</span></span>|<span data-ttu-id="91666-125">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="91666-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91666-126">関係</span><span class="sxs-lookup"><span data-stu-id="91666-126">Relationships</span></span>
<span data-ttu-id="91666-127">なし</span><span class="sxs-lookup"><span data-stu-id="91666-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91666-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91666-128">JSON Representation</span></span>
<span data-ttu-id="91666-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91666-129">Here is a JSON representation of the resource.</span></span>
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





