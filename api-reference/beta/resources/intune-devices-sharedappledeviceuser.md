---
title: sharedAppleDeviceUser リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 46e0993c69a8ae34a54a654959d8d67a1b7f4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394433"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="0dd74-103">sharedAppleDeviceUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0dd74-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="0dd74-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0dd74-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0dd74-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dd74-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0dd74-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0dd74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dd74-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0dd74-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0dd74-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dd74-108">Properties</span></span>
|<span data-ttu-id="0dd74-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dd74-109">Property</span></span>|<span data-ttu-id="0dd74-110">型</span><span class="sxs-lookup"><span data-stu-id="0dd74-110">Type</span></span>|<span data-ttu-id="0dd74-111">説明</span><span class="sxs-lookup"><span data-stu-id="0dd74-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dd74-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0dd74-112">userPrincipalName</span></span>|<span data-ttu-id="0dd74-113">String</span><span class="sxs-lookup"><span data-stu-id="0dd74-113">String</span></span>|<span data-ttu-id="0dd74-114">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="0dd74-114">User name</span></span>|
|<span data-ttu-id="0dd74-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="0dd74-115">dataToSync</span></span>|<span data-ttu-id="0dd74-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0dd74-116">Boolean</span></span>|<span data-ttu-id="0dd74-117">データを同期します。</span><span class="sxs-lookup"><span data-stu-id="0dd74-117">Data to sync</span></span>|
|<span data-ttu-id="0dd74-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="0dd74-118">dataQuota</span></span>|<span data-ttu-id="0dd74-119">Int64</span><span class="sxs-lookup"><span data-stu-id="0dd74-119">Int64</span></span>|<span data-ttu-id="0dd74-120">データのクォータ</span><span class="sxs-lookup"><span data-stu-id="0dd74-120">Data quota</span></span>|
|<span data-ttu-id="0dd74-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="0dd74-121">dataUsed</span></span>|<span data-ttu-id="0dd74-122">Int64</span><span class="sxs-lookup"><span data-stu-id="0dd74-122">Int64</span></span>|<span data-ttu-id="0dd74-123">データのクォータ</span><span class="sxs-lookup"><span data-stu-id="0dd74-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dd74-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0dd74-124">Relationships</span></span>
<span data-ttu-id="0dd74-125">なし</span><span class="sxs-lookup"><span data-stu-id="0dd74-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dd74-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0dd74-126">JSON Representation</span></span>
<span data-ttu-id="0dd74-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0dd74-127">Here is a JSON representation of the resource.</span></span>
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




