---
title: eBookInstallSummary リソース タイプ
description: デバイスのブックのインストール要約のプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4e8952012624a038f497fea3c6b81ad364448a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415342"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="84cd7-103">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="84cd7-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="84cd7-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="84cd7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84cd7-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84cd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84cd7-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="84cd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84cd7-107">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="84cd7-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="84cd7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="84cd7-108">Methods</span></span>
|<span data-ttu-id="84cd7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="84cd7-109">Method</span></span>|<span data-ttu-id="84cd7-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="84cd7-110">Return Type</span></span>|<span data-ttu-id="84cd7-111">説明</span><span class="sxs-lookup"><span data-stu-id="84cd7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84cd7-112">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="84cd7-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="84cd7-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="84cd7-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="84cd7-114">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="84cd7-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="84cd7-115">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="84cd7-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="84cd7-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="84cd7-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="84cd7-117">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="84cd7-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84cd7-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84cd7-118">Properties</span></span>
|<span data-ttu-id="84cd7-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84cd7-119">Property</span></span>|<span data-ttu-id="84cd7-120">型</span><span class="sxs-lookup"><span data-stu-id="84cd7-120">Type</span></span>|<span data-ttu-id="84cd7-121">説明</span><span class="sxs-lookup"><span data-stu-id="84cd7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84cd7-122">id</span><span class="sxs-lookup"><span data-stu-id="84cd7-122">id</span></span>|<span data-ttu-id="84cd7-123">String</span><span class="sxs-lookup"><span data-stu-id="84cd7-123">String</span></span>|<span data-ttu-id="84cd7-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="84cd7-124">Key of the entity.</span></span>|
|<span data-ttu-id="84cd7-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="84cd7-125">installedDeviceCount</span></span>|<span data-ttu-id="84cd7-126">Int32</span><span class="sxs-lookup"><span data-stu-id="84cd7-126">Int32</span></span>|<span data-ttu-id="84cd7-127">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="84cd7-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="84cd7-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="84cd7-128">failedDeviceCount</span></span>|<span data-ttu-id="84cd7-129">Int32</span><span class="sxs-lookup"><span data-stu-id="84cd7-129">Int32</span></span>|<span data-ttu-id="84cd7-130">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="84cd7-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="84cd7-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="84cd7-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="84cd7-132">Int32</span><span class="sxs-lookup"><span data-stu-id="84cd7-132">Int32</span></span>|<span data-ttu-id="84cd7-133">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="84cd7-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="84cd7-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="84cd7-134">installedUserCount</span></span>|<span data-ttu-id="84cd7-135">Int32</span><span class="sxs-lookup"><span data-stu-id="84cd7-135">Int32</span></span>|<span data-ttu-id="84cd7-136">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="84cd7-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="84cd7-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="84cd7-137">failedUserCount</span></span>|<span data-ttu-id="84cd7-138">Int32</span><span class="sxs-lookup"><span data-stu-id="84cd7-138">Int32</span></span>|<span data-ttu-id="84cd7-139">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="84cd7-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="84cd7-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="84cd7-140">notInstalledUserCount</span></span>|<span data-ttu-id="84cd7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="84cd7-141">Int32</span></span>|<span data-ttu-id="84cd7-142">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="84cd7-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84cd7-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="84cd7-143">Relationships</span></span>
<span data-ttu-id="84cd7-144">なし</span><span class="sxs-lookup"><span data-stu-id="84cd7-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84cd7-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84cd7-145">JSON Representation</span></span>
<span data-ttu-id="84cd7-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="84cd7-146">Here is a JSON representation of the resource.</span></span>
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




