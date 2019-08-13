---
title: windowsKioskAzureADUser リソースの種類
description: キオスク構成の AzureAD ユーザーアカウントを識別するために使用されるクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a7f2f72fc9d7ed6b0e1209bcff2fa81a806c7e21
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370936"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="4de7d-103">windowsKioskAzureADUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4de7d-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="4de7d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4de7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4de7d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4de7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4de7d-106">キオスク構成の AzureAD ユーザーアカウントを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="4de7d-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="4de7d-107">[Windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="4de7d-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4de7d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4de7d-108">Properties</span></span>
|<span data-ttu-id="4de7d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4de7d-109">Property</span></span>|<span data-ttu-id="4de7d-110">型</span><span class="sxs-lookup"><span data-stu-id="4de7d-110">Type</span></span>|<span data-ttu-id="4de7d-111">説明</span><span class="sxs-lookup"><span data-stu-id="4de7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4de7d-112">userId</span><span class="sxs-lookup"><span data-stu-id="4de7d-112">userId</span></span>|<span data-ttu-id="4de7d-113">String</span><span class="sxs-lookup"><span data-stu-id="4de7d-113">String</span></span>|<span data-ttu-id="4de7d-114">このキオスク構成にロックされる AzureAD ユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="4de7d-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="4de7d-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4de7d-115">userPrincipalName</span></span>|<span data-ttu-id="4de7d-116">String</span><span class="sxs-lookup"><span data-stu-id="4de7d-116">String</span></span>|<span data-ttu-id="4de7d-117">このキオスク構成にロックされるユーザーアカウント</span><span class="sxs-lookup"><span data-stu-id="4de7d-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4de7d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4de7d-118">Relationships</span></span>
<span data-ttu-id="4de7d-119">なし</span><span class="sxs-lookup"><span data-stu-id="4de7d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4de7d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4de7d-120">JSON Representation</span></span>
<span data-ttu-id="4de7d-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4de7d-121">Here is a JSON representation of the resource.</span></span>
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



