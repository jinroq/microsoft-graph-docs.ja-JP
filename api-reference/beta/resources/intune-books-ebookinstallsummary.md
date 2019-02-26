---
title: eBookInstallSummary リソース タイプ
description: デバイスのブックのインストール要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52d08d00bfbc26e0b72ddf53404eff8d55bb72b9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151241"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="91912-103">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="91912-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="91912-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91912-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91912-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91912-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91912-106">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="91912-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="91912-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="91912-107">Methods</span></span>
|<span data-ttu-id="91912-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="91912-108">Method</span></span>|<span data-ttu-id="91912-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="91912-109">Return Type</span></span>|<span data-ttu-id="91912-110">説明</span><span class="sxs-lookup"><span data-stu-id="91912-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91912-111">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="91912-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="91912-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="91912-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="91912-113">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="91912-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="91912-114">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="91912-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="91912-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="91912-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="91912-116">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="91912-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="91912-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91912-117">Properties</span></span>
|<span data-ttu-id="91912-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91912-118">Property</span></span>|<span data-ttu-id="91912-119">型</span><span class="sxs-lookup"><span data-stu-id="91912-119">Type</span></span>|<span data-ttu-id="91912-120">説明</span><span class="sxs-lookup"><span data-stu-id="91912-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91912-121">id</span><span class="sxs-lookup"><span data-stu-id="91912-121">id</span></span>|<span data-ttu-id="91912-122">String</span><span class="sxs-lookup"><span data-stu-id="91912-122">String</span></span>|<span data-ttu-id="91912-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="91912-123">Key of the entity.</span></span>|
|<span data-ttu-id="91912-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="91912-124">installedDeviceCount</span></span>|<span data-ttu-id="91912-125">Int32</span><span class="sxs-lookup"><span data-stu-id="91912-125">Int32</span></span>|<span data-ttu-id="91912-126">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="91912-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="91912-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="91912-127">failedDeviceCount</span></span>|<span data-ttu-id="91912-128">Int32</span><span class="sxs-lookup"><span data-stu-id="91912-128">Int32</span></span>|<span data-ttu-id="91912-129">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="91912-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="91912-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="91912-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="91912-131">Int32</span><span class="sxs-lookup"><span data-stu-id="91912-131">Int32</span></span>|<span data-ttu-id="91912-132">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="91912-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="91912-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="91912-133">installedUserCount</span></span>|<span data-ttu-id="91912-134">Int32</span><span class="sxs-lookup"><span data-stu-id="91912-134">Int32</span></span>|<span data-ttu-id="91912-135">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="91912-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="91912-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="91912-136">failedUserCount</span></span>|<span data-ttu-id="91912-137">Int32</span><span class="sxs-lookup"><span data-stu-id="91912-137">Int32</span></span>|<span data-ttu-id="91912-138">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="91912-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="91912-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="91912-139">notInstalledUserCount</span></span>|<span data-ttu-id="91912-140">Int32</span><span class="sxs-lookup"><span data-stu-id="91912-140">Int32</span></span>|<span data-ttu-id="91912-141">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="91912-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91912-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91912-142">Relationships</span></span>
<span data-ttu-id="91912-143">なし</span><span class="sxs-lookup"><span data-stu-id="91912-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91912-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91912-144">JSON Representation</span></span>
<span data-ttu-id="91912-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91912-145">Here is a JSON representation of the resource.</span></span>
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




