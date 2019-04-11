---
title: sharedAppleDeviceUser リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43bc64243cb330f0761c8ded3ab646a0cde4f926
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778006"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="f555d-103">sharedAppleDeviceUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f555d-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="f555d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f555d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f555d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f555d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f555d-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f555d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f555d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f555d-107">Properties</span></span>
|<span data-ttu-id="f555d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f555d-108">Property</span></span>|<span data-ttu-id="f555d-109">型</span><span class="sxs-lookup"><span data-stu-id="f555d-109">Type</span></span>|<span data-ttu-id="f555d-110">説明</span><span class="sxs-lookup"><span data-stu-id="f555d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f555d-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f555d-111">userPrincipalName</span></span>|<span data-ttu-id="f555d-112">String</span><span class="sxs-lookup"><span data-stu-id="f555d-112">String</span></span>|<span data-ttu-id="f555d-113">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="f555d-113">User name</span></span>|
|<span data-ttu-id="f555d-114">datatosync</span><span class="sxs-lookup"><span data-stu-id="f555d-114">dataToSync</span></span>|<span data-ttu-id="f555d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f555d-115">Boolean</span></span>|<span data-ttu-id="f555d-116">同期するデータ</span><span class="sxs-lookup"><span data-stu-id="f555d-116">Data to sync</span></span>|
|<span data-ttu-id="f555d-117">dataquota</span><span class="sxs-lookup"><span data-stu-id="f555d-117">dataQuota</span></span>|<span data-ttu-id="f555d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f555d-118">Int64</span></span>|<span data-ttu-id="f555d-119">データクォータ</span><span class="sxs-lookup"><span data-stu-id="f555d-119">Data quota</span></span>|
|<span data-ttu-id="f555d-120">使用されるデータ</span><span class="sxs-lookup"><span data-stu-id="f555d-120">dataUsed</span></span>|<span data-ttu-id="f555d-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f555d-121">Int64</span></span>|<span data-ttu-id="f555d-122">データクォータ</span><span class="sxs-lookup"><span data-stu-id="f555d-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="f555d-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f555d-123">Relationships</span></span>
<span data-ttu-id="f555d-124">なし</span><span class="sxs-lookup"><span data-stu-id="f555d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f555d-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f555d-125">JSON Representation</span></span>
<span data-ttu-id="f555d-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f555d-126">Here is a JSON representation of the resource.</span></span>
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





