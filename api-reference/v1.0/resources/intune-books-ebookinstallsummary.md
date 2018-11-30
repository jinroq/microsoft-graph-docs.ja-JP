---
title: eBookInstallSummary リソース タイプ
description: デバイスのブックのインストール要約のプロパティが含まれています。
ms.openlocfilehash: 59754a8b925f573e44abd9ae1f674ab3f08f51c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023657"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="29d9f-103">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="29d9f-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="29d9f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29d9f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29d9f-105">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="29d9f-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="29d9f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="29d9f-106">Methods</span></span>
|<span data-ttu-id="29d9f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="29d9f-107">Method</span></span>|<span data-ttu-id="29d9f-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="29d9f-108">Return Type</span></span>|<span data-ttu-id="29d9f-109">説明</span><span class="sxs-lookup"><span data-stu-id="29d9f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29d9f-110">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="29d9f-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="29d9f-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="29d9f-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="29d9f-112">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="29d9f-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="29d9f-113">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="29d9f-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="29d9f-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="29d9f-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="29d9f-115">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="29d9f-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29d9f-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29d9f-116">Properties</span></span>
|<span data-ttu-id="29d9f-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29d9f-117">Property</span></span>|<span data-ttu-id="29d9f-118">型</span><span class="sxs-lookup"><span data-stu-id="29d9f-118">Type</span></span>|<span data-ttu-id="29d9f-119">説明</span><span class="sxs-lookup"><span data-stu-id="29d9f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29d9f-120">id</span><span class="sxs-lookup"><span data-stu-id="29d9f-120">id</span></span>|<span data-ttu-id="29d9f-121">String</span><span class="sxs-lookup"><span data-stu-id="29d9f-121">String</span></span>|<span data-ttu-id="29d9f-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="29d9f-122">Key of the entity.</span></span>|
|<span data-ttu-id="29d9f-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="29d9f-123">installedDeviceCount</span></span>|<span data-ttu-id="29d9f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="29d9f-124">Int32</span></span>|<span data-ttu-id="29d9f-125">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="29d9f-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="29d9f-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="29d9f-126">failedDeviceCount</span></span>|<span data-ttu-id="29d9f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="29d9f-127">Int32</span></span>|<span data-ttu-id="29d9f-128">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="29d9f-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="29d9f-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="29d9f-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="29d9f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="29d9f-130">Int32</span></span>|<span data-ttu-id="29d9f-131">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="29d9f-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="29d9f-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="29d9f-132">installedUserCount</span></span>|<span data-ttu-id="29d9f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="29d9f-133">Int32</span></span>|<span data-ttu-id="29d9f-134">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="29d9f-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="29d9f-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="29d9f-135">failedUserCount</span></span>|<span data-ttu-id="29d9f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="29d9f-136">Int32</span></span>|<span data-ttu-id="29d9f-137">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="29d9f-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="29d9f-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="29d9f-138">notInstalledUserCount</span></span>|<span data-ttu-id="29d9f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="29d9f-139">Int32</span></span>|<span data-ttu-id="29d9f-140">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="29d9f-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29d9f-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29d9f-141">Relationships</span></span>
<span data-ttu-id="29d9f-142">なし</span><span class="sxs-lookup"><span data-stu-id="29d9f-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="29d9f-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29d9f-143">JSON Representation</span></span>
<span data-ttu-id="29d9f-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29d9f-144">Here is a JSON representation of the resource.</span></span>
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



