---
title: eBookInstallSummary リソース タイプ
description: デバイスのブックのインストール要約のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 722e293f8b5e2ee1be4eaed38040e648b76d60ee
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949417"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="aff01-103">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="aff01-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="aff01-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aff01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aff01-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aff01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aff01-106">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="aff01-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="aff01-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="aff01-107">Methods</span></span>
|<span data-ttu-id="aff01-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="aff01-108">Method</span></span>|<span data-ttu-id="aff01-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aff01-109">Return Type</span></span>|<span data-ttu-id="aff01-110">説明</span><span class="sxs-lookup"><span data-stu-id="aff01-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aff01-111">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="aff01-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="aff01-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="aff01-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="aff01-113">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aff01-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="aff01-114">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="aff01-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="aff01-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="aff01-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="aff01-116">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aff01-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aff01-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aff01-117">Properties</span></span>
|<span data-ttu-id="aff01-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aff01-118">Property</span></span>|<span data-ttu-id="aff01-119">型</span><span class="sxs-lookup"><span data-stu-id="aff01-119">Type</span></span>|<span data-ttu-id="aff01-120">説明</span><span class="sxs-lookup"><span data-stu-id="aff01-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff01-121">id</span><span class="sxs-lookup"><span data-stu-id="aff01-121">id</span></span>|<span data-ttu-id="aff01-122">String</span><span class="sxs-lookup"><span data-stu-id="aff01-122">String</span></span>|<span data-ttu-id="aff01-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aff01-123">Key of the entity.</span></span>|
|<span data-ttu-id="aff01-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aff01-124">installedDeviceCount</span></span>|<span data-ttu-id="aff01-125">Int32</span><span class="sxs-lookup"><span data-stu-id="aff01-125">Int32</span></span>|<span data-ttu-id="aff01-126">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="aff01-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="aff01-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aff01-127">failedDeviceCount</span></span>|<span data-ttu-id="aff01-128">Int32</span><span class="sxs-lookup"><span data-stu-id="aff01-128">Int32</span></span>|<span data-ttu-id="aff01-129">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="aff01-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="aff01-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aff01-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="aff01-131">Int32</span><span class="sxs-lookup"><span data-stu-id="aff01-131">Int32</span></span>|<span data-ttu-id="aff01-132">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="aff01-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="aff01-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="aff01-133">installedUserCount</span></span>|<span data-ttu-id="aff01-134">Int32</span><span class="sxs-lookup"><span data-stu-id="aff01-134">Int32</span></span>|<span data-ttu-id="aff01-135">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="aff01-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="aff01-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="aff01-136">failedUserCount</span></span>|<span data-ttu-id="aff01-137">Int32</span><span class="sxs-lookup"><span data-stu-id="aff01-137">Int32</span></span>|<span data-ttu-id="aff01-138">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="aff01-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="aff01-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="aff01-139">notInstalledUserCount</span></span>|<span data-ttu-id="aff01-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aff01-140">Int32</span></span>|<span data-ttu-id="aff01-141">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="aff01-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aff01-142">関係</span><span class="sxs-lookup"><span data-stu-id="aff01-142">Relationships</span></span>
<span data-ttu-id="aff01-143">なし</span><span class="sxs-lookup"><span data-stu-id="aff01-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aff01-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aff01-144">JSON Representation</span></span>
<span data-ttu-id="aff01-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aff01-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```




