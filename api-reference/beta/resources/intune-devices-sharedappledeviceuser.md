---
title: sharedAppleDeviceUser リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff51ad89600919fb1ed2c3bb506a53178ccdc445
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941752"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="f6069-103">sharedAppleDeviceUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6069-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="f6069-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6069-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6069-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6069-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6069-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f6069-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f6069-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6069-107">Properties</span></span>
|<span data-ttu-id="f6069-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6069-108">Property</span></span>|<span data-ttu-id="f6069-109">型</span><span class="sxs-lookup"><span data-stu-id="f6069-109">Type</span></span>|<span data-ttu-id="f6069-110">説明</span><span class="sxs-lookup"><span data-stu-id="f6069-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6069-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6069-111">userPrincipalName</span></span>|<span data-ttu-id="f6069-112">String</span><span class="sxs-lookup"><span data-stu-id="f6069-112">String</span></span>|<span data-ttu-id="f6069-113">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="f6069-113">User name</span></span>|
|<span data-ttu-id="f6069-114">dataToSync</span><span class="sxs-lookup"><span data-stu-id="f6069-114">dataToSync</span></span>|<span data-ttu-id="f6069-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6069-115">Boolean</span></span>|<span data-ttu-id="f6069-116">同期するデータ</span><span class="sxs-lookup"><span data-stu-id="f6069-116">Data to sync</span></span>|
|<span data-ttu-id="f6069-117">dataQuota</span><span class="sxs-lookup"><span data-stu-id="f6069-117">dataQuota</span></span>|<span data-ttu-id="f6069-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f6069-118">Int64</span></span>|<span data-ttu-id="f6069-119">データクォータ</span><span class="sxs-lookup"><span data-stu-id="f6069-119">Data quota</span></span>|
|<span data-ttu-id="f6069-120">使用されるデータ</span><span class="sxs-lookup"><span data-stu-id="f6069-120">dataUsed</span></span>|<span data-ttu-id="f6069-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f6069-121">Int64</span></span>|<span data-ttu-id="f6069-122">データクォータ</span><span class="sxs-lookup"><span data-stu-id="f6069-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6069-123">関係</span><span class="sxs-lookup"><span data-stu-id="f6069-123">Relationships</span></span>
<span data-ttu-id="f6069-124">なし</span><span class="sxs-lookup"><span data-stu-id="f6069-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6069-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6069-125">JSON Representation</span></span>
<span data-ttu-id="f6069-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f6069-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```




