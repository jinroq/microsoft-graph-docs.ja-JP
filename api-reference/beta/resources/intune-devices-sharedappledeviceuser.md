---
title: sharedAppleDeviceUser リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 79ebc5ae520c1c9b40bffb6a86e95693c52fa1e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068431"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="f5361-103">sharedAppleDeviceUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5361-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="f5361-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5361-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5361-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5361-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5361-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f5361-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5361-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f5361-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f5361-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5361-108">Properties</span></span>
|<span data-ttu-id="f5361-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5361-109">Property</span></span>|<span data-ttu-id="f5361-110">型</span><span class="sxs-lookup"><span data-stu-id="f5361-110">Type</span></span>|<span data-ttu-id="f5361-111">説明</span><span class="sxs-lookup"><span data-stu-id="f5361-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5361-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f5361-112">userPrincipalName</span></span>|<span data-ttu-id="f5361-113">String</span><span class="sxs-lookup"><span data-stu-id="f5361-113">String</span></span>|<span data-ttu-id="f5361-114">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="f5361-114">User name</span></span>|
|<span data-ttu-id="f5361-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="f5361-115">dataToSync</span></span>|<span data-ttu-id="f5361-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="f5361-116">Boolean</span></span>|<span data-ttu-id="f5361-117">データを同期します。</span><span class="sxs-lookup"><span data-stu-id="f5361-117">Data to sync</span></span>|
|<span data-ttu-id="f5361-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="f5361-118">dataQuota</span></span>|<span data-ttu-id="f5361-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f5361-119">Int64</span></span>|<span data-ttu-id="f5361-120">データのクォータ</span><span class="sxs-lookup"><span data-stu-id="f5361-120">Data quota</span></span>|
|<span data-ttu-id="f5361-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="f5361-121">dataUsed</span></span>|<span data-ttu-id="f5361-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f5361-122">Int64</span></span>|<span data-ttu-id="f5361-123">データのクォータ</span><span class="sxs-lookup"><span data-stu-id="f5361-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5361-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5361-124">Relationships</span></span>
<span data-ttu-id="f5361-125">なし</span><span class="sxs-lookup"><span data-stu-id="f5361-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f5361-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5361-126">JSON Representation</span></span>
<span data-ttu-id="f5361-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5361-127">Here is a JSON representation of the resource.</span></span>
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





