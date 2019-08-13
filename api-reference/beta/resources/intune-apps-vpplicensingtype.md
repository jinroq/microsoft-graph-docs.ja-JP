---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4303a77b2aa9a403c7d618e8b8cc07ddb7b3774f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335775"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="8a545-103">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a545-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="8a545-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a545-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a545-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a545-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a545-106">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8a545-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="8a545-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a545-107">Properties</span></span>
|<span data-ttu-id="8a545-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a545-108">Property</span></span>|<span data-ttu-id="8a545-109">型</span><span class="sxs-lookup"><span data-stu-id="8a545-109">Type</span></span>|<span data-ttu-id="8a545-110">説明</span><span class="sxs-lookup"><span data-stu-id="8a545-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a545-111">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="8a545-111">supportUserLicensing</span></span>|<span data-ttu-id="8a545-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a545-112">Boolean</span></span>|<span data-ttu-id="8a545-113">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="8a545-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="8a545-114">supportdevicelicenel</span><span class="sxs-lookup"><span data-stu-id="8a545-114">supportDeviceLicensing</span></span>|<span data-ttu-id="8a545-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8a545-115">Boolean</span></span>|<span data-ttu-id="8a545-116">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="8a545-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="8a545-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="8a545-117">supportsUserLicensing</span></span>|<span data-ttu-id="8a545-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a545-118">Boolean</span></span>|<span data-ttu-id="8a545-119">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="8a545-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="8a545-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8a545-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="8a545-121">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8a545-121">Boolean</span></span>|<span data-ttu-id="8a545-122">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="8a545-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a545-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a545-123">Relationships</span></span>
<span data-ttu-id="8a545-124">なし</span><span class="sxs-lookup"><span data-stu-id="8a545-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a545-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a545-125">JSON Representation</span></span>
<span data-ttu-id="8a545-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a545-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



