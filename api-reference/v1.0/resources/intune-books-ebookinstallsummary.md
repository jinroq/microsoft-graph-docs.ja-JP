---
title: eBookInstallSummary リソース タイプ
description: デバイスのブックのインストール要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82bc37303f815e782c3d2aac8e0c1b13eb8e6ec0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028848"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="ab541-103">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="ab541-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="ab541-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ab541-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab541-105">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab541-105">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="ab541-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab541-106">Methods</span></span>
|<span data-ttu-id="ab541-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab541-107">Method</span></span>|<span data-ttu-id="ab541-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ab541-108">Return Type</span></span>|<span data-ttu-id="ab541-109">説明</span><span class="sxs-lookup"><span data-stu-id="ab541-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab541-110">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab541-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="ab541-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab541-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ab541-112">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ab541-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="ab541-113">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab541-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="ab541-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab541-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ab541-115">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab541-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab541-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab541-116">Properties</span></span>
|<span data-ttu-id="ab541-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab541-117">Property</span></span>|<span data-ttu-id="ab541-118">型</span><span class="sxs-lookup"><span data-stu-id="ab541-118">Type</span></span>|<span data-ttu-id="ab541-119">説明</span><span class="sxs-lookup"><span data-stu-id="ab541-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab541-120">id</span><span class="sxs-lookup"><span data-stu-id="ab541-120">id</span></span>|<span data-ttu-id="ab541-121">String</span><span class="sxs-lookup"><span data-stu-id="ab541-121">String</span></span>|<span data-ttu-id="ab541-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ab541-122">Key of the entity.</span></span>|
|<span data-ttu-id="ab541-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab541-123">installedDeviceCount</span></span>|<span data-ttu-id="ab541-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-124">Int32</span></span>|<span data-ttu-id="ab541-125">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ab541-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="ab541-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab541-126">failedDeviceCount</span></span>|<span data-ttu-id="ab541-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-127">Int32</span></span>|<span data-ttu-id="ab541-128">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ab541-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="ab541-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab541-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="ab541-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-130">Int32</span></span>|<span data-ttu-id="ab541-131">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ab541-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="ab541-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ab541-132">installedUserCount</span></span>|<span data-ttu-id="ab541-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-133">Int32</span></span>|<span data-ttu-id="ab541-134">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="ab541-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="ab541-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ab541-135">failedUserCount</span></span>|<span data-ttu-id="ab541-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-136">Int32</span></span>|<span data-ttu-id="ab541-137">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="ab541-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="ab541-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ab541-138">notInstalledUserCount</span></span>|<span data-ttu-id="ab541-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-139">Int32</span></span>|<span data-ttu-id="ab541-140">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="ab541-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab541-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab541-141">Relationships</span></span>
<span data-ttu-id="ab541-142">なし</span><span class="sxs-lookup"><span data-stu-id="ab541-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab541-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab541-143">JSON Representation</span></span>
<span data-ttu-id="ab541-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ab541-144">Here is a JSON representation of the resource.</span></span>
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



