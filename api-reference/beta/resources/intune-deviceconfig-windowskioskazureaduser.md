---
title: windowsKioskAzureADUser リソースの種類
description: キオスク構成の AzureAD ユーザーアカウントを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93a47ba1bafe8f2070eedb028cb0eaa64808d03d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522490"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="05beb-103">windowsKioskAzureADUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="05beb-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="05beb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05beb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05beb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="05beb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05beb-106">キオスク構成の AzureAD ユーザーアカウントを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="05beb-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="05beb-107">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="05beb-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="05beb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05beb-108">Properties</span></span>
|<span data-ttu-id="05beb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05beb-109">Property</span></span>|<span data-ttu-id="05beb-110">型</span><span class="sxs-lookup"><span data-stu-id="05beb-110">Type</span></span>|<span data-ttu-id="05beb-111">説明</span><span class="sxs-lookup"><span data-stu-id="05beb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05beb-112">userId</span><span class="sxs-lookup"><span data-stu-id="05beb-112">userId</span></span>|<span data-ttu-id="05beb-113">String</span><span class="sxs-lookup"><span data-stu-id="05beb-113">String</span></span>|<span data-ttu-id="05beb-114">このキオスク構成にロックされる AzureAD ユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="05beb-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="05beb-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05beb-115">userPrincipalName</span></span>|<span data-ttu-id="05beb-116">String</span><span class="sxs-lookup"><span data-stu-id="05beb-116">String</span></span>|<span data-ttu-id="05beb-117">このキオスク構成にロックされるユーザーアカウント</span><span class="sxs-lookup"><span data-stu-id="05beb-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="05beb-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="05beb-118">Relationships</span></span>
<span data-ttu-id="05beb-119">なし</span><span class="sxs-lookup"><span data-stu-id="05beb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05beb-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05beb-120">JSON Representation</span></span>
<span data-ttu-id="05beb-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="05beb-121">Here is a JSON representation of the resource.</span></span>
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





