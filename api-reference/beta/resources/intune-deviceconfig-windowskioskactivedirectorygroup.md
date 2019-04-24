---
title: windowsKioskActiveDirectoryGroup リソースの種類
description: キオスク構成の Azure ディレクトリグループを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20f4c0eaf8470f01619a9ff4067bec0d95851b3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464625"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="54cba-103">windowsKioskActiveDirectoryGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54cba-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="54cba-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54cba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54cba-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54cba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54cba-106">キオスク構成の Azure ディレクトリグループを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="54cba-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="54cba-107">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="54cba-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="54cba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54cba-108">Properties</span></span>
|<span data-ttu-id="54cba-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54cba-109">Property</span></span>|<span data-ttu-id="54cba-110">型</span><span class="sxs-lookup"><span data-stu-id="54cba-110">Type</span></span>|<span data-ttu-id="54cba-111">説明</span><span class="sxs-lookup"><span data-stu-id="54cba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54cba-112">groupName</span><span class="sxs-lookup"><span data-stu-id="54cba-112">groupName</span></span>|<span data-ttu-id="54cba-113">String</span><span class="sxs-lookup"><span data-stu-id="54cba-113">String</span></span>|<span data-ttu-id="54cba-114">このキオスク構成にロックされる AD グループの名前</span><span class="sxs-lookup"><span data-stu-id="54cba-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="54cba-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54cba-115">Relationships</span></span>
<span data-ttu-id="54cba-116">なし</span><span class="sxs-lookup"><span data-stu-id="54cba-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54cba-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54cba-117">JSON Representation</span></span>
<span data-ttu-id="54cba-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54cba-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





