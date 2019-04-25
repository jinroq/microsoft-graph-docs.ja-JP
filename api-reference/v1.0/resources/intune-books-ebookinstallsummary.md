---
title: eBookInstallSummary リソース タイプ
description: デバイスのブックのインストール要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17075183e0541669923a69c140d228cb1cbd4a2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523918"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="ac6a3-103">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="ac6a3-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="ac6a3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac6a3-105">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-105">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="ac6a3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac6a3-106">Methods</span></span>
|<span data-ttu-id="ac6a3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac6a3-107">Method</span></span>|<span data-ttu-id="ac6a3-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ac6a3-108">Return Type</span></span>|<span data-ttu-id="ac6a3-109">説明</span><span class="sxs-lookup"><span data-stu-id="ac6a3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ac6a3-110">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ac6a3-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="ac6a3-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ac6a3-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ac6a3-112">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="ac6a3-113">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ac6a3-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="ac6a3-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ac6a3-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ac6a3-115">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac6a3-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac6a3-116">Properties</span></span>
|<span data-ttu-id="ac6a3-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac6a3-117">Property</span></span>|<span data-ttu-id="ac6a3-118">型</span><span class="sxs-lookup"><span data-stu-id="ac6a3-118">Type</span></span>|<span data-ttu-id="ac6a3-119">説明</span><span class="sxs-lookup"><span data-stu-id="ac6a3-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac6a3-120">id</span><span class="sxs-lookup"><span data-stu-id="ac6a3-120">id</span></span>|<span data-ttu-id="ac6a3-121">String</span><span class="sxs-lookup"><span data-stu-id="ac6a3-121">String</span></span>|<span data-ttu-id="ac6a3-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-122">Key of the entity.</span></span>|
|<span data-ttu-id="ac6a3-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac6a3-123">installedDeviceCount</span></span>|<span data-ttu-id="ac6a3-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6a3-124">Int32</span></span>|<span data-ttu-id="ac6a3-125">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="ac6a3-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac6a3-126">failedDeviceCount</span></span>|<span data-ttu-id="ac6a3-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6a3-127">Int32</span></span>|<span data-ttu-id="ac6a3-128">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="ac6a3-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac6a3-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="ac6a3-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6a3-130">Int32</span></span>|<span data-ttu-id="ac6a3-131">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="ac6a3-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ac6a3-132">installedUserCount</span></span>|<span data-ttu-id="ac6a3-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6a3-133">Int32</span></span>|<span data-ttu-id="ac6a3-134">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="ac6a3-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ac6a3-135">failedUserCount</span></span>|<span data-ttu-id="ac6a3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6a3-136">Int32</span></span>|<span data-ttu-id="ac6a3-137">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="ac6a3-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ac6a3-138">notInstalledUserCount</span></span>|<span data-ttu-id="ac6a3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6a3-139">Int32</span></span>|<span data-ttu-id="ac6a3-140">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac6a3-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac6a3-141">Relationships</span></span>
<span data-ttu-id="ac6a3-142">なし</span><span class="sxs-lookup"><span data-stu-id="ac6a3-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac6a3-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac6a3-143">JSON Representation</span></span>
<span data-ttu-id="ac6a3-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac6a3-144">Here is a JSON representation of the resource.</span></span>
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



