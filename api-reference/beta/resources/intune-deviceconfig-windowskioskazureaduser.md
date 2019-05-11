---
title: windowsKioskAzureADUser リソースの種類
description: キオスク構成の AzureAD ユーザーアカウントを識別するために使用されるクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96d91f585d8c762a2e1080d38bfd7cebb75e3acc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943949"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="185d8-103">windowsKioskAzureADUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="185d8-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="185d8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="185d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="185d8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="185d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="185d8-106">キオスク構成の AzureAD ユーザーアカウントを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="185d8-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="185d8-107">[Windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="185d8-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="185d8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="185d8-108">Properties</span></span>
|<span data-ttu-id="185d8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="185d8-109">Property</span></span>|<span data-ttu-id="185d8-110">型</span><span class="sxs-lookup"><span data-stu-id="185d8-110">Type</span></span>|<span data-ttu-id="185d8-111">説明</span><span class="sxs-lookup"><span data-stu-id="185d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="185d8-112">userId</span><span class="sxs-lookup"><span data-stu-id="185d8-112">userId</span></span>|<span data-ttu-id="185d8-113">String</span><span class="sxs-lookup"><span data-stu-id="185d8-113">String</span></span>|<span data-ttu-id="185d8-114">このキオスク構成にロックされる AzureAD ユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="185d8-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="185d8-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="185d8-115">userPrincipalName</span></span>|<span data-ttu-id="185d8-116">String</span><span class="sxs-lookup"><span data-stu-id="185d8-116">String</span></span>|<span data-ttu-id="185d8-117">このキオスク構成にロックされるユーザーアカウント</span><span class="sxs-lookup"><span data-stu-id="185d8-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="185d8-118">関係</span><span class="sxs-lookup"><span data-stu-id="185d8-118">Relationships</span></span>
<span data-ttu-id="185d8-119">なし</span><span class="sxs-lookup"><span data-stu-id="185d8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="185d8-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="185d8-120">JSON Representation</span></span>
<span data-ttu-id="185d8-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="185d8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```




